---
TOCTitle: 'MS12-JUN'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor juni 2012'
ms:assetid: 'ms12-jun'
ms:contentKeyID: 61232005
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms12-jun(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor juni 2012
==================================================================

Gepubliceerd: dinsdag 12 juni 2012

**Versie:** 1.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor juni 2012.

Met de beveiligingsbulletins voor juni 2012 wordt de vooraankondiging van de bulletins, die oorspronkelijk werd uitgegeven op 7 juni 2012, vervangen. Ga voor meer informatie over de vooraankondiging naar [Vooraankondiging van Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=217213).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 13 juni 2012 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van juni.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499671) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://go.microsoft.com/fwlink/?linkid=217214) voor meer informatie.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246927"><strong>MS12-036</strong></a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Remote Desktop kan externe code worden uitgevoerd (2685939)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Remote Desktop Protocol opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een aanvaller een reeks speciaal vervaardigde RDP-pakketten naar een getroffen systeem verzendt. Standaard is Remote Desktop Protocol (RDP) niet ingeschakeld op een Windows-besturingssysteem. Systemen waarop RDP niet is ingeschakeld, lopen geen risico.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=249045"><strong>MS12-037</strong></a></td>
<td style="border:1px solid black;"><strong>Cumulatieve beveiligingsupdate voor Internet Explorer (2699988)</strong><br />
<br />
Met deze beveiligingsupdate worden één openbaar gemaakt beveiligingslek en twaalf privé gemelde beveiligingslekken in Internet Explorer opgelost. Door de ernstigste beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina weergeeft in Internet Explorer. Een aanvaller die erin slaagt misbruik te maken van een van deze beveiligingslekken, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251095"><strong>MS12-038</strong></a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in .NET Framework kan externe code worden uitgevoerd (2706726)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft .NET Framework opgelost. Door het beveiligingslek kan externe code worden uitgevoerd op een clientsysteem als een gebruiker een speciaal vervaardigde webpagina bekijkt met een webbrowser die XAML-browsertoepassingen (XBAPs) kan uitvoeren. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. Het beveiligingslek zou ook door Windows .NET-toepassingen kunnen worden gebruikt om CAS-beperkingen (Code Access Security) te omzeilen. In het geval van een aanval vanaf het web zou de aanvaller kunnen beschikken over een website waarop zich een webpagina bevindt waarmee dit beveiligingslek wordt misbruikt. Daarnaast kunnen ook gemanipuleerde websites en websites waarop gegevens of advertenties staan of gegevens of advertenties kunnen worden ingevoerd, schadelijke inhoud bevatten die dit beveiligingslek kunnen misbruiken. Een aanvaller kan echter een gebruiker er niet toe dwingen om naar deze websites te gaan. De aanvaller moet een gebruiker er dus van overtuigen een bezoek te brengen aan de website. In de meeste gevallen doet de aanvaller dat door de gebruiker ertoe te bewegen op een koppeling in een e-mailbericht of een verzoek in een expresbericht te klikken waarmee de gebruiker naar de website van de aanvaller gaat.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=252488"><strong>MS12-039</strong></a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in</strong> <strong>Lync</strong> <strong>kunnen leiden tot uitvoering van externe code (2707956)</strong><br />
<br />
Met deze beveiligingsupdate worden één openbaar gemaakt beveiligingslek en drie privé gemelde beveiligingslekken in Microsoft Lync opgelost. Als gevolg van de ernstigste van deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker gedeelde content bekijkt die speciaal vervaardigde TrueType-lettertypen bevat.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Lync</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251612"><strong>MS12-040</strong></a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Microsoft Dynamics AX Enterprise Portal kan leiden tot misbruik van bevoegdheden (2709100)</strong><br />
<br />
Deze beveiligingsupdate lost één privé gemeld beveiligingslek in Microsoft Dynamics AX Enterprise Portal op. Het beveiligingslek kan leiden tot misbruik van bevoegdheden als een gebruiker op een speciaal vervaardigde URL klikt of een speciaal vervaardigde website bezoekt. In het geval van een aanval via e-mail kan een aanvaller misbruik maken van het beveiligingslek door een e-mailbericht met de speciaal vervaardigde URL te verzenden naar de gebruiker van de Microsoft Dynamics AX Enterprise Portal-website waarop de aanval is gericht en door de gebruiker vervolgens over te halen op de speciaal vervaardigde URL te klikken. Gebruikers van Internet Explorer 8 en Internet Explorer 9 die naar een Microsoft Dynamics AX Enterprise Portal-website in de zone Internet bladeren lopen minder risico. Standaard wordt deze aanval in de zone Internet voorkomen door het XSS-filter in Internet Explorer 8 en Internet Explorer 9. Het XSS-filter in Internet Explorer 8 en Internet Explorer 9 is echter niet standaard in de zone Lokaal intranet ingeschakeld.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Dynamics AX</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251707"><strong>MS12-041</strong></a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in de Windows-stuurprogramma's voor de kernelmodus kunnen leiden tot misbruik van bevoegdheden (2709162)</strong><br />
<br />
Met deze beveiligingsupdate worden vijf privé gemelde beveiligingslekken in Microsoft Windows opgelost. De beveiligingslekken kunnen leiden tot misbruik van bevoegdheden als een aanvaller zich aanmeldt op een systeem en een speciaal vervaardigde toepassing uitvoert. Om misbruik te kunnen maken van deze beveiligingslekken, moet een aanvaller geldige aanmeldingsreferenties hebben en zich lokaal kunnen aanmelden.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=252515"><strong>MS12-042</strong></a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (2711167)</strong><br />
<br />
Met deze beveiligingsupdate worden een privé gemeld beveiligingslek en een openbaar gemeld beveiligingslek in Microsoft Windows opgelost. De beveiligingslekken kunnen leiden tot misbruik van bevoegdheden als een aanvaller zich aanmeldt op een getroffen systeem en een toepassing uitvoert die speciaal is vervaardigd om misbruik te maken van het beveiligingslek. Een aanvaller moet geldige aanmeldingsreferenties hebben en zich lokaal kunnen aanmelden om het beveiligingslek te kunnen misbruiken. Het beveiligingslek kan niet vanaf een externe locatie of door anonieme gebruikers worden misbruikt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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
  
