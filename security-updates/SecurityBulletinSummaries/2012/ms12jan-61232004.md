---
TOCTitle: 'MS12-JAN'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor januari 2012'
ms:assetid: 'ms12-jan'
ms:contentKeyID: 61232004
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms12-jan(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor januari 2012
=====================================================================

Gepubliceerd: dinsdag 10 januari 2012 | Bijgewerkt: vrijdag 27 januari 2012

**Versie:** 2.1

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor januari 2012.

Met de beveiligingsbulletins voor januari 2012 wordt de vooraankondiging van de bulletins, die oorspronkelijk werd uitgegeven op 5 januari 2012, vervangen. Ga voor meer informatie over de vooraankondiging naar [Vooraankondiging van Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=217213).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 11 januari 2012 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van januari](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499498). Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://go.microsoft.com/fwlink/?linkid=217214) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

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
<th style="border:1px solid black;" >Software waarin dit probleem optreedt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227487">MS12-004</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Windows Media kan externe code worden uitgevoerd (2636391)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Microsoft Windows opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd mediabestand opent. Een aanvaller die misbruik weet te maken van het beveiligingslek, kan dezelfde gebruikersrechten krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235999">MS12-001</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in de Windows-kernel kan een beveiligingsfunctie worden omzeild (2644615)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan een aanvaller de SafeSEH-beveiligingsfunctie in een softwaretoepassing omzeilen. Een aanvaller kan vervolgens misbruik maken van andere beveiligingslekken om de gestructureerde uitzonderingshandler toe te passen en willekeurige code uit te voeren. Alleen softwaretoepassingen die zijn gecompileerd met Microsoft Visual C++ .NET 2003 kunnen worden gebruikt om misbruik te maken van dit beveiligingslek.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Omzeiling van beveiligingsfunctie</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229637">MS12-002</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Windows Object Packager kan externe code worden uitgevoerd (2603381)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een gebruiker een legitiem bestand met een ingesloten object opent dat zich bevindt in dezelfde netwerkmap als een speciaal vervaardigd uitvoerbaar bestand. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235400">MS12-003</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Windows Client/Server Run-time Subsystem kan leiden tot misbruik van bevoegdheden (2646524)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Het prioriteitsniveau van deze beveiligingsupdate is Belangrijk voor alle ondersteunde edities van Windows XP, Windows Server 2003, Windows Vista en Windows Server 2008. Alle ondersteunde edities van Windows 7 en Windows Server 2008 R2 worden niet door het beveiligingslek getroffen.<br />
<br />
Het beveiligingslek kan leiden tot misbruik van bevoegdheden als een aanvaller zich aanmeldt op een getroffen systeem en een speciaal vervaardigde toepassing uitvoert. De aanvaller kan vervolgens volledige controle over het getroffen systeem krijgen en kan programma's installeren; gegevens weergeven, wijzigen of verwijderen; of nieuwe accounts met volledige gebruikersrechten maken. Van dit beveiligingslek kan alleen misbruik worden gemaakt op systemen met een Chinese, Japanse of Koreaanse landinstelling van het systeem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=230777">MS12-005</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Microsoft Windows kan externe code worden uitgevoerd (2584146)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan externe code worden uitgevoerd indien een gebruiker een speciaal vervaardigd Microsoft Office-bestand met een schadelijke ingesloten ClickOnce-toepassing opent. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232510">MS12-006</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in SSL/TLS kan leiden tot het vrijgeven van informatie (2643584)</strong><br />
<br />
Dit beveiligingsupdate lost een openbaar gemeld beveiligingslek in SSL 3.0 en TLS 1.0 op. Dit beveiligingslek treft het protocol zelf en is niet specifiek voor het Windows-besturingssysteem. Door het beveiligingslek kan informatie worden vrijgegeven als een aanvaller gecodeerd webverkeer onderschept dat afkomstig is van een getroffen systeem. TLS 1.1, TLS 1.2 en alle coderingssuites die geen gebruik maken van de CBC-modus, worden niet getroffen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Vrijgeven van informatie</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227561">MS12-007</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in</strong> <strong>AntiXSS-bibliotheek kan leiden tot vrijgeven van informatie (2607664)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in de Microsoft AntiXSS-bibliotheek (Anti-Cross Site Scripting) opgelost. Het beveiligingslek kan leiden tot onrechtmatig vrijgeven van informatie indien een aanvaller een schadelijke scriptcode doorstuurt naar een website met de opschoningsfunctie van de AntiXSS-bibliotheek. De gevolgen van het vrijgeven van die informatie is afhankelijk van de aard van de informatie. Dit beveiligingslek kan er niet toe leiden dat een aanvaller rechtstreeks code uitvoert of zich machtigingen toekent, maar wel dat de aanvaller bruikbare informatie kan genereren waarmee het systeem waarin dit probleem optreedt verder kan worden misbruikt. Alleen websites die de opschoningsmodule van de AntiXSS-bibliotheek gebruiken, worden getroffen door dit beveiligingslek.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Vrijgeven van informatie</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft-programma's en software voor ontwikkelaars</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden vermeld in volgorde van bulletin-id en daarna van CVE-id. Alleen beveiligingslekken met het prioriteitsniveau Kritiek of Belangrijk in de bulletins zijn opgenomen.
  
