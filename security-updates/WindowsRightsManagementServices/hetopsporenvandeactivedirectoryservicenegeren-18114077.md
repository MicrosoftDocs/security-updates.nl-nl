---
TOCTitle: 'Het opsporen van de Active Directory-service negeren'
Title: 'Het opsporen van de Active Directory-service negeren'
ms:assetid: '9d97e7fb-5b05-4853-ad7b-6cc82b9729f0'
ms:contentKeyID: 18114077
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747614(v=WS.10)'
---

Het opsporen van de Active Directory-service negeren
====================================================

RMS-services en -clients ontdekken servicelocaties door eerst het lokale register ter doorzoeken. Als bepaalde sleutels in het register geen waarde bevatten, zoeken RMS-services en -clients in Active Directory naar het serviceverbindingspunt (SCP). Dit betekent dat u de standaardinstelling Ontdekken via Active Directory kunt omzeilen als u bepaalde sleutels invult in het server- of clientregister.

| ![](images/Cc747614.note(WS.10).gif)Opmerking                                                                                                                  |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als de RMS-basiscluster zo is geconfigureerd dat het SCP niet wordt gepubliceerd in Active Directory, kunt u deze sleutels gebruiken om de RMS-clients te verwijzen naar de juiste locatie. |

In dit gedeelte worden de registervermeldingen beschreven en worden bijzonderheden gegeven over de manier waarop u die kunt maken.

Service ontdekken omzeilen voor subinschrijvingsservice van een cluster exclusief voor licentieverlening
--------------------------------------------------------------------------------------------------------

Als u een cluster exclusief inricht voor licentieverlening en u wilt die cluster subinschrijven bij een andere basiscluster dan de basiscluster die u hebt ingericht in het Active Directory-forest van die cluster exclusief voor licentieverlening, moet u het ontdekken van zowel de subinschrijvings- als de accountcertificeringsservices omzeilen.

#### Beschrijving registervermeldingen

De volgende registervermeldingen worden gebruikt voor het omzeilen van de services voor subinschrijving en accountcertificering.

-   **SubEnrollmentURL**. Deze vermelding bevat het pad naar de basiscluster die de licentieserver gebruikt bij het aanvragen van het eigen serverlicentieverleningscertificaat.
-   **GicURL**. Deze vermelding bevat het pad naar de accountcertificeringsservice voor deze cluster exclusief voor licentieverlening.

#### Bijzonderheden van de vermeldingen

Op computers waarop de 32-bits versie van Windows Server 2003 wordt uitgevoerd, is het volledige subsleutelpad naar de registervermeldingen voor service ontdekken voor subinschrijving van clusters exclusief voor licentieverlening:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Op computers waarop de 64-bits versie van Windows Server 2003 wordt uitgevoerd, is het volledige subsleutelpad naar de registervermeldingen voor service ontdekken voor subinschrijving van clusters exclusief voor licentieverlening:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

In de onderstaande tabel vindt u de vermeldingen die u kunt toevoegen om service ontdekken te omzeilen.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Naam</th>
<th style="border:1px solid black;" >Type</th>
<th style="border:1px solid black;" >Waarde</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SubEnrollmentURL</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">http(of https)://<em>servernaam</em>/_wmcs/certification/subenrollservice.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GicURL</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">http(of https)://<em>servernaam</em>/_wmcs/certification/certification.asmx</td>
</tr>
</tbody>
</table>
  
Clientzijde service ontdekken omzeilen voor uitgeven  
----------------------------------------------------
  
Als de gebruikers inhoud uitgeven vanaf hun computers, wilt u misschien de locaties omzeilen van de servers die worden gebruikt voor uitgeven, afhankelijk van de in de organisatie gebruikte topologie. De locaties van de servers die worden gebruikt voor uitgeven worden meestal door de client ontdekt door gebruik te maken van Active Directory. Door op de clientcomputers de juiste registersleutels toe te voegen, omzeilen de clients die methoden en gebruiken in plaats daarvan de URL's die u opgeeft als waarden voor de registervermeldingen.
  
