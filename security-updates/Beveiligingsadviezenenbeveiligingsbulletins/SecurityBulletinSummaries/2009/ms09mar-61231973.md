---
TOCTitle: 'MS09-MAR'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor maart 2009'
ms:assetid: 'ms09-mar'
ms:contentKeyID: 61231973
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms09-mar(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor maart 2009
===================================================================

Gepubliceerd: dinsdag 10 maart 2009 | Bijgewerkt: woensdag 11 maart 2009

**Versie:** 1.1

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor maart 2009.

Met de release van de bulletins voor maart 2009 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 5 maart 2009. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 11 februari 2009 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van maart.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395124) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

Samenvattingen
--------------

<span></span>
In de volgende tabel staat de beveiligingsbulletins voor deze maand op volgorde van prioriteit.

Zie de volgende sectie **Software waarin dit probleem optreedt en Downloadlocaties** voor meer informatie over software die last heeft van een probleem.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bulletin-id</th>
<th style="border:1px solid black;" >Titel bulletin en samenvatting</th>
<th style="border:1px solid black;" >Maximaal prioriteitsniveau en gevolgen van het beveiligingslek</th>
<th style="border:1px solid black;" >Opnieuw opstarten vereist</th>
<th style="border:1px solid black;" >Software waarin het probleem optreedt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-006">MS09-006</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de Windows-kernel kan externe code worden uitgevoerd (958690)</strong><br />
<br />
Met deze beveiligingsupdate worden verschillende privé gemelde beveiligingslekken in de Windows-kernel opgelost. Het ernstigste beveiligingslek kan leiden tot uitvoering van externe code als een gebruiker een speciaal vervaardigd EMF- of WMF-afbeeldingsbestand van een getroffen systeem weergeeft.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-007">MS09-007</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in SChannel is vervalsing (spoofing) mogelijk (960225)</strong><br />
<br />
Deze beveiligingsupdate lost een privé gemeld beveiligingslek in het beveiligingspakket voor veilige kanalen (SChannel) in Windows op. Door dit beveiligingslek is vervalsen (spoofen) mogelijk als een aanvaller toegang weet te krijgen tot het certificaat dat de eindgebruiker gebruikt voor verificatie. Klanten worden uitsluitend getroffen wanneer de aanvaller het openbare-sleutelonderdeel van het certificaat dat voor verificatie wordt gebruikt langs een andere weg heeft verkregen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Spoofing</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-008">MS09-008</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in DNS- en WINS-server maken vervalsing (spoofing) mogelijk (962238)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken en twee openbaar vrijgegeven beveiligingslekken in Windows DNS-server en Windows WINS-server opgelost. Door deze beveiligingslekken kan een externe aanvaller netwerkverkeer dat is bestemd voor systemen op internet omleiden naar de eigen systemen van de aanvaller.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Spoofing</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden vermeld volgens bulletin-id en CVE-id.
  
**Gebruik van deze tabel**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins functionerende exploitatiecode verschijnt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de ernst van het probleem te kunnen vaststellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.
  