**Gebruik van deze tabel**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins externe code wordt uitgevoerd en denial of service optreedt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de prioriteit van de implementatie van de updates van deze maand vast te stellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.
  
In de onderstaande kolommen verwijst "Nieuwste softwarerelease" naar de nieuwste release van de software en verwijst "Oudere softwarereleases" naar alle oudere, ondersteunde releases van de software die wordt genoemd in de tabel "Software waarin dit probleem optreedt" of de tabel "Software waarin dit probleem niet optreedt" in het bulletin.
  
| Bulletin-id                                               | Titel van beveiligingslek                                                                              | CVE-id                                                                           | Beoordeling van het risico op misbruik voor de nieuwste softwarerelease                              | Beoordeling van het risico op misbruik voor oudere softwarerelease                                   | Beoordeling van het risico op misbruik door denial of service | Belangrijke opmerkingen                                                                                                  |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|  
| [MS12-001](http://go.microsoft.com/fwlink/?linkid=235999) | Beveiligingslek met betrekking tot omzeiling van SafeSEH in de Windows-kernel                          | [CVE-2012-0001](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0001) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot omzeiling van een beveiligingsfunctie.                                     |  
| [MS12-002](http://go.microsoft.com/fwlink/?linkid=229637) | Beveiligingslek in Object Packager met betrekking tot het onveilig starten van een uitvoerbaar bestand | [CVE-2012-0009](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0009) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                                                                                                                   |  
| [MS12-003](http://go.microsoft.com/fwlink/?linkid=235400) | Beveiligingslek in CSRSS met betrekking tot misbruik van bevoegdheden                                  | [CVE-2012-0005](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0005) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                   |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Beveiligingslek in MIDI met betrekking tot het uitvoeren van externe code                              | [CVE-2012-0003](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0003) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                                                                                                                   |  
| [MS12-004](http://go.microsoft.com/fwlink/?linkid=227487) | Beveiligingslek met betrekking tot de uitvoering van externe code in DirectShow                        | [CVE-2012-0004](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0004) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                                                                                                                   |  
| [MS12-005](http://go.microsoft.com/fwlink/?linkid=230777) | Beveiligingslek met betrekking tot het uitvoeren van assembly's                                        | [CVE-2012-0013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0013) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                                                                                                                   |  
| [MS12-006](http://go.microsoft.com/fwlink/?linkid=232510) | Beveiligingslek in SSL- en TLS-protocollen                                                             | [CVE-2011-3389](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3389) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie dat openbaar is gemaakt met beperkte details. |  
| [MS12-007](http://go.microsoft.com/fwlink/?linkid=227561) | Beveiligingslek met betrekking tot omzeiling van de AntiXSS-bibliotheek                                | [CVE-2012-0007](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0007) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie.                                              |
  
Software waarin het probleem optreedt en Downloadlocaties  
---------------------------------------------------------
  
<span></span>
In de volgende tabellen staan de bulletins volgens belangrijke softwarecategorie en prioriteit.
  
**Gebruik van deze tabellen**
  
In deze tabellen vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of -onderdeel in de tabel controleren of er nieuwe beveiligingsupdates zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.
  
**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.
  
#### Windows-besturingssysteem en -onderdelen

 
<table style="border:1px solid black;">
<tr>
<th colspan="7">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=a142f7ba-4268-4453-a8eb-470213c028ac)  
(KB2598479)  
(Kritiek)  
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=89b23d72-410f-4133-9c14-24eb01e5a732)  
(KB2628259)  
(Alleen Windows XP Media Center Edition 2005 Service Pack 3)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4b168ee8-eb15-4c2c-afb0-e63d62b4a6dc)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=feaeda8c-84ee-47be-8c68-736f0e5b1fc7)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfc38dc2-c4c7-4a44-8e5a-b98bb9bc0396)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bcb1d1e-9261-4a36-9256-90d3df9bd4fb)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fb0360b1-254c-4ecb-a36a-807cabfec1ab)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=0928d720-ae88-40d6-b76f-636d67da8526)  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13d74cc6-8d8e-45ea-8cdc-c15782f6626b)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46386269-6e37-4710-bfef-cedfe60d881c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=211827f2-fe6a-4e16-a90c-0cc3b60a722d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3956db98-88d9-49fc-be51-247b40bfc272)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c687796-4c41-4d17-b738-511d2fbfc126)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=afe6b34d-21b1-4dfa-afa6-2c5c2a678e9e)  
(KB2585542)  
(Belangrijk)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=986f1156-0190-48c2-9f39-29cacb91f0f9)  
(KB2638806)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-** **id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**P** **rioriteitsniveau**
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
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=3c266dfb-630d-4f32-b2ca-63955279b6a9)  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=89ae6ed0-537f-421c-b755-ef28691abd88)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9cdfc0fe-8f43-4e13-8a1f-2b48ff9ff472)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8e46267-7988-4fbe-ae94-68b6fdb2e7d9)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=39f5f8fb-ee4d-4b7a-9cd7-3d1e9c8abd8c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c39be84-1eab-4794-b3ed-e529643aca21)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e2c503a5-3f15-4a77-9a05-9ea0fbaf4503)  
(KB2585542)  
(Belangrijk)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c23e7604-d489-4836-8b54-3b2b3d6a365c)  
(KB2638806)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=8dd1c882-4ed1-4e47-a017-7d162bd94194)  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=08be569c-e9d1-4fc5-8670-ebe9da0a2072)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e5783aa-6847-404c-9b75-621fa14ebbb8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5975b01e-139b-4b9d-a0d5-a87a279bfea1)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e27d85f8-a285-4e95-85a0-0868286cc2b9)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3cf29dfd-239e-4707-92e6-952133c1c1c2)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ad34496-40af-40cb-9f85-5d3c31543211)  
(KB2585542)  
(Belangrijk)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2f36e991-4e1a-4b8c-8cfb-e7f20d97cf0b)  
(KB2638806)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=3a9b09d6-7060-47ab-9f76-c3c5acb024e6)  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=3401ac20-3701-471f-9757-097a9402d761)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=cdf8208c-d55b-428f-bdd3-26e291dfb08d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=26079c35-4b96-42fc-ad47-138be25a6bf0)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b69bd01d-9925-4ff1-bfeb-b4473631578c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=623c1c7d-6902-4876-9614-1b6e1ef80831)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=56deb935-9226-49f8-b705-edb3d662d8aa)  
(KB2585542)  
(Belangrijk)  
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=2d72cf5a-cca7-4341-b862-017e3f34a3c9)  
(KB2638806)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=99d9b9fc-ed37-4a32-a20d-6604a1b9c4ca)  
(KB2598479)  
(Kritiek)  
[Windows Media Center TV Pack voor Windows Vista (32-bits edities)](http://www.microsoft.com/downloads/details.aspx?familyid=f345e093-336d-4464-b7f8-a14398b62ebf)<sup>[1]</sup>
(KB2628642)  
(Belangrijk)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=4818059a-52ad-4c2e-9605-4e0f5d9da5ba)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=44eeb0a2-ae17-4971-8a7e-e25b260c582c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73682d4b-3179-4488-8ba9-94ed68c4896b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=038970b6-aeec-4e18-8dfe-887b260a7c87)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9269bd6-8c4f-476e-8481-fc0de52a22e6)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=44aa8d91-2b30-4191-8965-8aee2b860d50)  
(KB2598479)  
(Kritiek)  
[Windows Media Center TV Pack voor Windows Vista (64-bit-edities)](http://www.microsoft.com/downloads/details.aspx?familyid=559d028f-9810-4c50-b65d-f567cbb15427)<sup>[1]</sup>
(KB2628642)  
(Belangrijk)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=13cc2519-860d-4c64-b7f8-8f9c0bdaefcf)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79ceba86-59a1-4138-a5de-8df20ad81b02)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b5c33025-13d9-43d2-a415-a8a4d683a821)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23abeb12-f2fe-43fd-9c4a-4d3d244832f8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0403c753-d4fa-4e3d-a61b-7f816f5c352b)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
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
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=787e6285-3ba5-4aae-9d8d-e3c1eca3b35d)\*  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=92df13c1-fdf6-4602-acb2-e634a1bcd9da)\*\*  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ab87c6c-5802-4454-bce4-12501e5b816d)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf119cf-a8ed-4266-a673-442149992f7c)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d089d9cb-382c-4e64-94c5-69b9864010b1)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2fe2f398-433f-4338-a273-813185b43ea8)\*  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=9eff12b2-70a4-452b-b6bc-0d83f2edcf6c)\*  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=7ff10d7f-26a6-403a-a4b7-7aff55e2fa16)\*\*  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=726ff17e-ac90-4832-91e7-46f71ad2f868)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8e68f89-27f4-4142-94ca-58f086a98157)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ac8a368-4298-4c1d-9cfd-924d6df563af)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f54ac30d-8e41-4df9-bd43-db6742a24d4c)\*  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Multimedia Library](http://www.microsoft.com/downloads/details.aspx?familyid=4e2edb23-7f4e-4fe4-848c-1d744e0dce9f)  
(KB2598479)  
(Kritiek)  
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=5e0394c9-3de4-46f6-ae7f-18d5a555532e)  
(KB2631813)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ba2c3d57-1bdd-44f2-9233-86c7ea6f0ddb)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc6491e8-6c3e-43a1-bc56-16c9a2fd2749)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e08b242-2516-4cf6-b38e-35ec2b8b788d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3979db3b-4961-4df8-84a4-1f26672b127c)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
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
Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d736daf8-db6d-485f-b0cb-7f2d8c86f9a2)  
(KB2631813)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0ee22036-b7f4-40f5-8f40-a77e8faf48b2)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7422605b-7a02-4161-b7f8-92b3ccffef64)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0f433f2c-c61d-461d-af9c-0145af4b72ab)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=21b37775-3e7b-462d-8234-7c47d52daef9)  
(KB2631813)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7444e20c-9821-4c91-9779-2728c537dd6a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4ba46bc7-af7a-445a-84f2-b0c13674409b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0839fec0-b6a7-4e47-9da3-2caef44a7df4)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-004**](http://go.microsoft.com/fwlink/?linkid=227487)
</td>
<td style="border:1px solid black;">
[**MS12-001**](http://go.microsoft.com/fwlink/?linkid=235999)
</td>
<td style="border:1px solid black;">
[**MS12-002**](http://go.microsoft.com/fwlink/?linkid=229637)
</td>
<td style="border:1px solid black;">
[**MS12-003**](http://go.microsoft.com/fwlink/?linkid=235400)
</td>
<td style="border:1px solid black;">
[**MS12-005**](http://go.microsoft.com/fwlink/?linkid=230777)
</td>
<td style="border:1px solid black;">
[**MS12-006**](http://go.microsoft.com/fwlink/?linkid=232510)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
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
Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=355c980d-ec2e-4b2d-a7d4-2e3dbd3a0dde)\*\*  
(KB2631813)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4c73a16d-e9fa-48de-9dca-a6360ce3d029)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=db3a4814-a409-4def-944d-4eaa540b83b0)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34542a5a-88df-4a07-b1ed-d4c845502cd8)\*  
(KB2585542)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[DirectShow](http://www.microsoft.com/downloads/details.aspx?familyid=d4b2389e-fd9f-47c7-9afd-4077f5632c21)  
(KB2631813)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1cc14ee8-f035-4bfc-bf38-33c6b9a2e776)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2101663a-ed3d-4850-b79a-16960ab56b45)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe661936-06e1-45d3-89f6-1093504496a7)  
(KB2585542)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerkingen voor Windows Server 2008 en Windows Server 2008 R2**