| ![](images/Cc747614.note(WS.10).gif)Opmerking                                                                                                                                                            |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| De in deze sectie opgesomde toevoegingen aan het clientregister moeten worden gemaakt als sleutel en niet als afzonderlijke vermeldingen. De waarde van die sleutels moet worden gemaakt in de standaardvermelding voor elke sleutel. |
  
#### Beschrijving registersleutels
  
De volgende registersleutels kunnen worden gebruikt om het automatisch ontdekken van de RMS-cluster te omzeilen.
  
-   **Activation**. Deze registersleutel definieert de URL van de service voor computeractivering. Als u RMS-client met Service Pack 1 of later uitvoert, wordt deze registervermelding niet meer gebruikt.  
-   **EnterprisePublishing**. Deze registersleutel definieert de URL van een RMS-installatie die u deze client wilt laten gebruiken voor licentieaanvragen.  
-   **CloudPublishing**. Deze registersleutel definieert de URL van de door Microsoft gehoste licentieservice die kan worden gebruikt als de client geen toegang heeft tot een RMS-installatie maar wel toegang heeft tot internet.
  
#### Bijzonderheden van de sleutels
  
Het volledige subsleutelpad naar de registervermeldingen voor clientzijde service ontdekken voor uitgeven is:
  
**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\MSDRM\\ServiceLocation\\**
  
In de onderstaande tabel vindt u de registersleutels die u op een RMS-clientcomputer kunt toevoegen om service ontdekken te omzeilen.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Naam</th>
<th style="border:1px solid black;" >Type</th>
<th style="border:1px solid black;" >Waarde</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Activation</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">http(of https)://<em>RMS-clusternaam</em>/_wmcs/Certification waarbij <em>RMS-clusternaam</em> de naam is van de RMS-cluster.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">EnterprisePublishing</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">http(of https)://<em>RMS-clusternaam</em>/_wmcs/Licensing waarbij <em>RMS-clusternaam</em> de naam is van de RMS-cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CloudPublishing</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">http(of https)://<em>FQDN-clusternaam</em>/_wmcs/Licensing waarbij <em>FQDN-clusternaam</em> de FQDN-naam (Fully Qualified Domain Name) is van de RMS-cluster.</td>
</tr>
</tbody>
</table>
  
We raden u aan deze registersleutels te implementeren met Systems Management Server of Groepbeleid om er zeker van te zijn dat alle clients in uw onderneming de juiste servers voor uitgeven gebruiken.
  
| ![](images/Cc747614.Caution(WS.10).gif)Waarschuwing                                                                                           |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Onjuiste bewerking van het register kan uw computer beschadigen. Maak een back-up van waardevolle gegevens op de computer voordat u wijzigingen aanbrengt in het register. |
  
U kunt een voorbeeldregisterbestand (.reg) gebruiken om de juiste registersleutels te importeren op elk van de servers in de RMS-cluster.
  
**De juiste registersleutels importeren op elk van de servers in de RMS-cluster**  
1.  Kopieer het volgende voorbeeldregisterbestand naar Notepad.
  
    `Windows Registry Editor Version 5.00`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation]`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\Activation]`
  
    `@="http://<RMS_cluster_name>/_wmcs/certification"`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\EnterprisePublishing]`
  
    `@="http://<RMS_cluster_name>/_wmcs/licensing"`
  
2.  Vervang &lt;RMS\_cluster\_name&gt; door de naam van de RMS-cluster.
  
3.  Sla het bestand op met de bestandsnaamextensie .reg.
  
4.  Dubbelklik op de naam van het bestand in Windows Verkenner.
  
5.  Als het dialoogvenster **Beheer van gebruikersaccounts** wordt weergegeven, controleer dan of de weergegeven actie is wat u wilt, en klik op **Doorgaan**.. Wanneer een prompt verschijnt waarin u wordt gevraagd of u de informatie wilt toevoegen aan het register, klikt u op **Ja**.