| Bulletin-id                                                         | Titel bulletin                                                                           | CVE-id                                                                           | Beoordeling van de exploitatie-index                                                                                 | Belangrijke opmerkingen                                                                                                                                                                                        |  
|---------------------------------------------------------------------|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Door beveiligingslekken in de Windows-kernel kan externe code worden uitgevoerd (958690) | [CVE-2009-0081](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0081) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Uit dit beveiligingslek voortvloeiende denial-of-service-aanvallen zijn waarschijnlijker dan betrouwbare uitvoering van functionele code                                                                       |  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Door beveiligingslekken in de Windows-kernel kan externe code worden uitgevoerd (958690) | [CVE-2009-0082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0082) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Uit dit beveiligingslek voortvloeiende denial-of-service-aanvallen zijn waarschijnlijker dan betrouwbare uitvoering van functionele code                                                                       |  
| [MS09-006](http://technet.microsoft.com/security/bulletin/ms09-006) | Door beveiligingslekken in de Windows-kernel kan externe code worden uitgevoerd (958690) | [CVE-2009-0083](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0083) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Lokale bedreiging bestaat uitsluitend uit consequente denial-of-service-aanvallen of onrechtmatig vrijgeven van informatie, gevolgen die waarschijnlijker zijn dan betrouwbare uitvoering van functionele code |  
| [MS09-007](http://technet.microsoft.com/security/bulletin/ms09-007) | Door een beveiligingslek in SChannel is vervalsing (spoofing) mogelijk (KB960225)        | [CVE-2009-0085](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0085) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | De vereisten voor betrouwbare misbruikmogelijkheden zijn hoog en het aantal beduidende klantscenario's is laag                                                                                                 |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Beveiligingslekken in DNS- en WINS-server maken vervalsing (spoofing) mogelijk (962238)  | [CVE-2009-0093](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0093) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Consequente spoofing-conceptcode is waarschijnlijk, maar functionele exploitatiecode die resulteert in uitvoering van schadelijke code is zeer onwaarschijnlijk                                                |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Beveiligingslekken in DNS- en WINS-server maken vervalsing (spoofing) mogelijk (962238)  | [CVE-2009-0094](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0094) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Consequente spoofing-conceptcode is waarschijnlijk, maar functionele exploitatiecode die resulteert in uitvoering van schadelijke code is zeer onwaarschijnlijk                                                |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Beveiligingslekken in DNS- en WINS-server maken vervalsing (spoofing) mogelijk (962238)  | [CVE-2009-0233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Consequente spoofing-conceptcode is waarschijnlijk, maar functionele exploitatiecode die resulteert in uitvoering van schadelijke code is zeer onwaarschijnlijk                                                |  
| [MS09-008](http://technet.microsoft.com/security/bulletin/ms09-008) | Beveiligingslekken in DNS- en WINS-server maken vervalsing (spoofing) mogelijk (962238)  | [CVE-2009-0234](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0234) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Consequente spoofing-conceptcode is waarschijnlijk, maar functionele exploitatiecode die resulteert in uitvoering van schadelijke code is zeer onwaarschijnlijk                                                |
  
Software waarin het probleem optreedt en Downloadlocaties  
---------------------------------------------------------
  
<span></span>
In de volgende tabellen staan de bulletins volgens belangrijke softwarecategorie en prioriteit.
  
**Gebruik van deze tabellen**
  
In deze tabellen vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of -onderdeel in de tabel controleren of er nieuwe beveiligingsupdates zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.
  
**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.
  
#### Windows-besturingssysteem en -onderdelen

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4">
Microsoft Windows 2000:  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[](http://technet.microsoft.com/security/bulletin/ms09-008)**MS09-008**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=98bb7d40-89a0-470a-8eb7-06f15072a635)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bf7065bc-c183-4a78-8d46-72fe7385c07c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=110354f7-5ece-4c4d-b563-3adba6ac0116)  
(961063)  
(Belangrijk)  
[WINS-server op Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=4319abb3-1ea2-466a-a815-c0b3b86b4462)  
(961064)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[](http://technet.microsoft.com/security/bulletin/ms09-008)**MS09-008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e09641ba-6cbe-4095-82b5-703d3a7dc33b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=942d87f6-3cb1-4d36-a70a-70d9c34488f3)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d0d704c6-48c2-4907-b6c3-2455d7cf21c8)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6d02306e-9e2e-4ae8-bd21-8a2c1a229472)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[](http://technet.microsoft.com/security/bulletin/ms09-008)**MS09-008**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f5cfb8da-e7cc-4183-8631-507c2a406500)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b3f6fdd-276e-4267-99d8-8f00d91ad6a2)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6cc42c9e-c34e-4577-8b23-9e07e2369878)  
(961063)  
(Belangrijk)  
[WINS-server op Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=049e5db5-7315-4188-99fd-4a54833e6bf2)  
(961064)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ecf75c70-8489-41ad-9759-3a07e13957be)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ce98ff55-f565-469d-bbd2-32b681faf908)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1f81fd2-0099-4450-8543-0459561d22d0)  
(961063)  
(Belangrijk)  
[WINS-server op Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a393c63-eff5-4c8c-9c3f-33ce45c32428)  
(961064)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=04be3d7e-7dda-4dca-887a-e7a8156ede1c)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=5ca3c72c-cadb-4b0a-b3a3-fb81d0bfd7b3)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=d3ed7d9a-d652-4bd0-aecc-5a415bec6c59)  
(961063)  
(Belangrijk)  
[WINS-server op Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=37e3a75e-0a5d-4df0-881f-cdb87efa4dcf)  
(961064)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[](http://technet.microsoft.com/security/bulletin/ms09-008)**MS09-008**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista en Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b1aaaba-f355-4265-83c0-50b901856ced)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=21086a04-402a-4940-8358-7fa63508102b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0fcac480-d6db-4a94-8c7d-b7319282cf56)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c75a2ea9-b42f-457b-be09-5c8fa0339388)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://technet.microsoft.com/security/bulletin/ms09-006)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://technet.microsoft.com/security/bulletin/ms09-007)
</td>
<td style="border:1px solid black;">
[](http://technet.microsoft.com/security/bulletin/ms09-008)**MS09-008**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=38851df2-4fb5-4d28-9d15-181c260cf8cf)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=47b361ce-624b-466c-b5c5-8703f6532615)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=92e89882-d656-4b61-a05c-3afb44895f08)\*  
(961063)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=ec15acc4-3e0f-4414-9383-61c122ff1382)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=5c81ac45-60e6-4121-ab6b-d3b3179aacc4)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[DNS-server op Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=be068d06-5939-4ad8-8191-e85931ed610f)\*  
(961063)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=eead6f93-10fd-4492-8137-481d9876a5fe)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=bf8f5a86-1757-4f9b-b632-d4aa7005a9f8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
</table>
 