| Bulletin-id                                                   | Titel van beveiligingslek                                                                        | CVE-id                                                                           | Beoordeling van het risico op misbruik voor de nieuwste softwarerelease                              | Beoordeling van het risico op misbruik voor oudere softwarerelease                                   | Beoordeling van het risico op misbruik door denial of service | Belangrijke opmerkingen                                                                                                                                                |  
|---------------------------------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927) | Beveiligingslek in Remote Desktop Protocol                                                       | [CVE-2012-0173](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0173) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot het uitvoeren van externe code in centrale elementen          | [CVE-2012-1523](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1523) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot het opschonen van HTML                                        | [CVE-2012-1858](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1858) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie. [MS12-039](http://go.microsoft.com/fwlink/?linkid=252488) lost ook dit beveiligingslek op. |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot het vrijgeven van informatie door null-bytes                  | [CVE-2012-1873](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1873) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie.                                                                                            |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot uitvoering van externe code in de werkbalk voor ontwikkelaars | [CVE-2012-1874](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1874) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot het uitvoeren van externe code in dezelfde ID                 | [CVE-2012-1875](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1875) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | Microsoft is op de hoogte van beperkte aanvallen waarbij wordt geprobeerd het beveiligingslek te misbruiken.                                                           |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot uitvoering van externe code in COL-elementen                  | [CVE-2012-1876](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1876) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek met betrekking tot uitvoering van externe code in titelelementen                 | [CVE-2012-1877](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1877) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek in OnBeforeDeactivate met betrekking tot het uitvoeren van externe code          | [CVE-2012-1878](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1878) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek in insertAdjacentText met betrekking tot het uitvoeren van externe code          | [CVE-2012-1879](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1879) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek in insertRow met betrekking tot het uitvoeren van externe code                   | [CVE-2012-1880](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1880) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Beveiligingslek in OnRowsInserted met betrekking tot het uitvoeren van externe code              | [CVE-2012-1881](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1881) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Tijdelijk                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095) | Beveiligingslek met betrekking tot geheugentoegang in .NET Framework                             | [CVE-2012-1855](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1855) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                                                                                                                                                                 |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | Beveiligingslek met betrekking tot het parseren van TrueType-lettertypen                         | [CVE-2011-3402](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3402) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                                                                  | Permanent                                                     | Dit beveiligingslek is openbaar gemaakt.                                                                                                                               |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | Beveiligingslek met betrekking tot het parseren van TrueType-lettertypen                         | [CVE-2012-0159](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0159) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                                                                  | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | Beveiligingslek in Lync met betrekking tot onveilig laden van bibliotheken                       | [CVE-2012-1849](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1849) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                                                                  | Niet van toepassing                                           | (Geen)                                                                                                                                                                 |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | Beveiligingslek met betrekking tot het opschonen van HTML                                        | [CVE-2012-1858](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1858) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is onwaarschijnlijk | Niet van toepassing                                           | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie. [MS12-037](http://go.microsoft.com/fwlink/?linkid=249045) lost ook dit beveiligingslek op. |  
| [**MS12-040**](http://go.microsoft.com/fwlink/?linkid=251612) | Beveiligingslek met betrekking tot XSS in Dynamics AX Enterprise Portal                          | [CVE-2012-1857](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1857) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                                                                  | Niet van toepassing                                           | (Geen)                                                                                                                                                                 |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Beveiligingslek met betrekking tot afhandeling van string atom-klassenaam                        | [CVE-2012-1864](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1864) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Beveiligingslek met betrekking tot afhandeling van string atom-klassenaam                        | [CVE-2012-1865](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1865) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Beveiligingslek met betrekking tot afhandeling van atom-naam in klembordindeling                 | [CVE-2012-1866](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1866) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Beveiligingslek met betrekking tot integeroverloop in Font Resource Refcount                     | [CVE-2012-1867](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1867) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Beveiligingslek met betrekking tot race condition in Win32k.sys                                  | [CVE-2012-1868](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1868) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515) | Beveiligingslek met betrekking tot ontregeld geheugen in User Mode Scheduler                     | [CVE-2012-0217](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0217) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Niet van toepassing                                                                                  | Permanent                                                     | (Geen)                                                                                                                                                                 |  
| [**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515) | Beveiligingslek met betrekking tot ontregeld BIOS ROM                                            | [CVE-2012-1515](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1515) | Niet van toepassing                                                                                  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Exploitatiecode is waarschijnlijk   | Permanent                                                     | Dit beveiligingslek is openbaar gemaakt.                                                                                                                               |
  
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
<th colspan="6">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fd2216eb-283b-4a23-b259-018a7fa5fe47)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=7f222e05-2a8d-4099-851f-2044811f7425)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=07c75ac6-f92a-4204-aa58-bdf8c033df9e)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5bc1656f-cf1d-4f77-a078-a8602401b8e1)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a399bd47-ffe1-4476-932c-9c119496222a)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0efff733-4c8d-4fce-8de3-28465c6b762b)  
(KB2707511)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e354955-32ae-447c-b16f-960acc01773b)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=57e8bf9d-97c3-4166-a5d4-6b0c99afc6a1)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b35e90b-145d-44c2-a8bc-4f9108d46fa1)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0a386b16-74f7-4d36-93d0-75e7da9bf9b5)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bdb356db-bd36-4159-8e64-ecdb3dfc61bf)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e856fec-9f05-49b7-91b6-11c2636a2f1d)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b1dcc826-7e96-464b-830e-39946e7802aa)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=de828031-1ace-43df-80f2-db7d503fb0a2)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4e6e5589-b767-4e8a-b8b3-df7b97e002e5)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0b39b00-d7db-4008-8310-1258e84a72a2)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=855611a1-91ad-4d22-8c1c-fdcd6af4cef0)  
(KB2707511)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b63fa4d-b42e-43ca-9f2c-cf60c37731a5)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b060e03b-e63e-446b-9cfd-ea4e1e9383a6)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a36f7ffe-d537-4f9e-b676-22a24f50c089)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b1acb2f0-63ba-4524-94cf-42b3534e21e7)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ed7359ce-13e8-42b2-956d-e8be534583aa)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=7dfdc5dc-54b0-49e3-bf5a-bbc40b0f159f)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=893667c4-ef9f-48d3-ab18-a0df51bd3dcc)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=30a9d518-8067-44f4-90fd-09fec8a0c883)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=2317c8d9-cae8-497b-952e-78eb4a6d585c)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="6">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f55b62bf-0571-4888-9061-3f7cc75d7f17)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=16f4404e-e6d6-4bde-af15-3bb692412213)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=610e753a-21db-43e6-bc42-3e1227fa4bb1)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=828fdb71-747b-481d-9683-895325331478)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9188f1eb-b568-4a99-9b39-745c760a693d)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab06290c-4f57-4349-8abd-a382b9044631)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=993c5bc4-8903-4c8c-bbc9-da2e47d959f9)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=87100a7e-7feb-4a18-b7aa-04fdd2d6ef52)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7b551d67-e0f1-498a-ac4f-06376a0fcf18)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b94ae42-2882-444c-ad5e-74e34b805006)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8dcb487-0df7-46f4-8726-bd58e2722812)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e7f9ad40-d515-4224-90ff-4bd4bff9180f)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c4eaeff8-7b7a-4418-a479-09b2146df2bf)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=a20c839c-ce3b-46a5-becb-588de404878d)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6398a156-9618-4ca4-95bc-d36ecacf0745)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40c16540-7839-412c-b474-892292a96fa5)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7420c9f3-8f7e-4823-aaba-b14b957408d8)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fd5308b7-7430-4713-922c-f06c46886fad)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1a737d87-0689-470b-8fc0-8c874af18794)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc4412ee-8cb8-42e9-96fe-0be49af149b2)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c4b8af1c-b483-4aed-9be5-b0f1698b2c28)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=472842c4-5fe7-4d4c-a927-05be030b5b4e)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=098607b3-9424-4440-8832-fc1de010977e)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="6">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows 7 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=e8549243-e6bf-4007-9bc3-d9c2a24936ef)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=595e72c3-f195-4f93-b24e-afe444abd628)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=48ca08c8-78cc-4b09-a0ec-bcd208668620)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=605f64bd-0615-47d8-bb32-6bc3e80da4a7)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor 32-bits systemen Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e8549243-e6bf-4007-9bc3-d9c2a24936ef)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=595e72c3-f195-4f93-b24e-afe444abd628)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=48ca08c8-78cc-4b09-a0ec-bcd208668620)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=605f64bd-0615-47d8-bb32-6bc3e80da4a7)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=7f0f54e4-b9d9-45d8-bc58-05d7e7b75f07)  
(KB2685939)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=30feb2fe-b19b-4d02-8c5b-4499dd6905d1)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bf8dbfee-573b-4d45-a752-90e1d485e503)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=3c77ca1f-2eec-4f95-a769-973b75af184c)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=c2b47091-534f-41c3-a229-b5a9ec4b64bb)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor x64-systemen Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7f0f54e4-b9d9-45d8-bc58-05d7e7b75f07)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=30feb2fe-b19b-4d02-8c5b-4499dd6905d1)  
(KB2699988)  
(Kritiek)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bf8dbfee-573b-4d45-a752-90e1d485e503)  
(KB2699988)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3c77ca1f-2eec-4f95-a769-973b75af184c)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c2b47091-534f-41c3-a229-b5a9ec4b64bb)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 R2 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9464b044-e40b-4300-97b8-dc3a13c85929)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c8b04-b749-4c6c-8b9f-244abc5f8ecf)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor x64-systemen Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9464b044-e40b-4300-97b8-dc3a13c85929)  
(KB2699988)  
(Gemiddeld)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c8b04-b749-4c6c-8b9f-244abc5f8ecf)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=8ecc5d12-9921-4d04-a04c-d69e8f4349dc)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=40302688-fcda-489c-87c4-480d3b9d754c)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=039ddfe1-3ce5-48d8-8cb4-65481da3f29c)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8ecc5d12-9921-4d04-a04c-d69e8f4349dc)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=40302688-fcda-489c-87c4-480d3b9d754c)  
(KB2699988)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=039ddfe1-3ce5-48d8-8cb4-65481da3f29c)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="6">
Server Core-installatieoptie
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
Geen
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
Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8dcb487-0df7-46f4-8726-bd58e2722812)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6398a156-9618-4ca4-95bc-d36ecacf0745)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40c16540-7839-412c-b474-892292a96fa5)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc4412ee-8cb8-42e9-96fe-0be49af149b2)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor x64-systemen Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritiek)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerking** **bij** **MS12-038**