**\*Treedt op bij Server Core-installatie.** Deze update is met hetzelfde prioriteitsniveau van toepassing op ondersteunde edities van Windows Server 2008 en Windows Server 2008 R2, zoals is aangegeven, ongeacht of deze zijn geïnstalleerd met de optie Server Core-installatie. Zie de TechNet-artikelen [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) en [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Server Core-installatie niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de TechNet-artikelen [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) en [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Opmerking bij MS12-004**

<sup>[1]</sup>Windows Media Center TV Pack voor Windows Vista is alleen verkrijgbaar op OEM-installaties (Original Equipment Manufacturer) van de Home Premium- en Ultimate-edities van Windows Vista als een optioneel onderdeel. Klanten die dit optionele onderdeel hebben geïnstalleerd, moeten alle updates installeren die beschikbaar zijn voor hun editie van Windows Vista. Microsoft raadt u aan de toepasbare updates voor het besturingssysteem (KB2598479 en KB2631813) te installeren voordat u de update voor Windows Media Center TV Pack (KB2628642) installeert.

#### Microsoft-programma's en software voor ontwikkelaars

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Anti-Cross Site Scripting Library
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-007**](http://go.microsoft.com/fwlink/?linkid=227561)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Anti-Cross Site Scripting Library V3.x en Microsoft Anti-Cross Site Scripting Library V4.0
</td>
<td style="border:1px solid black;">
[Microsoft Anti-Cross Site Scripting Library V3.x en Microsoft Anti-Cross Site Scripting Library V4.0](http://www.microsoft.com/downloads/details.aspx?familyid=b3ef05ce-70fe-4f25-9aee-cb7a42a53d11)<sup>[1]</sup><sup>[2]</sup>
</td>
</tr>
</table>
 
**Opmerking bij MS12-007**

<sup>[1]</sup>Deze download werkt Microsoft AntiXSS-bibliotheek (Anti-Cross Site Scripting) bij naar een nieuwere versie van de AntiXSS-bibliotheek die niet door het beveiligingslek wordt getroffen.

<sup>[2]</sup>Deze update is alleen verkrijgbaar via het Microsoft Downloadcentrum.

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging voor thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn beschikbaar op [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) en [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.

Gebruikers van Microsoft Office voor Mac kunnen Microsoft AutoUpdate voor Mac gebruiken om hun Microsoft-software up-to-date te houden. Raadpleeg [Automatisch op software-updates controleren](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea) voor meer informatie over het gebruik van Microsoft AutoUpdate voor Mac.

Ten slotte kunt u beveiligingsupdates downloaden uit de [Microsoft Update-catalogus](http://go.microsoft.com/fwlink/?linkid=96155). In de Microsoft Update-catalogus vindt u een doorzoekbare catalogus met inhoud die beschikbaar is gesteld via Windows Update en Microsoft Update, waaronder beveiligingsupdates, stuurprogramma's en service packs. Door tijdens het zoeken het nummer van het beveiligingsbulletin (bijvoorbeeld “MS07-036”) te gebruiken, kunt u alle beschikbare updates toevoegen aan uw winkelmand (waaronder de verschillende talen voor een update) en de map van uw keuze downloaden. Raadpleeg de veelgestelde vragen van de [Microsoft Windows Update-catalogus](http://go.microsoft.com/fwlink/?linkid=97900) voor meer informatie over de Microsoft Windows Update-catalogus.

**Richtlijnen voor detecteren en implementeren:**

Microsoft biedt zoekfuncties en richtlijnen voor het implementeren van beveiligingsupdates. Deze begeleiding bevat aanbevelingen en informatie die IT-professionals kunnen helpen verschillende hulpprogramma's voor het zoeken naar en toepassen van beveiligingsupdates te gebruiken. Zie [Microsoft Knowledge Base-artikel 961747](http://support.microsoft.com/kb/961747) voor meer informatie.

**Microsoft Baseline Security Analyzer**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders de nieuwste essentiële updates en beveiligingsupdates snel en betrouwbaar implementeren voor Microsoft Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 voor Microsoft Windows-besturingssysteem Windows 2000 en later.

Ga naar de website [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**System Center Configuration Manager 2007**

Configuration Manager 2007 Software-updates beheren vereenvoudigt de complexe taak van het verspreiden en beheren van updates aan IT-systemen binnen een onderneming. Met Configuration Manager 2007 kunnen IT-beheerders updates van Microsoft-producten verspreiden over diverse apparaten, waaronder pc's, laptops, servers en mobiele apparaten.

De geautomatiseerde beveiligingslekbeoordeling in Configuration Manager 2007 bepaalt of updates nodig zijn en rapporteert over aanbevolen acties. Software-updates beheren van Configuration Manager 2007 is ingebouwd in Microsoft Windows Software Update Services (WSUS), een langdurig geteste update-infrastructuur die vertrouwd is voor IT-beheerders over de gehele wereld. Zie [Software-updates beheren](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx) voor meer informatie over hoe beheerders Configuration Manager 2007 kunnen gebruiken om updates te implementeren. Ga naar [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx) voor meer informatie over Configuration Manager.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers.

**Opmerking** De algemene ondersteuning van System Management Server 2003 is beëindigd met ingang van 12 januari 2010. Voor meer informatie over productlevenscycli gaat u naar [Microsoft Support Lifecycle](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar. Zie **System Center Configuration Manager 2007**.

Voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren, gaat u naar [Scenario's en procedures voor Microsoft Systems Management Server 2003: Softwaredistributie en patchbeheer](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Voor informatie over SMS gaat u naar het [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Opmerking** SMS maakt gebruik van de Microsoft Baseline Security Analyzer om brede ondersteuning te kunnen bieden voor het zoeken en installeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)) gebruiken.

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows-updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Microsoft Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Niet-beveiligingsupdates op MU, WU en WSUS:

Voor informatie over andere releases voor Windows Update en Microsoft Update (geen beveiligingsreleases), verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services. Heeft betrekking op alle Windows-inhoud.
-   [Updates van vorige maanden voor Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Toont alle nieuwe, herziene en opnieuw uitgebrachte updates voor alle Microsoft-producten behalve Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Om de beveiliging voor klanten te verbeteren, verstrekt Microsoft bij elke maandelijkse uitgifte van beveiligingsupdates informatie over beveiligingslekken aan de grote producenten van beveiligingsprogramma's. Deze producenten kunnen dan die informatie over beveiligingslekken gebruiken om hun klanten een betere beveiliging te bieden door hun software of apparatuur aan te passen, zoals antivirusprogramma's, inbraakdetectiesystemen voor netwerken of inbraakpreventiesystemen voor hosts. Op de websites van de programmapartners (zie [Microsoft Active Protections Program (MAPP)-partners](http://go.microsoft.com/fwlink/?linkid=215201)) kunt u nagaan of de leveranciers van beveiligingsprogramma's hun producten steeds aanpassen.

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

-   Joshua J. Drake van [Accuvant LABS](http://www.accuvant.com/) voor het melden van een probleem dat wordt beschreven in MS12-001
-   Parvez Anwar, in samenwerking met [Secunia Research](http://secunia.com/), voor het melden van een probleem dat wordt beschreven in MS12-002
-   Kang Wu van [Shenzhen Jowto Research Dep](http://www.jowto.com) voor het melden van een probleem dat wordt beschreven in MS12-003
-   Shane Garrett van [IBM Security System's X-Force Research](http://xforce.iss.net/) voor het melden van een probleem dat wordt beschreven in MS12-004
-   Neel Mehta van [Google Inc.](http://www.google.com/) voor het melden van een probleem dat wordt beschreven in MS12-004
-   Yorick Koster in samenwerking met het [Beyond Security's SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html)-programma voor het melden van een probleem dat wordt beschreven in MS12-005
-   Adi Cohen van [IBM Rational Application Security](http://blog.watchfire.com/) voor het melden van een probleem dat wordt beschreven in MS12-007

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (10 januari 2012): Samenvatting van de gepubliceerde bulletins.
-   V2.0 (11 januari 2012): In MS12-003 is de exploitatie-index voor de nieuwste softwarerelease gecorrigeerd in de **Exploitatie-index** voor CVE-2012-0005. MS12-007 is herzien om de heruitgave van het bulletin aan te kondigen. Zie het bulletin MS12-007 voor meer informatie.
-   V2.1 (27 januari 2012): In MS12-004 is het prioriteitsniveau gecorrigeerd voor het updatepakket KB2631813 voor alle ondersteunde edities van Windows XP, Windows Server 2003, Windows Vista en Windows Server 2008. Zie het bulletin MS12-004 voor details.

*Built at 2014-04-18T01:50:00Z-07:00*