**Opmerkingen voor Windows Server 2008**

**\*Windows Server 2008 Server Core-installatie is getroffen.** Voor ondersteunde edities van Windows Server 2008 is deze update van toepassing met hetzelfde prioriteitsniveau, ongeacht of Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging voor thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn verkrijgbaar via [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) en [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.

Ten slotte kunt u beveiligingsupdates downloaden uit de [Microsoft Update-catalogus](http://go.microsoft.com/fwlink/?linkid=96155). In de Microsoft Update-catalogus vindt u een doorzoekbare catalogus met inhoud die beschikbaar is gesteld via Windows Update en Microsoft Update, waaronder beveiligingsupdates, stuurprogramma's en service packs. Door tijdens het zoeken het nummer van het beveiligingsbulletin (bijvoorbeeld “MS07-036”) te gebruiken, kunt u alle beschikbare updates toevoegen aan uw winkelmand (waaronder de verschillende talen voor een update) en de map van uw keuze downloaden. Raadpleeg de [veelgestelde vragen van de Microsoft Windows Update-catalogus](http://go.microsoft.com/fwlink/?linkid=97900) voor meer informatie over de Microsoft Windows Update-catalogus.

**Richtlijnen voor detecteren en implementeren**

Microsoft heeft richtlijnen voor detecteren en implementeren uitgebracht voor de beveiligingsupdates van deze maand. Aan de hand van deze richtlijnen kunnen IT-professionals zien hoe zij met diverse middelen, zoals Windows Update, Microsoft Update, Office Update, de Microsoft Baseline Security Analyzer (MBSA), de Office Detection Tool, Microsoft Systems Management Server (SMS) en de Extended Security Update Inventory Tool (ESUIT) de beveiligingsupdate kunnen implementeren. Zie [Microsoft Knowledge Base-artikel 910723](http://support.microsoft.com/kb/910723) voor meer informatie.

**Microsoft Baseline Security Analyzer**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders snel en betrouwbaar de nieuwste essentiële updates en beveiligingsupdates implementeren voor Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar; zie ook [System Center Configuration Manager 2007.](http://technet.microsoft.com/en-us/library/bb735860.aspx) Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren. SMS 2.0-gebruikers kunnen ook het [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) gebruiken voor de implementatie van beveiligingsupdates. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking:** SMS maakt gebruik van de Microsoft Baseline Security Analyzer en de Microsoft Office Detection Tool om brede ondersteuning te kunnen bieden voor het zoeken en uitvoeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows Updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibiliteit Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Microsoft Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:

Voor informatie over andere releases voor Windows Update en Microsoft Update (geen beveiligingsreleases), verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services. Heeft betrekking op alle Windows-inhoud.
-   [Nieuwe, herziene en vrijgegeven updates voor Microsoft-producten behalve Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Microsoft Active Protections Program (MAPP)

Om de beveiliging voor klanten te verbeteren, verstrekt Microsoft bij elke maandelijkse uitgifte van beveiligingsupdates informatie over beveiligingslekken aan de grote producenten van beveiligingsprogramma's. Deze producenten kunnen dan die informatie over beveiligingslekken gebruiken om hun klanten een betere beveiliging te bieden door hun software of apparatuur aan te passen, zoals antivirusprogramma's, inbraakdetectiesystemen voor netwerken of inbraakpreventiesystemen voor hosts. Op de websites van de programmapartners (zie [Microsoft Active Protections Program (MAPP)-partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx)) kunt u nagaan of de leveranciers van beveiligingsprogramma's hun producten steeds aanpassen.

#### Veiligheidsstrategieën en community

**Strategieën voor updatebeheer**

Op de website [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) kunt u extra informatie vinden over aanbevelingen van Microsoft voor het toepassen van beveiligingsupdates.

**Verkrijgen van andere beveiligingsupdates**

Op de volgende locaties zijn updates verkrijgbaar voor andere beveiligingsproblemen:

-   Beveiligingsupdates zijn verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.
-   Updates voor consumentenplatforms zijn verkrijgbaar op de website [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   U kunt de beveiligingsupdates van deze maand die op Windows Update staan, via het ISO CD-imagebestand met beveiligingsupdates en essentiële updates vanaf het Downloadcentrum ophalen. Zie [Microsoft Knowledge Base-artikel 913086](http://support.microsoft.com/kb/913086) voor meer informatie.

**IT Pro Security-community**

Leer de beveiliging te verbeteren en uw IT-infrastructuur te optimaliseren en bespreek beveiligingsonderwerpen met andere IT-professionals op de website [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Dankbetuiging

Microsoft [bedankt](http://go.microsoft.com/fwlink/?linkid=21127) de volgende partijen voor de samenwerking bij het verbeteren van de beveiliging voor klanten:

-   Helmut Buhler ([http://home.arcor.de/clipboarder](http://home.arcor.de/clipboarder/)/) voor het melden van een probleem dat wordt beschreven in MS09-006
-   Thomas Garnier van [SkyRecon](http://www.skyrecon.com/) voor het melden van een probleem dat wordt beschreven in MS09-006
-   [Secretaria da Fazenda do Estado do Rio Grande do Sul](http://www.sefaz.rs.gov.br/) voor het melden van een probleem dat wordt beschreven in MS09-007
-   [Cia de Processamento de Dados do Estado do Rio Grande do Sul](http://www.procergs.rs.gov.br/) voor het melden van een probleem dat wordt beschreven in MS09-007
-   Kevin Day voor de samenwerking met ons bij twee problemen beschreven in MS09-008
-   Dave Dagon van [Georgia Tech Information Security Center](http://www.gtisc.gatech.edu/) voor de samenwerking met ons aan twee problemen die worden beschreven in MS09-008

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (10 maart 2009): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (4 maart 2009): Informatie over de ontdekker bijgewerkt voor MS09-008.

*Built at 2014-04-18T01:50:00Z-07:00*