<sup>[1]</sup>**.NET Framework 4 en .NET Framework 4 Client Profile worden getroffen.** De herdistribueerbare pakketten van .NET Framework versie 4 zijn beschikbaar in twee profielen: .NET Framework 4 en .NET Framework 4 Client Profile. .NET Framework 4 Client Profile is een onderdeel van .NET Framework 4. Het beveiligingslek dat wordt opgelost met deze update, treft zowel .NET Framework 4 als .NET Framework 4 Client Profile. Voor meer informatie raadpleegt u het MSDN-artikel [Installing the .NET Framework](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx).

#### Microsoft Communications-platforms en -software

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Communicator
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488)
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
Microsoft Communicator 2007 R2
</td>
<td style="border:1px solid black;">
[Microsoft Communicator 2007 R2](http://www.microsoft.com/downloads/details.aspx?familyid=75eea324-689a-4892-bdd9-03ef399c4cba)  
(KB2708980)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Lync
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 (32-bits)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 (32-bits)](http://www.microsoft.com/downloads/details.aspx?familyid=425406ea-28b9-46f7-8c49-0c7ea46f16e3)  
(KB2693282)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64-bits)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 (64-bits)](http://www.microsoft.com/downloads/details.aspx?familyid=06e5285f-1947-4409-b608-e0a145fadba4)  
(KB2693282)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendee](http://www.microsoft.com/downloads/details.aspx?familyid=c40f0d38-af90-4966-a0f0-346fa48683d0)  
(installatie op beheerdersniveau)  
(KB2696031)  
(Belangrijk)  
[Microsoft Lync 2010 Attendee](http://www.microsoft.com/downloads/details.aspx?familyid=ad864c0e-5850-44a3-b74f-5980a998a384)<sup>[1]</sup>
(installatie op gebruikersniveau)  
(KB2693283)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendant (32-bits)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendant (32-bits)](http://www.microsoft.com/downloads/details.aspx?familyid=fe7ad0f9-ee84-4cda-b252-a8d31ead5053)  
(KB2702444)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendant (64-bits)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendant (64-bits)](http://www.microsoft.com/downloads/details.aspx?familyid=fe7ad0f9-ee84-4cda-b252-a8d31ead5053)  
(KB2702444)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerking bij MS12-039**

<sup>[1]</sup>Deze update is alleen verkrijgbaar via het Microsoft Downloadcentrum.

#### Microsoft ERP-oplossingen (Enterprise Resource Planning)

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Dynamics ERP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS12-040**](http://go.microsoft.com/fwlink/?linkid=251612)
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
Microsoft Dynamics AX 2012
</td>
<td style="border:1px solid black;">
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=45df362d-8fed-4d99-91c1-81c61878300a)<sup>[1]</sup>
(KB2706738)  
(Belangrijk)  
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=780ddcef-19da-44c4-beca-d10b652cd22a)<sup>[1]</sup>
(KB2710639)  
(Belangrijk)  
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=41dc5958-c224-40f9-89c2-179607a8ee2a)<sup>[1]</sup>
(KB2711239)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerking bij MS12-040**

