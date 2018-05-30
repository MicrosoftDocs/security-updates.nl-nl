---
TOCTitle: Intrekkingslijsten maken
Title: Intrekkingslijsten maken
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18113849
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720208(v=WS.10)'
---

Intrekkingslijsten maken
========================

Wanneer u intrekking wilt implementeren, moet u een intrekkingslijst distribueren. Een intrekkingslijst is een XML-document waarin XrML-taal (eXtensible Rights Markup Language) wordt gebruikt en waarin de principals zijn opgenomen die geen toegang meer mogen krijgen tot met rechten beveiligde inhoud. Met het hulpprogramma Revocation List Signing (RLsigner.exe) dat bij RMS wordt geleverd, voorziet u de intrekkingslijsten van een tijdstempel en een correcte handtekening.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Belangrijk                                                      |
|---------------------------------------------------------------------------------------------------------------------------------------|
| Als u de intrekkingslijst wilt ondertekenen met RLsigner.exe, moet u het bestand met de intrekkingslijst opslaan als Unicode-bestand. |

Voorbeeld van een intrekkingslijst
----------------------------------

In dit onderwerp wordt een voorbeeld van een intrekkingslijst gegeven waarin alle mogelijke intrekkingsmechanismen worden weergegeven. U kunt dit voorbeeld als model voor uw eigen intrekkingslijsten gebruiken.

Een intrekkingslijst is een XML-bestand waarin gebruik wordt gemaakt van de XrML-taal.

Het element BODY bevat vier onderliggende elementen:

-   **ISSUEDTIME**. Bevat de datum en het tijdstip waarop de intrekkingslijst is uitgegeven. RLsigner.exe voegt dit element in in het bestand. In dit voorbeeld wordt dit element alleen weergegeven om de algehele structuur van het intrekkingslijstbestand te tonen.
-   **DESCRIPTOR**. Bevat gegevens waarmee het bestand wordt geïdentificeerd als een intrekkingslijst.
-   **ISSUER**. Bevat gegevens waarmee de entiteit wordt geïdentificeerd die de intrekkingslijst uitgeeft.
-   **REVOCATIONLIST**. Bevat de onderliggende REVOKE-elementen waarmee wordt aangegeven welke entiteiten worden ingetrokken met deze lijst.

Onderstaand ziet u een voorbeeld van een intrekkingslijstbestand.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------|
```
    <?xml version="1.0" ?> 
    <XrML xml:space=”preserve” version=”1.2”>
    <BODY type="LICENSE" version="3.0">
        <ISSUEDTIME>...</ISSUEDTIME> 
        <DESCRIPTOR>
        <OBJECT type="Revocation-List">
            <ID type="MS-GUID">{d6373cba-01f1-4f32-ac58-260f580af0f8}</ID>
        </OBJECT>
        </DESCRIPTOR>
    &lt;ISSUER&gt;
        <OBJECT type="Revocation-List">
            <ID type="acsii-tag">External revocation authority</ID>
            <NAME>Revocation list name</NAME>
            <ADDRESS type="URL">https://somedomain.com/revocation_list_file</ADDRESS>
        </OBJECT>
       <PUBLICKEY&>...</PUBLICKEY>
        </ISSUER>
    <REVOCATIONLIST>
        <REVOKE>...<\REVOKE>
        <REVOKE>...<\REVOKE>
    </REVOCATIONLIST>
    <SIGNATURE>...</SIGNATURE>
    </XrML>
```


| ![](/security-updates/images/Cc720208.Caution(WS.10).gif)Waarschuwing                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wanneer u in de intrekkingslijst een URL opgeeft, wordt in RMS met SP1 en RMS met SP2 niet langer een UNC-pad ondersteund. U moet een URL gebruiken. |

Als u de REVOKE-elementen hebt gedefinieerd, kan de intrekkingslijst worden ondertekend.

Werken met het REVOKE-element
-----------------------------

In de voorbeeldintrekkingslijst in de sectie Voorbeeld van een intrekkingslijst specificeert elk REVOKE-element een in te trekken principal. De begincodes bevatten categorie- en typekenmerken waarmee wordt opgegeven welke entiteiten worden ingetrokken en op basis van welk criterium deze entiteiten worden ingetrokken. Verschillende REVOKE-elementen hebben verschillende onderliggende elementen, afhankelijk van de actie die is gedefinieerd met de categorie- en typekenmerken.

Zie de volgende voorbeelden voor meer informatie over het opgeven van REVOKE-elementen:

-   [Principals intrekken op basis van een openbare sleutel](#bkmk_1)
-   [Certificaten en licenties intrekken op basis van de GUID](#bkmk_2)
-   [Certificaten en licenties intrekken op basis van de hashwaarde](#bkmk_3)
-   [Certificaten en licenties intrekken op basis van de openbare sleutel van de uitgever](#bkmk_4)
-   [Certificaten en licenties intrekken op basis van de uitgever-id](#bkmk_5)
-   [Inhoud intrekken op basis van de inhouds-id](#bkmk_6)
-   [Principals intrekken op basis van de principal-id](#bkmk_10)
-   [Principals intrekken op basis van de Windows Live-ID](#bkmk_7)

<span id="BKMK_1"></span>

#### Principals intrekken op basis van een openbare sleutel

In dit voorbeeld wordt een principal ingetrokken op basis van de openbare sleutel. De inhoud van de code &lt;PUBLICKEY&gt; is in dit geval afkomstig uit het knooppunt <BODY><ISSUEDPRINCIPALS><PRINCIPAL>&lt;PUBLICKEY&gt; van het certificaat waarmee de sleutel is uitgegeven.

```
   <REVOKE category="principal" type="principal-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
6Jn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```
<span id="BKMK_2"></span>
#### Certificaten en licenties intrekken op basis van de GUID

In dit voorbeeld wordt een certificaat of licentie ingetrokken op basis van de GUID (Globally Unique Identifier). U kunt geen certificaat of licentie met een overeenkomende GUID gebruiken als deze intrekkingslijst wordt gebruikt. De inhoud van de code <ID> is in dat geval afkomstig uit het knooppunt <BODY><DESCRIPTOR><OBJECT><ID> van het certificaat dat of de licentie die u intrekt. U kunt op deze manier ook toepassingen intrekken door de id van het toepassingsmanifest op te geven.

```
<REVOKE category="license" type="license-id">
        <OBJECT>
          <ID type="MS-GUID">{06BCB94D-43E5-419f-B180-AA9FD321ED7A}</ID>
        </OBJECT>
      </REVOKE>
```
#### Intrekken op basis van toepassingsmanifest

Om op toepassingsmanifest in te trekken dient u de gebruikers-id, openbare sleutel van de uitgever, licentie-id of licentie-hash van het toepassingsmanifest uit te pakken. Toepassingsmanifesten zijn echter gecodeerd volgens base-64. Informatie is niet beschikbaar in tekst zonder opmaak. Met de Windows Rights Management Services Software Development Kit (SDK) kunnen programma's worden ontwikkeld volgens de DRMConstructCertificateChain-, DRMDeconstructCertificateChain- en DRMDecode-methoden, die het toepassingsmanifest decoderen en de benodigde informatie opvragen.

Als u wilt voorkomen dat een toepassing bepaalde met rechten beveiligde inhoud gebruikt, kunt u de desbetreffende toepassing uitsluiten zodat de RMS-cluster geen gebruikslicenties aan die toepassing kan verlenen. De beperking van uitsluiting is dat niet kan worden verhinderd dat iemand met een geldige gebruikerslicentie nog steeds met rechten beveiligde inhoud kan decoderen. Zie [Toepassingen uitsluiten](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) eerder in dit onderwerp voor meer informatie over het uitsluiten van toepassingen.

<span id="BKMK_3"></span>
#### Certificaten en licenties intrekken op basis van de hashwaarde

In dit voorbeeld wordt een certificaat of licentie ingetrokken op basis van de hash. De inhoud van de code <VALUE> is in dit geval de SHA-1-hash van de UNICODE-tekens van <BODY> tot </BODY> in het certificaat of de licentie. U vindt deze hashwaarde in het gedeelte <SIGNATURE> van het certificaat of de licentie. U kunt op deze manier ook toepassingen intrekken door de hash van het toepassingsmanifest op te geven.

```
<REVOKE category="license" type="license-hash">
        <DIGEST>
          <ALGORITHM>SHA1</ALGORITHM>
          <VALUE encoding="base64" size="160">
            ABfB4mcEslVCMEZR9reACqXHCoQ=
          </VALUE>
        </DIGEST>
      </REVOKE>
```
#### Intrekken op basis van toepassingsmanifest

Om op toepassingsmanifest in te trekken dient u de gebruikers-id, openbare sleutel van de uitgever, licentie-id of licentie-hash van het toepassingsmanifest uit te pakken. Toepassingsmanifesten zijn echter gecodeerd volgens base-64. Informatie is niet beschikbaar in tekst zonder opmaak. Met de Rights Management Services SDK kunnen programma's worden ontwikkeld volgens de DRMConstructCertificateChain-, DRMDeconstructCertificateChain- en DRMDecode-methoden, die het toepassingsmanifest decoderen en de benodigde informatie opvragen.

Als u wilt voorkomen dat een toepassing bepaalde met rechten beveiligde inhoud ophaalt, kunt u de desbetreffende toepassing uitsluiten zodat de RMS-cluster geen gebruikslicenties aan die toepassing kan verlenen. De beperking van uitsluiting is dat niet kan worden verhinderd dat iemand met een geldige gebruikerslicentie nog steeds door RMS beveiligde inhoud kan decoderen. Zie [Toepassingen uitsluiten](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) eerder in dit onderwerp voor meer informatie over het uitsluiten van toepassingen.

<span id="BKMK_4"></span>
#### Certificaten en licenties intrekken op basis van de openbare sleutel van de uitgever

In dit voorbeeld worden alle certificaten en licenties ingetrokken die zijn uitgegeven door de eigenaar van de opgegeven openbare sleutel. De inhoud van de code &lt;PUBLICKEY&gt; is in dit geval het knooppunt &lt;BODY&gt;&lt;ISSUER&gt;&lt;PUBLICKEY&gt; van de certificaten of licenties die u intrekt.

```
<REVOKE category="license" type="issuer-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
AAn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_5"></span>
#### Certificaten en licenties intrekken op basis van de uitgever-id

In dit voorbeeld wordt een verzameling certificaten of licenties ingetrokken op basis van de id van de uitgever. De inhoud van de code <ID> is in dit geval het knooppunt <BODY>&lt;ISSUER&gt;<OBJECT><ID> van de certificaten of licenties die u intrekt.

```
    <REVOKE category="license" type="issuer-id">
        <OBJECT type="MS-DRM-Server">
          <ID type="MS-GUID">{2BE9E200-3040-41B9-8832-D4D0445EBBD6}</ID> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Zorg ervoor dat u tijdens het opgeven van het ID-type niet op ENTER drukt tussen de GUID (Globally Unique Identifier) en de sluitingscode. Als u dit per ongeluk wel doet, kan de intrekkingslijst niet door de RMS-client worden geparseerd. |

<span id="BKMK_6"></span>
#### Inhoud intrekken op basis van de inhouds-id

In dit voorbeeld wordt inhoud ingetrokken op basis van de inhouds-id. Dit is de beste methode voor het intrekken van inhoud omdat de inhouds-id overeenkomt voor alle gebruikslicenties die zijn gemaakt op basis van een bepaalde uitgiftelicentie. De waarde van het knooppunt <OBJECT> is in dit geval afkomstig uit het knooppunt <BODY><WORK><OBJECT> van een uitgiftelicentie of gebruikslicentie voor de inhoud.

```
<REVOKE category="content" type="content-id">
        <OBJECT type="Microsoft Office Document">
          <ID type="MS-GUID">{8702641D-3512-4AA4-A584-84C703A5B5C0}</ID>
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Zorg ervoor dat u tijdens het opgeven van het ID-type niet op ENTER drukt tussen de GUID (Globally Unique Identifier) en de sluitingscode. Als u dit per ongeluk wel doet, kan de intrekkingslijst niet door de RMS-client worden geparseerd. |

<span id="BKMK_10"></span>
#### Principals intrekken op basis van de Windows-account

In dit voorbeeld wordt een gebruiker of machtigingsprincipal ingetrokken op basis van de Windows-account. De inhoud van het element <OBJECT> is in dit geval afkomstig uit het knooppunt <BODY><ISSUEDPRINCIPALS><PRINCIPAL><OBJECT> van een rechtenaccountcertificaat of gebruikslicentie.

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Windows">{Windows account SID}</ID> 
          <NAME>{E-mail address}</NAME> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Zorg ervoor dat u tijdens het opgeven van het ID-type niet op ENTER drukt tussen de SID van de Windows-account en de sluitingscode. Als u dit per ongeluk wel doet, kan de intrekkingslijst niet door de RMS-client worden geparseerd. |

<span id="BKMK_7"></span>
#### Principals intrekken op basis van de Windows Live-ID
In dit voorbeeld wordt een gebruiker of machtigingsprincipal ingetrokken op basis van de Windows Live-ID. De inhoud van het element <OBJECT> is in dit geval afkomstig uit het knooppunt <BODY><ISSUEDPRINCIPALS><PRINCIPAL><OBJECT> van een rechtenaccountcertificaat of gebruikslicentie.

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Passport">{PUID}</ID> 
          <NAME>michael@contoso.com</NAME> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Zorg ervoor dat u tijdens het opgeven van het ID-type niet op ENTER drukt tussen de PUID (Principal Unique Identifier) en de sluitingscode. Als u dit per ongeluk wel doet, kan de intrekkingslijst niet door de RMS-client worden geparseerd. |

<span id="BKMK_8"></span>
Een handtekening invoegen in een intrekkingslijst
-------------------------------------------------

Wanneer u een intrekkingslijst hebt gemaakt, moet u een handtekening in de intrekkingslijst invoegen zoals in dit onderwerp wordt beschreven. Vervolgens kunt u de intrekkingslijst aan gebruikers beschikbaar stellen via de URL die u opgeeft in de bijbehorende sjabloon voor het rechtenbeleid.

De eerste stap bij het invoegen van een handtekening is het genereren van een sleutelpaar en sleutelbestand voor de intrekkingslijst met het hulpprogramma Strong Name (Sn.exe). Het hulpprogramma Sn.exe is opgenomen in de SDK voor .NET Framework 1.1 en is beschikbaar via de website van Microsoft [http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796).

Het intrekkingslijstbestand kan uitsluitend worden ondertekend met RLsigner.exe wanneer het als Unicode-bestand is opgeslagen.

**Met Sn.exe een nieuw sleutelpaar maken en dat naar een bestand schrijven**
1.  De persoonlijke sleutel maken. Typ de volgende opdracht bij de opdrachtprompt en druk op ENTER:

    **sn -k** *persoonlijke-sleutelbestand***.snk**

    waarbij *persoonlijke-sleutelbestand* de naam is van het sleutelbestand.

2.  Gebruik Sn.exe om de openbare sleutel op te halen uit het sleutelpaarbestand dat bij stap 1 is gemaakt en naar een afzonderlijk bestand te exporteren. Typ de volgende opdracht en druk op ENTER:

    **sn -p** *persoonlijke-sleutelbestand openbare-sleutelbestand*

    waarbij *persoonlijke-sleutelbestand* de naam is van het sleutelbestand en *openbare-sleutelbestand* de naam is van het bestand waarin de geëxporteerde openbare sleutel wordt opgeslagen.

3.  Wijzig de extensie van het bestand met de persoonlijke sleutel (gemaakt bij stap 1) van .snk in .dat zodat het kan worden gebruikt met RLsigner.exe.

4.  Gebruik RLsigner.exe om een handtekening in te voegen in een intrekkingslijstbestand. Dit hulpprogramma wordt meegeleverd met RMS. Standaard is dit programma opgenomen in de map %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking |
|----------------------------------------------------------------------------|
| RLsigner.exe ondersteunt geen bestandsnamen met spaties.                   |

<span id="BKMK_9"></span>
Werken met RLsigner.exe
-----------------------

Als u RLsigner.exe uitvoert, wordt eerst een handtekening gemaakt op basis van de persoonlijke sleutel in het sleutelbestand. Vervolgens wordt er een uitvoerbestand gemaakt dat is gebaseerd op het intrekkingslijstbestand dat u hebt opgegeven.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Belangrijk                                  |
|-------------------------------------------------------------------------------------------------------------------|
| Het intrekkingslijstbestand moet zijn opgeslagen als Unicode-bestand om er met RLsigner.exe mee te kunnen werken. |

Om de intrekkingslijst te ondertekenen met RLsigner.exe, typt u het volgende achter de opdrachtprompt:

**rlsigner.exe***invoerbestand***{-f***sleutelbestand* **| -**h *containernaam***CSP}***uitvoerbestand*

Gebruik de volgende informatie om de invoerparameters voor de opdracht te voltooien:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parameter</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>Invoerbestand</em></td>
<td style="border:1px solid black;">Naam van het met XrML compatibele intrekkingslijstbestand dat u hebt voorbereid.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>sleutelbestand</em></td>
<td style="border:1px solid black;">Naam van het bestand met de openbare en persoonlijke sleutels die u hebt gegenereerd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>containernaam</em></td>
<td style="border:1px solid black;">Naam van de sleutelcontainer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>uitvoerbestand</em></td>
<td style="border:1px solid black;">Naam van het ondertekende intrekkingslijstbestand dat u met het hulpprogramma maakt.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Opmerking |  
|----------------------------------------------------------------------------|  
| RLsigner.exe ondersteunt geen bestandsnamen met spaties.                   |
  
In de volgende voorbeelden wordt beschreven hoe u RLsigner.exe op een opdrachtregel kunt gebruiken met verschillende cryptografieproviders:
  
-   Voorbeeld van de opdrachtregelsyntaxis waarin een sleutelbestand wordt gebruikt:  
    **rlsigner.exe rl.xml -f key.dat output.xml**  
-   Voorbeeld van de opdrachtregelsyntaxis waarin een hardwarebeveiligingsmodule wordt gebruikt:  
    **rlsigner.exe rl.xml -h Container CSP output.xml**
  
De retourcode van RLsigner.exe biedt basisinformatie over eventuele fouten. In de volgende tabel worden de mogelijke retourcodes beschreven.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Retourcode</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Gelukt</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Kan het bronbestand niet lezen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Kan het sleutelbestand niet lezen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Ongeldig sleutelbestand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Ongeldig bronbestand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Kan het uitvoerbestand niet schrijven</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Onbekende fout</td>
</tr>
</tbody>
</table>
  
U kunt de ondertekening van intrekkingslijsten plannen op basis van het vernieuwingsinterval dat u hebt opgegeven voor de server.
  
U kunt het ondertekenen van intrekkingslijsten automatiseren met scripts. In het volgende voorbeeldscript wordt RLSigner.exe aangeroepen met VBScript en worden de resultaten geschreven naar het logboek voor systeemgebeurtenissen.
  
<codesnippet asp="http://msdn2.microsoft.com/asp" language displaylanguage="Visual Basic">const EVT\_SUCCESS = 0 const EVT\_ERROR = 1 const EVT\_WARNING = 2 const EVT\_INFORMATION = 4 const EVT\_AUDIT\_SUCCESS = 8 const EVT\_AUDIT\_FAILURE = 16 Dim WshShell, oExec Set WshShell = CreateObject( "WScript.Shell" ) Set oExec = WshShell.Exec("rlsigner.exe input\_file key\_file output\_file") Do While oExec.Status = 0 WScript.Sleep 100 Loop if WshShell.ExitCode &lt;&gt; 0 Then WshShell.LogEvent EVT\_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """" else WshShell.LogEvent EVT\_SUCCESS, "RLsigner completed successfully" end if  

```VB
const EVT_SUCCESS       = 0
const EVT_ERROR         = 1
const EVT_WARNING       = 2
const EVT_INFORMATION   = 4
const EVT_AUDIT_SUCCESS = 8
const EVT_AUDIT_FAILURE = 16

Dim WshShell, oExec

Set WshShell = CreateObject( "WScript.Shell" )
Set oExec = WshShell.Exec("rlsigner.exe input_file key_file output_file")
Do While oExec.Status = 0
     WScript.Sleep 100
Loop

if WshShell.ExitCode <> 0 Then
    WshShell.LogEvent EVT_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """"
else
    WshShell.LogEvent EVT_SUCCESS, "RLsigner completed successfully"
end if
```