<sup>[1]</sup>Deze update is alleen verkrijgbaar via het Microsoft Downloadcentrum en de Microsoft Dynamics CustomerSource- en Microsoft Dynamics PartnerSource-websites.

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

**SystemCenter Configuration Manager**

Software-updatebeheer van System Center Configuration Manager vereenvoudigt de complexe taak van het verspreiden en beheren van updates op IT-systemen binnen een onderneming. Met System Center Configuration Manager kunnen IT-beheerders updates van Microsoft-producten verspreiden over diverse apparaten, waaronder pc's, laptops, servers en mobiele apparaten.

De geautomatiseerde beveiligingslekbeoordeling in System Center Configuration Manager bepaalt of updates nodig zijn en rapporteert over aanbevolen acties. Het software-updatebeheer van System Center Configuration Manager is ingebouwd in Microsoft Windows Software Update Services (WSUS), een langdurig geteste update-infrastructuur die vertrouwd is voor IT-beheerders over de gehele wereld. Zie [Software-updates beheren](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx) voor meer informatie over hoe beheerders System Center Configuration Manager kunnen gebruiken om updates te implementeren. Ga naar [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx) voor meer informatie over System Center Configuration Manager.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers.

**Opmerking** De algemene ondersteuning van System Management Server 2003 is beëindigd met ingang van 12 januari 2010. Voor meer informatie over productlevenscycli gaat u naar [Microsoft Support Lifecycle](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). De volgende release van SMS, System Center Configuration Manager, is nu verkrijgbaar. Zie **System Center Configuration Manager**.

Voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren, gaat u naar [Scenario's en procedures voor Microsoft Systems Management Server 2003: Softwaredistributie en patchbeheer](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Voor informatie over SMS gaat u naar het [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Opmerking** SMS maakt gebruik van de Microsoft Baseline Security Analyzer om brede ondersteuning te kunnen bieden voor het zoeken en installeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)) gebruiken.

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows-updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

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

-   Een anonieme onderzoeker, in samenwerking met [VeriSign iDefense Labs](http://labs.idefense.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Adi Cohen van [IBM Security Systems - Application Security](http://blog.watchfire.com/) voor het melden van een probleem dat wordt beschreven in MS12-037
-   Masato Kinugawa voor het melden van een probleem dat wordt beschreven in MS12-037
-   Roman Shafigullin van LinkedIn voor het melden van een probleem dat wordt beschreven in MS12-037
-   Code Audit Labs van [VulnHunt](http://www.vulnhunt.com) voor het melden van een probleem dat wordt beschreven in MS12-037
-   Dark Son van [VulnHunt](http://www.vulnhunt.com) voor het melden van een probleem dat wordt beschreven in MS12-037
-   [Qihoo 360 Security Center](http://www.360.cn/) voor de samenwerking bij het oplossen van een probleem dat wordt beschreven in MS12-037
-   Yichong Lin van McAfee Labs voor de samenwerking bij het oplossen van een probleem dat wordt beschreven in MS12-037
-   [Google Inc.](http://www.google.com/) voor de samenwerking bij het oplossen van een probleem dat wordt beschreven in MS12-037
-   [VUPEN Security](http://www.vupen.com), in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van het probleem dat wordt beschreven in MS12-037
-   Een anonieme onderzoeker, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Een anonieme onderzoeker, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Een anonieme onderzoeker, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Een anonieme onderzoeker, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Een anonieme onderzoeker, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-037
-   Vitaliy Toropov, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-038
-   hamburgers maccoy via Secunia SVCRP voor het melden van een probleem dat wordt beschreven in MS12-039
-   Adi Cohen van [IBM Security Systems - Application Security](http://blog.watchfire.com/) voor het melden van een probleem dat wordt beschreven in MS12-039
-   Alin Rad Pop, in samenwerking met [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/), voor het melden van een probleem dat wordt beschreven in MS12-039
-   Finian Mackin voor het melden van een probleem dat wordt beschreven in MS12-040
-   Tarjei Mandt van [Azimut Security](http://www.azimuthsecurity.com/) voor het melden van drie problemen die worden beschreven in MS12-041
-   [Mateusz "j00 ru" Jurczyk](http://j00ru.vexillium.org) van [Google Inc.](http://www.google.com) voor het melden van een probleem dat wordt beschreven in MS12-041
-   Rafal Wojtczuk van [Bromium](http://www.bromium.com/) en Jan Beulich van [SUSE](http://www.suse.com/) voor het melden van een probleem dat wordt beschreven in MS12-042

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Beveiligingsoplossingen voor IT-professionals: [Ondersteuning en probleemoplossing van TechNet Security](http://technet.microsoft.com/security/bb980617.aspx)
-   Help uw computer met Windows te beschermen tegen virussen en schadelijke software: [Virus Solution and Security Center](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokale ondersteuning in uw land: [Internationale ondersteuning](http://support.microsoft.com/common/international.aspx)

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voor zover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (12 juni 2012): Samenvatting van de gepubliceerde bulletins.

*Built at 2014-04-18T01:50:00Z-07:00*
