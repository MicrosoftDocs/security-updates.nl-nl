---
TOCTitle: 'MS09-OCT'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor oktober 2009'
ms:assetid: 'ms09-oct'
ms:contentKeyID: 61231976
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms09-oct(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor oktober 2009
=====================================================================

Gepubliceerd: dinsdag 13 oktober 2009 | Bijgewerkt: dinsdag 22 juni 2010

**Versie:** 4.2

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor oktober 2009.

Met de release van de bulletins voor oktober 2009 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die is uitgegeven op 8 oktober 2009. Ga voor meer informatie over de vooraankondiging van de bulletins naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 14 oktober 2009 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van oktober.](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407488&culture=en-us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

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
<th style="border:1px solid black;" >Software waarin dit probleem optreedt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-050">MS09-050</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in SMBv2 kan externe code worden uitgevoerd (975517)</strong><br />
<br />
Deze beveiligingsupdate lost één openbaar vrijgegeven en twee privé gemelde beveiligingslekken in Server Message Block Versie 2 (SMBv2) op. Als gevolg van het ernstigste beveiligingslek kan externe code worden uitgevoerd indien een aanvaller een speciaal vervaardigd SMB-pakket naar een computer heeft verzonden waarop de Server-service wordt uitgevoerd. Met aanbevolen procedures voor firewalls en standaardfirewallconfiguraties kunt u netwerken beveiligen tegen aanvallen die vanuit het bedrijfsnetwerk komen. Het wordt aanbevolen op de systemen die met internet zijn verbonden zo min mogelijk poorten bloot te stellen aan deze aanvallen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-051">MS09-051</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Windows Media Runtime kan externe code worden uitgevoerd (975682)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Windows Media Runtime opgelost. Door de beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen mediabestand opent of speciaal ontworpen streaming content ontvangt van een website of een toepassing die webinhoud levert. Een aanvaller die erin slaagt misbruik te maken van deze beveiligingslekken, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-052">MS09-052</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Windows Media Player kan externe code worden uitgevoerd (974112)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Media Player opgelost. Door het beveiligingslek kan externe code worden uitgevoerd indien een speciaal vervaardigd ASF-bestand wordt afgespeeld met Windows Media Player 6.4. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-054">MS09-054</a></td>
<td style="border:1px solid black;"><strong>Cumulatieve beveiligingsupdate voor Internet Explorer (974455)</strong><br />
<br />
Met deze beveiligingsupdate worden drie privé gemelde beveiligingslekken en een openbaar gemaakt beveiligingslek in Internet Explorer opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina weergeeft in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. Gebruikers van Firefox die de Windows Presentation Foundation-invoegtoepassing gebruiken en deze invoegtoepassing niet hebben uitgeschakeld, dienen deze beveiligingsupdate toe te passen. Zie de sectie Veelgestelde vragen over het beveiligingslek met betrekking tot de afhandeling van HTML's – CVE-2009-2529 voor meer informatie over dit probleem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-055">MS09-055</a></td>
<td style="border:1px solid black;"><strong>Cumulatieve beveiligingsupdate voor ActiveX kill-bits (973525)</strong><br />
<br />
Deze beveiligingsupdate lost een privé gemeld beveiligingslek in ActiveX-besturingselementen op dat momenteel wordt misbruikt. Door het beveiligingslek dat ActiveX-besturingselementen treft die zijn gecompileerd met de versie van de Microsoft Active Template Library (ATL) waarin dit probleem optreedt, kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina opent met Internet Explorer, waardoor het ActiveX-besturingselement wordt gestart. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-060">MS09-060</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Active X-besturingselementen voor de Microsoft Active Template Library (ATL) voor Microsoft Office kan externe code worden uitgevoerd (973965)</strong><br />
<br />
Deze beveiligingsupdate lost diverse privé gemelde beveiligingslekken op in ActiveX-besturingselementen voor Microsoft Office die zijn gecompileerd met een versie van de Microsoft Active Template Library (ATL) waarin dit probleem optreedt. Door de beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd onderdeel of besturingselement heeft geladen. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-061">MS09-061</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de Microsoft .NET Common Language Runtime kan externe code worden uitgevoerd (974378)</strong><br />
<br />
Door deze update worden drie privé gemelde beveiligingslekken in Microsoft .NET Framework en Microsoft Silverlight opgelost. Door de beveiligingslekken kan externe code worden uitgevoerd op een client-systeem als een gebruiker een speciaal vervaardigde webpagina bekijkt met een webbrowser die XAML Browser Applications (XBAPs) of Silverlight kan uitvoeren, of als een aanvaller een gebruiker ertoe kan bewegen een speciaal vervaardigde Microsoft .NET-toepassing uit te voeren. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. Door de beveiligingslekken kan ook externe code worden uitgevoerd op een server-systeem waarop IIS actief is, indien die server verwerking van ASP.NET-pagina's toestaat en het een aanvaller lukt een speciaal vervaardigde ASP.NET-pagina te uploaden naar die server en die pagina te laten uitvoeren, zoals het geval kan zijn bij webhosting. Microsoft .NET-toepassingen, Silverlight-toepassingen, XBAPs en ASP.NET-pagina's die niet schadelijk zijn, zijn niet kwetsbaar voor dit probleem.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-062">MS09-062</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)</strong><br />
<br />
Met deze beveiligingsupdate worden enkele privé gemelde beveiligingslekken in Microsoft Windows GDI+ opgelost. Door deze beveiligingslekken kan programmacode vanaf een externe locatie worden uitgevoerd indien een gebruiker een speciaal vervaardigd afbeeldingsbestand opent met de software waarin dit probleem optreedt of een website met speciaal vervaardigde inhoud bezoekt. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer,<br />
Microsoft .NET Framework,<br />
Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft-ontwikkelprogramma's<br />
Microsoft Forefront</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-053">MS09-053</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de FTP-service voor Internet Information Services kan externe code worden uitgevoerd (975254)</strong><br />
<br />
Deze beveiligingsupdate lost twee openbaar vrijgegeven beveiligingslekken op in de FTP-service van Microsoft Internet Information Services (IIS) 5.0, Microsoft Internet Information Services (IIS) 5.1, Microsoft Internet Information Services (IIS) 6.0 en Microsoft Internet Information Services (IIS) 7.0 op. Op IIS 7.0 is dit beveiligingslek alleen van toepassing op FTP Service 6.0. Door beveiligingslekken kan externe code worden uitgevoerd (RCE) op systemen waarop de FTP-service op IIS 5.0 wordt uitgevoerd, of is denial of service (DoS) mogelijk op systemen waarop FTP Service wordt uitgevoerd op IIS 5.0, IIS 5.1, IIS 6.0 of IIS 7.0.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-056">MS09-056</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Windows CryptoAPI is spoofing mogelijk (974571)</strong><br />
<br />
Met deze beveiligingsupdate worden twee openbaar vrijgegeven beveiligingslekken in Microsoft Windows opgelost. Door deze beveiligingslekken is vervalsing (spoofing) mogelijk als een aanvaller toegang weet te krijgen tot het certificaat dat de eindgebruiker gebruikt voor verificatie.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Spoofing</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-057">MS09-057</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in de Indexing-service kan externe code worden uitgevoerd (969059)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een aanvaller een schadelijke website opstelt die de Indexing-service aanroept via een oproep voor het ActiveX-onderdeel. Deze oproep kan een schadelijke URL bevatten waardoor misbruik kan worden gemaakt van het beveiligingslek en de aanvaller toegang krijgt tot het clientsysteem met de bevoegdheden van de gebruiker die de website heeft geopend. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-058">MS09-058</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (971486)</strong><br />
<br />
Met deze beveiligingsupdate worden verschillende privé gemelde beveiligingslekken in de Windows-kernel opgelost. Het meest ernstige beveiligingslek kan leiden tot misbruik van bevoegdheden als een aanvaller zich aanmeldt op een systeem en een speciaal vervaardigde toepassing uitvoert. Om misbruik te kunnen maken van deze beveiligingslekken, moet een aanvaller geldige aanmeldingsreferenties hebben en zich lokaal kunnen aanmelden. De beveiligingslekken kunnen niet vanaf een externe locatie of door anonieme gebruikers worden misbruikt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-059">MS09-059</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in de Local Security Authority Subsystem-service kan leiden tot denial of service (975467)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Het beveiligingslek kan leiden tot denial of service als een aanvaller een schadelijk pakket verzendt tijdens de NTLM-verificatie.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Denial of service</td>
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
  
| Bulletin-id                                                         | Titel bulletin                                                                                                                                                   | CVE-id                                                                           | Beoordeling van de exploitatie-index                                                                                 | Belangrijke opmerkingen                                                                                                                                                                                                                                                                                                                                                                                                  |  
|---------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-050](http://technet.microsoft.com/security/bulletin/ms09-050) | Door beveiligingslekken in SMBv2 kan externe code worden uitgevoerd (975517)                                                                                     | [CVE-2009-2526](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2526) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit beveiligingslek heeft betrekking op een denial of service.                                                                                                                                                                                                                                                                                                                                                           |  
| [MS09-050](http://technet.microsoft.com/security/bulletin/ms09-050) | Door beveiligingslekken in SMBv2 kan externe code worden uitgevoerd (975517)                                                                                     | [CVE-2009-2532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2532) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-050](http://technet.microsoft.com/security/bulletin/ms09-050) | Door beveiligingslekken in SMBv2 kan externe code worden uitgevoerd (975517)                                                                                     | [CVE-2009-3103](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3103) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | De exploitatiecode is openbaar gepubliceerd.                                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-051](http://technet.microsoft.com/security/bulletin/ms09-051) | Door beveiligingslekken in Windows Media Runtime kan externe code worden uitgevoerd (975682)                                                                     | [CVE-2009-0555](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0555) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-051](http://technet.microsoft.com/security/bulletin/ms09-051) | Door beveiligingslekken in Windows Media Runtime kan externe code worden uitgevoerd (975682)                                                                     | [CVE-2009-2525](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2525) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-052](http://technet.microsoft.com/security/bulletin/ms09-052) | Door een beveiligingslek in Windows Media Player kan externe code worden uitgevoerd (974112)                                                                     | [CVE-2009-2527](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2527) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-053](http://technet.microsoft.com/security/bulletin/ms09-053) | Door beveiligingslekken in de FTP-service van Internet Information Services kan externe code worden uitgevoerd (975254)                                          | [CVE-2009-2521](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2521) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit beveiligingslek heeft betrekking op een denial of service. De exploitatiecode is openbaar gepubliceerd.                                                                                                                                                                                                                                                                                                              |  
| [MS09-053](http://technet.microsoft.com/security/bulletin/ms09-053) | Door beveiligingslekken in de FTP-service van Internet Information Services kan externe code worden uitgevoerd (975254)                                          | [CVE-2009-3023](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3023) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | De exploitatiecode is openbaar gepubliceerd.                                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-054](http://technet.microsoft.com/security/bulletin/ms09-054) | Cumulatieve beveiligingsupdate voor Internet Explorer (974455)                                                                                                   | [CVE-2009-1547](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1547) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-054](http://technet.microsoft.com/security/bulletin/ms09-054) | Cumulatieve beveiligingsupdate voor Internet Explorer (974455)                                                                                                   | [CVE-2009-2529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2529) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-054](http://technet.microsoft.com/security/bulletin/ms09-054) | Cumulatieve beveiligingsupdate voor Internet Explorer (974455)                                                                                                   | [CVE-2009-2530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Op Microsoft Windows 2000-systemen verhoogt het tekort aan heapbescherming de beoordeling van de exploitatie-index tot [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk.                                                                                                                                                                               |  
| [MS09-054](http://technet.microsoft.com/security/bulletin/ms09-054) | Cumulatieve beveiligingsupdate voor Internet Explorer (974455)                                                                                                   | [CVE-2009-2531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2531) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk |                                                                                                                                                                                                                                                                                                                                                                                                                          |  
| [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055) | Cumulatieve beveiligingsupdate voor ActiveX kill-bits (973525)                                                                                                   | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Geen                                                                                                                 | (Aan dit beveiligingslek is reeds een misbruikindexbeoordeling toegewezen in [de samenvatting van het bulletin voor juli](http://technet.microsoft.com/security/bulletin/ms09-jul). Dat komt doordat dit beveiligingslek voor het eerst in [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) is behandeld.) Zie ook hetzelfde CVE-nummer in [MS09-060](http://technet.microsoft.com/security/bulletin/ms09-060). |  
| [MS09-056](http://technet.microsoft.com/security/bulletin/ms09-056) | Door beveiligingslekken in Windows CryptoAPI is spoofing mogelijk (974571)                                                                                       | [CVE-2009-2510](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2510) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit is een beveiligingslek dat betrekking heeft op spoofing.                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-056](http://technet.microsoft.com/security/bulletin/ms09-056) | Door beveiligingslekken in Windows CryptoAPI is spoofing mogelijk (974571)                                                                                       | [CVE-2009-2511](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2511) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit is een beveiligingslek dat betrekking heeft op spoofing.                                                                                                                                                                                                                                                                                                                                                             |  
| [MS09-057](http://technet.microsoft.com/security/bulletin/ms09-057) | Door een beveiligingslek in de Indexing-service kan externe code worden uitgevoerd (969059)                                                                      | [CVE-2009-2507](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2507) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-058](http://technet.microsoft.com/security/bulletin/ms09-058) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (971486)                                                                     | [CVE-2009-2515](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2515) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-058](http://technet.microsoft.com/security/bulletin/ms09-058) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (971486)                                                                     | [CVE-2009-2516](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2516) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit beveiligingslek kan leiden tot een denial of service in het geval van een gedeelde netwerklocatie en tot misbruik van bevoegdheden wanneer er lokaal misbruik wordt gemaakt van het beveiligingslek, gericht op een lokaal systeem.                                                                                                                                                                                  |  
| [MS09-058](http://technet.microsoft.com/security/bulletin/ms09-058) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (971486)                                                                     | [CVE-2009-2517](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2517) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit beveiligingslek heeft betrekking op een denial of service.                                                                                                                                                                                                                                                                                                                                                           |  
| [MS09-059](http://technet.microsoft.com/security/bulletin/ms09-059) | Beveiligingslek in de Local Security Authority Subsystem-service kan leiden tot denial of service (975467)                                                       | [CVE-2009-2524](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2524) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit beveiligingslek heeft betrekking op een denial of service.                                                                                                                                                                                                                                                                                                                                                           |  
| [MS09-060](http://technet.microsoft.com/security/bulletin/ms09-060) | Door beveiligingslekken in Microsoft Active Template Library (ATL) ActiveX-besturingselementen voor Microsoft Office kan externe code worden uitgevoerd (973965) | [CVE-2009-0901](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0901) | Geen                                                                                                                 | (Aan dit beveiligingslek is reeds een misbruikindexbeoordeling toegewezen in [de samenvatting van het bulletin voor juli](http://technet.microsoft.com/security/bulletin/ms09-jul). Dat komt doordat dit beveiligingslek voor het eerst in [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) is behandeld.)                                                                                                      |  
| [MS09-060](http://technet.microsoft.com/security/bulletin/ms09-060) | Door beveiligingslekken in Microsoft Active Template Library (ATL) ActiveX-besturingselementen voor Microsoft Office kan externe code worden uitgevoerd (973965) | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Geen                                                                                                                 | (Aan dit beveiligingslek is reeds een misbruikindexbeoordeling toegewezen in [de samenvatting van het bulletin voor juli](http://technet.microsoft.com/security/bulletin/ms09-jul). Dat komt doordat dit beveiligingslek voor het eerst in [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) is behandeld.) Zie ook hetzelfde CVE-nummer in [MS09-055](http://technet.microsoft.com/security/bulletin/ms09-055). |  
| [MS09-060](http://technet.microsoft.com/security/bulletin/ms09-060) | Door beveiligingslekken in Microsoft Active Template Library (ATL) ActiveX-besturingselementen voor Microsoft Office kan externe code worden uitgevoerd (973965) | [CVE-2009-2495](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2495) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit is een beveiligingslek met betrekking tot het vrijgeven van informatie.                                                                                                                                                                                                                                                                                                                                              |  
| [MS09-061](http://technet.microsoft.com/security/bulletin/ms09-061) | Door beveiligingslekken in de Microsoft .NET Common Language Runtime kan externe code worden uitgevoerd (974378)                                                 | [CVE-2009-0090](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0090) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-061](http://technet.microsoft.com/security/bulletin/ms09-061) | Door beveiligingslekken in de Microsoft .NET Common Language Runtime kan externe code worden uitgevoerd (974378)                                                 | [CVE-2009-0091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0091) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-061](http://technet.microsoft.com/security/bulletin/ms09-061) | Door beveiligingslekken in de Microsoft .NET Common Language Runtime kan externe code worden uitgevoerd (974378)                                                 | [CVE-2009-2497](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2497) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Er is een kans op aanvallen die gevolgen hebben voor internet.                                                                                                                                                                                                                                                                                                                                                           |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2500](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2500) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2501](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2501) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2502](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2502) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2503](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2503) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2504](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2504) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2518](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2518) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-2528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2528) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |  
| [MS09-062](http://technet.microsoft.com/security/bulletin/ms09-062) | Door beveiligingslekken in GDI+ kan externe code worden uitgevoerd (957488)                                                                                      | [CVE-2009-3126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3126) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                                                                                                                                   |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
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
<th colspan="13">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
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
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Geen**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[DirectShow-WMA-spraakcodec](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=8f850a82-61f9-447b-a0aa-a2c192cc5d2e)  
(KB954155)  
(Kritiek)  
[Audiocompressiebeheer](http://www.microsoft.com/downloads/details.aspx?familyid=6dfd5405-cabe-4bd7-9330-b6bde1d99194)  
(KB975025)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=13035ef7-7e47-487c-8b7c-7795d33ce7de)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=26515c7b-d7a6-4405-96b5-a518dcb39d38)  
(Kritiek)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8154ba37-0fbc-4d31-9d6e-0b21586ad65a)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=edfea805-9544-4dc0-a52c-d7594205657b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f3fef608-dafb-4b37-a65a-9cc4ae8e2c4c)  
(KB958869)  
(Kritiek)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ecf78619-80fa-417d-852b-1b5b2cf574e2)  
(KB971108)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e534aa8-29c2-4379-9f57-931a6ff47418)  
(KB971110)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e6f5e730-85cc-4c08-a50d-c456b1e9f5bc)  
(KB971111)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=7fecd367-aaff-458b-91bc-8925c8e57528)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=52b9198d-b65f-467a-a5ab-141e23d64a86)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=b34d94b5-b828-4e16-a636-04344c60d945)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bdfa6583-28a2-4d6b-91d2-157a8518b664)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="13">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
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
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[DirectShow-WMA-spraakcodec](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=4516c219-e357-485e-a52b-23dcb8ee49d8)  
(KB954155)  
(Kritiek)  
(Uitsluitend Windows XP Service Pack 2)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=746d3440-5a6a-421e-9286-7b534a1dfe54)  
(KB954155)  
(Kritiek)  
(Uitsluitend Windows XP Service Pack 3)  
[Audiocompressiebeheer](http://www.microsoft.com/downloads/details.aspx?familyid=6ecc7129-8caa-4daf-a8e2-8f3536225fb3)  
(KB975025)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=b2efe1ac-d8d7-41bb-b87d-fc5e22afef0f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9aacf890-afb4-46a7-a13f-dd9fe3c0ca4a)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=dc166dc6-577f-4d8d-94df-dd963233dd85)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8799159d-df69-49f6-9db5-49147690ce0c)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=171d43d3-669c-4923-b266-e47591833c05)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1bc56c26-1c7c-47e3-94f4-37af7e00392c)  
(KB953295)  
(Kritiek)  
(alleen Tablet PC Edition 2005 en Media Center Edition 2005)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e2acde20-a6d3-4135-b6eb-1214f743d474)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ae0bdd4-f8b2-420a-b1ac-d2cdaa87c828)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9c5ab624-e37b-418a-a919-d8f652b15679)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=768fd74e-0a2f-4353-ac22-65d0d6321739)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cece4c55-0756-4357-9d2d-6709e8426068)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e997ea40-668e-40df-bd50-0ca53437b375)<sup>[1]</sup>
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[DirectShow-WMA-spraakcodec](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=4729de51-8fd8-46c6-b4ad-9c9f25202684)  
(KB954155)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) in Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=a866a490-6d3a-4ecd-acf4-770312ba2fd6) in Windows Media Format SDK 11  
(KB954155)  
(Kritiek)  
[Audiocompressiebeheer](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=a9e7dfd8-7ba1-4f14-8e60-92ef00d91467)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=89a2cf2a-a7a2-4d4b-aa6f-24dde288d500)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd54e595-25f2-4839-a838-2a0f809bde2b)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=77b18fc2-e769-47c6-8e72-916716a49e58)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c08623bf-94bc-4c50-8c10-f50fb8448a0b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad92503a-8c91-4d73-98b0-942d7961637d)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=819dd2d1-cad5-4784-9baf-185d8a76df5d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad29696d-4611-4a12-9dfa-74fa6866b759)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=270ec100-5ba1-4f8c-aa36-105d30ad57bf)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5459b7d4-1fab-4a04-ab9d-b8323505c1e2)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17008892-7950-44c4-850d-002c8d73495f)<sup>[1]</sup>
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[DirectShow-WMA-spraakcodec](http://www.microsoft.com/downloads/details.aspx?familyid=4fe0dff5-04d9-4409-8d1d-52419537126b)  
(KB969878)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=00b3cb86-c9eb-4fbe-987e-2b0d94271d87)  
(KB954155)  
(Kritiek)  
[Audiocompressiebeheer](http://www.microsoft.com/downloads/details.aspx?familyid=ab1803ff-2371-487f-a7b6-95747c46ba4e)  
(KB975025)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=5f82d01c-573e-425e-b9f2-86a54f377b19)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8101625d-ee93-46e5-aec2-3bdbf2d86472)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4647bcf1-69fb-4ad6-9e03-7bc22d8a914b)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9eae7eca-1a6f-4397-a6e2-7dda6b9d5276)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f3249c99-82e4-45dc-a254-28e647e822c8)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d1b4a58b-f0b1-4400-a6e6-0255b0513bd1) (KB953298)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=414466a4-39a0-476d-9a43-ae7674cbd6a0)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48256ea3-b433-4e84-9019-22300069cfc1)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=78072164-84d1-44da-8ede-2a9d212d47a9)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3f3842-f8fd-4969-a2cf-706db38d7580)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9dff4662-7771-4bdc-87ec-7899d79b3a55)<sup>[1]</sup>
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[DirectShow-WMA-spraakcodec](http://www.microsoft.com/downloads/details.aspx?familyid=c116ae9d-e416-4b7d-be75-4b4b2ebcc33a)  
(KB969878)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=13ba4839-7fa9-4bbb-95f6-3fafb6c49f20)  
(KB954155)  
(Kritiek)  
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=fe0d51b2-345e-4eb7-a036-d8c3f6a683d2) in Windows Media Format SDK 9.5 x64 Edition  
(KB954155)  
(Kritiek)  
[Audiocompressiebeheer](http://www.microsoft.com/downloads/details.aspx?familyid=46daf7c7-1cd3-4f47-9c7a-d5eb6ea7327b)  
(KB975025)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=65e9036e-2e1b-40ff-a84b-c507107bcce8)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2f966053-01eb-4a23-a9d5-71deac2498ea)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e7d77bd9-8317-42f3-9ad1-a0b8bfa65b53)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=708a549d-11fd-43bf-a6e1-309e3205d59d)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ad3f7b3-58d5-4507-ae20-a265e47cee9c)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eb95e8d9-6ef5-4526-99d2-507e50de049b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61bded07-201e-4815-ac1e-468bf907e063)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d170cef9-f5d2-4fcd-997b-e778ad5a6797)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8aa1f97d-ad53-4450-bb93-4a147dd10a87)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=95286b8d-4b53-4e6c-af59-e9e18fad3559)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8df7a2d9-2f97-4f18-84e8-415a1632cf09)<sup>[1]</sup>
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=79a1a94d-3b47-47e9-9476-2f591c3f6a59)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=07e66c09-2cd7-47ba-bf87-d3da602184b4)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=575e75d9-e348-4fbb-9eaa-43240e4d715e)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=d4a328b5-5470-46b0-86c7-cfe0e6a3ea01) (KB953300)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=491874d4-5eea-4545-9b7d-3861857c862e) (KB974417)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=a678ceb9-a37a-4c29-8bd1-f209922990e5)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b99d4d9b-e0cc-4a8c-ad99-6a53958b37c8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=2ede1eb9-7f5f-411d-bbc3-5db46d80e0bb)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=fb5678b9-5ef1-42db-902e-c9ea02880e0a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=faef714b-5f46-47f2-bea7-881df05a1bc0)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=83c77015-7f96-4c0d-bd56-60aef90ea2f8)<sup>[1]</sup>
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="13">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
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
Geen
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Vista
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29842c0c-8930-4b5f-83c6-1a718974b63f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=f17ee0ea-f1e2-49f4-9f90-60296246ddfe)  
(KB954155)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f6995616-2a84-4c26-9599-26f1314873ed)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e8f6014f-950b-4e11-a105-51d298069f1a)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7313c03b-8844-4086-a0cc-43dfdb3ca48c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=19aa01f3-026d-4264-85f8-216d0597969b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bb96eb1c-66a2-4276-9773-eea22179bcd4)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b5a9a95-9439-40c8-acef-000b919daa04)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=04ae306b-0d0d-4767-ab54-cc11aec477ed)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=acf6f3e6-282e-4f05-9060-8d0ebb874b97)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62ed5d0a-5ca6-4942-80c9-7808b14cb6b5)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Audio-spraakdecoder](http://www.microsoft.com/downloads/details.aspx?familyid=26905f12-92c7-4d45-99e7-227f03d2cb82)  
(KB954155)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3de5236-afdd-436e-8648-5382d564cc99)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=85978f28-5fc0-481b-9b03-2021c785889b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7216bcb1-ff16-402b-ad1b-1500d46d0157)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=6f99521e-86b3-4083-9132-e5ac06d40b63) (KB974468)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1 en Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=3cf329c6-6d3d-41eb-bb72-8ba241df0882) (KB974292)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7438eb1e-6e86-4aa1-b1f4-f71a7699d233) (KB974467)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8f5f0c1d-1dd6-47fa-aef2-d3c96c8fc06e)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bce096c8-833b-45c8-99cd-1280f0744f2f)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4a60f789-1a4a-49a8-8d13-fda989ed40be)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=58c995ca-f308-4e07-8e60-2e542384d95d)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda) (KB974291)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8) (KB974469)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f) (KB953297)  
(Kritiek)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4) (KB974470)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a3fe0b-e300-4568-aa08-d586ab8d5434)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
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
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Laag**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2008 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ff6bfcf3-76c9-4c45-b57d-22f94458dd6e)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=2eaa9857-a147-4f31-9bf4-b9e2cf4c15c3)\*\*  
(KB954155)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=72dd580e-eb53-41da-a5c0-a392ad388bfc)\*\*  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1baf7e96-ba3e-47e7-8ea3-eb092e653a39)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51eb56fa-8204-45f3-86d7-6d03a2c8d78d)\*\*  
(Laag)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=fd1694af-8873-43aa-9243-91f7cde452b7)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d9c5039f-d0cf-4d84-850f-f2f7701dcb79)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9b487af-fe73-42a8-b240-d59c4321f95b)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f2f617c2-f149-4e9b-bfdd-08ed0f3f99db)\*  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71aec6f6-a36b-465e-8885-b094dfd30423)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aff6f9c7-4a72-48f2-b750-204d796c7daa)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Audio Voice Decoder](http://www.microsoft.com/downloads/details.aspx?familyid=70aabba3-53d6-4b52-be83-6d3f3869ecbd)\*\*  
(KB954155)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0111d741-bda4-4a50-a12b-d3337ff4441d)\*\*  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7a4b755b-7fa0-43aa-8862-c1d0c7d94c2c)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=131b047a-ae93-4a99-83e5-71d5a79e96ea)\*\*  
(Laag)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
( Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)\*\*  
(KB974291)  
( Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)\*\*  
(KB974469)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=41bc4cdb-273a-4a6e-80d9-c8ce20e32da9)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=db969ddc-708e-42b7-9956-6c27bf346bbb)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0d8a2a3e-d7d4-47fb-8364-16fce28e4d38)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=deb84cb8-2ba3-47e3-9185-2bbc5b0a7e18)\*  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)\*\*  
(KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)\*\*  
(KB974470)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88f4189f-71fe-404a-869e-3f76692acf94)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b70108b-7f59-4898-ab4e-76be990de878)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e81f30b7-ef05-4488-b62a-d330e17129cf)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d16c5bf-ee5c-4220-9755-5cb92eac2aae)  
(Laag)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=30e5410d-0942-4964-9037-52330488efda)  
(KB974291)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2 en Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72fe9066-2397-439d-82fb-2b7f9d2bcce8)  
(KB974469)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=a4f42085-1cb9-4b8d-a931-85be71fdf06d)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a221451a-cb4e-4a43-a225-4b1e86e87525)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8962f0b6-f346-4e88-9d83-4d15b699dd9d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4aac0e3e-9b49-4a4a-ab17-707ff03b4d9b)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=78ac8b97-8327-4ae1-8bb0-6cf227f3968f)  
(KB953297)  
(Belangrijk)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614a92ee-0512-4ccc-b6b8-32ebcec8e6a4)  
(KB974470)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e0f0b1c-ca5d-43fc-9770-73396a5f191c)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Zelfde als boven
</td>
</tr>
<tr>
<th colspan="13">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
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
Geen
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
Windows 7 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=89d1fb78-68cd-48dd-afc2-15a79ebe9fde)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b64bcc14-38a7-45b9-8f85-acc573777506)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=ad6f06d5-27db-445d-a8b2-c42adc90afc0)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=35b85783-90df-4f67-a3cb-02351432133e)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor x64-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=10d9f7ac-65f4-437c-91cc-171632c69b0e)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=809e29f3-ec68-4a2b-b04e-11759dd16001)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=70cd0270-77e9-492a-82d9-798364640c10)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=97010f2c-6c10-4fda-84fd-6c8749968db5)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="13">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-050**](http://technet.microsoft.com/security/bulletin/ms09-050)
</td>
<td style="border:1px solid black;">
[**MS09-051**](http://technet.microsoft.com/security/bulletin/ms09-051)
</td>
<td style="border:1px solid black;">
[**MS09-052**](http://technet.microsoft.com/security/bulletin/ms09-052)
</td>
<td style="border:1px solid black;">
[**MS09-054**](http://technet.microsoft.com/security/bulletin/ms09-054)
</td>
<td style="border:1px solid black;">
[**MS09-055**](http://technet.microsoft.com/security/bulletin/ms09-055)
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
<td style="border:1px solid black;">
[**MS09-053**](http://technet.microsoft.com/security/bulletin/ms09-053)
</td>
<td style="border:1px solid black;">
[**MS09-056**](http://technet.microsoft.com/security/bulletin/ms09-056)
</td>
<td style="border:1px solid black;">
[**MS09-057**](http://technet.microsoft.com/security/bulletin/ms09-057)
</td>
<td style="border:1px solid black;">
[**MS09-058**](http://technet.microsoft.com/security/bulletin/ms09-058)
</td>
<td style="border:1px solid black;">
[**MS09-059**](http://technet.microsoft.com/security/bulletin/ms09-059)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Laag**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
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
Windows Server 2008 R2 voor x64-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=f50307d6-7869-4996-9ff7-23f87d08994b)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=bcd2b944-6852-48f2-820b-cce7d195e391)\*\*  
(Laag)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=ce78c019-ec08-4ec6-abec-334f5ec5cb76)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=597ac3a7-e02d-49a5-9b8e-d097e867acea)\*  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9b6a28ae-b3f2-42b0-8209-e3950ec37abb)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=85e76e55-3766-4ffe-9a18-8655de935b7c)  
(Laag)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=6442a77a-3c0d-4beb-b2d2-2885376c2135)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=abc94857-37d8-4bb8-ad9e-46e687fca40e)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerkingen voor Windows Server 2008 en Windows Server 2008 R2**

**\*Treedt op bij Server Core-installatie.** Deze update is met hetzelfde prioriteitsniveau van toepassing op ondersteunde edities van Windows Server 2008 en Windows Server 2008 R2, zoals is aangegeven, ongeacht of deze zijn geïnstalleerd met de optie Server Core-installatie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Server Core-installatie niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Opmerking voor MS09-061**

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

**Opmerkingen voor MS09-062**

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

**Opmerkingen voor MS09-059**

<sup>[1]</sup>Dit besturingssysteem wordt alleen getroffen wanneer KB968389, Uitgebreide beveiliging voor verificatie (zie [Microsoft-beveiligingsadvies 973811](http://technet.microsoft.com/security/advisory/973811)) is geïnstalleerd. Voor meer informatie raadpleegt u de vermelding in Veelgestelde vragen (FAQ) over deze beveiligingsupdate in [MS09-059](http://technet.microsoft.com/security/bulletin/ms09-059).

#### Microsoft Office-pakketen en -software

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Office-pakketten, -systemen en -onderdelen
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-060**](http://technet.microsoft.com/security/bulletin/ms09-060)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Outlook 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=04878c2c-eb97-426f-be08-89036a6799db)  
(KB973702)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Met Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=79e2b2e8-d5e8-4014-b489-720af2b5083d)  
(KB973705)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office System
</td>
<td style="border:1px solid black;">
[Microsoft Office Outlook 2007 Service Pack 1 en Microsoft Office Outlook 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d39234a3-c62c-44ba-a626-3179a183ca09)  
(KB972363)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[2007 Microsoft Office System Service Pack 1 en 2007 Microsoft Office System Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="3">
Overige Microsoft Office-software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-060**](http://technet.microsoft.com/security/bulletin/ms09-060)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=920ee70b-c5c1-47b5-8f33-938ffe14eea4)  
(KB975365)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio Viewer
</td>
<td style="border:1px solid black;">
Microsoft Visio 2002 Viewer<sup>[1]</sup>
(Kritiek)  
Microsoft Office Visio 2003 Viewer<sup>[1]</sup>
(Kritiek)  
[Microsoft Office Visio Viewer 2007 Service Pack 1 en Microsoft Office Visio Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d20004c5-dd01-459e-8120-5f127e20c085)  
(KB973709)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio Viewer 2007 Service Pack 1 en Microsoft Office Visio Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4ac7fbe-dd19-4940-a576-89a6b7ed602d)<sup>[2]</sup>
(KB974811)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Office Excel Viewer en Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Word Viewer 2003 Service Pack 3 en Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=48752ab4-5928-476d-a8bc-e998d188b1f7)<sup>[3]</sup>
(KB972580)  
(Belangrijk)  
[Microsoft Office Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Belangrijk)  
[PowerPoint Viewer 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=98d7c4ab-f8ca-4806-a609-453fb29b02ec)\[4\]  
(KB972581)  
(Belangrijk
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=6f96de9a-62d8-428f-9567-51d55c129be6)  
(KB973636)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerkingen voor MS09-060**

<sup>[1]</sup>Microsoft raadt gebruikers van Microsoft Visio Viewer 2002 en Microsoft Visio Viewer 2003 aan om de upgrade naar Microsoft Office Visio Viewer 2007 Service Pack 2 aan te schaffen.

**Opmerkingen voor MS09-062**

<sup>[2]</sup>Deze updates zijn identiek.

<sup>[3]</sup>Deze updates zijn identiek.

\[4\]Deze updates zijn identiek.

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

#### Microsoft Server-software

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2000 Reporting Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-update  
Niet van toepassing  
QFE-update:  
[SQL Server 2000 Reporting Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=33554f96-5af7-4683-a537-9db293b67b8d)  
(KB970899)  
(Kritiek)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritiek)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritiek)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-update:  
[SQL Server 2005 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d971a262-1dfb-498c-a4f3-59fdc1b85d23)<sup>[1]</sup>
(KB970895)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76d3d653-e9a0-48bc-afae-d3553f7b9235)<sup>[1]</sup>
(KB970896)  
(Kritiek)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-update  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritiek)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-update:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritiek)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 voor Itanium-systemen Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-update:  
[SQL Server 2005 voor Itanium-systemen Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d878f4b-71e8-4170-9a14-1bce684811ce)<sup>[2]</sup>
(KB970892)  
(Kritiek)  
QFE-update:  
[SQL Server 2005 voor Itanium-systemen Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e6f307c1-8b21-406e-9c6f-b1a3a1e9a98f)<sup>[2]</sup>
(KB970894)  
(Kritiek)
</td>
</tr>
</table>
 
**Opmerking voor MS09-062**

<sup>[1]</sup>Gebruikers van SQL Server 2005 Service Pack 2 met een afhankelijkheid van Reporting Services SharePoint moeten ook de [Microsoft SQL Server 2005 Reporting Services-invoegtoepassing voor Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=%20f4d4d0ae-e5d4-4ed1-8d78-7137578161ce&displaylang=en) installeren via het Microsoft Downloadcentrum.

<sup>[2]</sup>Gebruikers van SQL Server 2005 Service Pack 3 met een afhankelijkheid van Reporting Services SharePoint moeten ook de [Microsoft SQL Server 2005 Reporting Services-invoegtoepassing voor Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=%20648766ac-2a35-4238-a3f4-c26d7077f2a9&displaylang=en) installeren via het Microsoft Downloadcentrum.

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

#### Microsoft-programma's en software voor ontwikkelaars

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> indien geïnstalleerd op Mac  
(KB970363)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> indien geïnstalleerd op alle edities van Microsoft Windows-clients  
(KB970363)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 2](http://www.microsoft.com/silverlight/get-started/install/default.aspx)<sup>[1]</sup> indien geïnstalleerd op alle edities van Microsoft Windows-servers\*\*  
(KB970363)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Visual Studio
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9e3b52d3-b211-4d62-891c-ae8f2e4ffc6c)  
(KB971022)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e186aeed-e9d7-4a02-84b3-bbed116ca060)  
(KB971023)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?familyid=4fa10c93-ce20-43df-a725-ef4c77353747)  
(KB972221)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b904dee8-8a26-43f8-8ca9-86ad12cfdb52)  
(KB972222)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1 indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4  
(KB971104)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5d0d515-4b36-4025-bc6f-1c5cdf09e1af)  
indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4  
(KB971104)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2 indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4  
(KB971105)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2a930f56-59ac-49a6-830f-bfae7c540ec7)  
indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4  
(KB971105)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Report Viewer
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-061**](http://technet.microsoft.com/security/bulletin/ms09-061)
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Herdistribueerbaar pakket voor Microsoft Report Viewer 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=0dfaf300-2b53-4678-a779-0d805ddfe538)  
(KB971117)  
(Kritiek)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=42ed040f-cf94-4754-b0b3-c8016fbcbe22)  
(KB971118)  
(Kritiek)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Herdistribueerbaar pakket voor Microsoft Report Viewer 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6aaa74bd-a46e-4478-b4e1-2063d18d2d42)  
(KB971119)  
(Kritiek)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Platform SDK Redistributable: GDI+
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Platform SDK Redistributable: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(KB975337)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
</tr>
</table>
 
**Opmerkingen voor MS09-061**

<sup>[1]</sup>Deze download werkt Microsoft Silverlight 2 bij naar Microsoft Silverlight 3, waarin het in het bulletin beschreven beveiligingslek is opgelost.

**\*\*Server Core-installatie niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

**Opmerkingen voor MS09-062**

<sup>[2]</sup>Op deze update zijn geen prioriteitsniveaus van toepassing omdat Microsoft geen aanvalsvectoren heeft gevonden die verband houden met de beveiligingslekken die worden besproken in dit bulletin en die specifiek zijn voor deze software. Deze beveiligingsupdate wordt echter aangeboden aan ontwikkelaars die deze software gebruiken zodat zij hun eigen bijgewerkte versie van hun toepassingen kunnen uitgeven.

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

#### Microsoft-beveiligingssoftware

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Forefront Client Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-062**](http://technet.microsoft.com/security/bulletin/ms09-062)
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
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?familyid=c0ce624c-8df3-4223-8a7a-5cba4ac334a8)  
indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4  
(KB975962)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerking voor MS09-062**

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn beschikbaar op [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) en [Windows Update.](http://go.microsoft.com/fwlink/?linkid=21130) Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.

Ten slotte kunt u beveiligingsupdates downloaden uit de [Microsoft Update-catalogus](http://go.microsoft.com/fwlink/?linkid=96155). In de Microsoft Update-catalogus vindt u een doorzoekbare catalogus met inhoud die beschikbaar is gesteld via Windows Update en Microsoft Update, waaronder beveiligingsupdates, stuurprogramma's en service packs. Door tijdens het zoeken het nummer van het beveiligingsbulletin (bijvoorbeeld “MS07-036”) te gebruiken, kunt u alle beschikbare updates toevoegen aan uw winkelmand (waaronder de verschillende talen voor een update) en de map van uw keuze downloaden. Raadpleeg de [veelgestelde vragen van de Microsoft Windows Update-catalogus](http://go.microsoft.com/fwlink/?linkid=97900) voor meer informatie over de Microsoft Windows Update-catalogus.

**Opmerking** Vanaf 1 augustus 2009 biedt Microsoft niet langer ondersteuning voor Office Update en het Office Update Inventory Tool. Gebruik [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) voor het verkrijgen van de nieuwste updates voor Microsoft Office. Zie [informatie over Microsoft Office Update: Veelgestelde vragen.](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx)

**Richtlijnen voor detecteren en implementeren**

Microsoft biedt zoekfuncties en richtlijnen voor het implementeren van beveiligingsupdates. Deze begeleiding bevat aanbevelingen en informatie die IT-professionals kunnen helpen verschillende hulpprogramma's voor het zoeken naar en toepassen van beveiligingsupdates te gebruiken. Zie [Microsoft Knowledge Base-artikel 961747](http://support.microsoft.com/kb/961747) voor meer informatie.

**Microsoft Baseline Security Analyzer**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders snel en betrouwbaar de nieuwste essentiële updates en beveiligingsupdates implementeren voor Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 tot Windows 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar; zie ook [System Center Configuration Manager 2007.](http://technet.microsoft.com/en-us/library/bb735860.aspx) Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren. Gebruikers van SMS 2.0 kunnen ook met de Security Update Inventory Tool (SUIT) beveiligingsupdates implementeren. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking** SMS maakt gebruik van de Microsoft Baseline Security Analyzer om brede ondersteuning te kunnen bieden voor het zoeken en installeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows-updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Microsoft Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:

Voor informatie over andere releases voor Windows Update en Microsoft Update (geen beveiligingsreleases), verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services. Heeft betrekking op alle Windows-inhoud.
-   [Updates van vorige maanden voor Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965,aspx). Toont alle nieuwe, herziene en opnieuw uitgebrachte updates voor alle Microsoft-producten behalve Microsoft Windows.

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

-   [Matthieu Suiche](http://www.msuiche.net/) van het [Nederlands forensisch instituut](http://www.nederlandsforensischinstituut.nl/) voor het melden van een probleem dat is beschreven in MS09-050
-   Ivan Fratric van [Zero Day Initiative](http://www.zerodayinitiative.com/) en Jun Xie van [McAfee Avert Labs](http://www.avertlabs.com/) voor het melden van een probleem dat is beschreven in MS09-051
-   Vinay Anantharaman van [Adobe Systems, Inc.](http://www.adobe.com/) voor het melden van een probleem dat is beschreven in MS09-051
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS09-052
-   SkyLined van [Google Inc.](http://www.google.com/) voor het melden van een probleem dat wordt beschreven in MS09-054
-   Mark Dowd van [IBM ISS X-Force](http://www.iss.net/) voor het melden van een probleem dat wordt beschreven in MS09-054.
-   [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS09-054
-   Sam Thomas van eshu.co.uk, die bij [TippingPoint](http://www.tippingpoint.com/) werkt, en [Zero Day Initiative](http://www.zerodayinitiative.com/), voor het melden van een probleem dat wordt beschreven in MS09-054
-   Ian Wright en Jean-Luc Giraud van [Citrix](http://www.citrix.com/) voor hun samenwerking met ons aan een probleem dat is beschreven in MS09-056
-   Dan Kaminsky van [IOActive](http://www.ioactive.com/) voor het melden van twee problemen die zijn beschreven in MS09-056
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS09-057
-   Tavis Ormandy en Neel Mehta van [Google Inc.](http://www.google.com/) voor het melden van twee problemen die zijn beschreven in MS09-058
-   [NSFocus Security Team](http://www.nsfocus.com/) voor het melden van een probleem dat wordt beschreven in MS09-058.
-   David Dewey van [IBM ISS X-Force](http://www.iss.net/) voor het melden van een probleem dat wordt beschreven in MS09-060
-   Ryan Smith van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van twee problemen die worden beschreven in MS09-060
-   [Pavel Minaev](http://int19h.org/) voor het melden van een probleem dat wordt beschreven in MS09-061.
-   Jeroen Frijters van [Sumatra](http://www.sumatra.nl/) voor het melden van een probleem dat is beschreven in MS09-061
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS09-062
-   Thomas Garnier van [SkyRecon](http://www.skyrecon.com/) voor het melden van een probleem dat wordt beschreven in MS09-062
-   Wushi van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat is beschreven in MS09-062
-   Ivan Fratric van [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat is beschreven in MS09-062
-   Tavis Ormandy van [Google Inc.](http://www.google.com/) voor het melden van twee problemen die zijn beschreven in MS09-062
-   Carlo Di Dato (ook bekend onder de naam shinnai) voor het melden van een probleem dat wordt beschreven in MS09-062
-   Marsu Pilami van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat is beschreven in MS09-062
-   Carsten H. Eiram van [Secunia](http://secunia.com/) voor het melden van een probleem dat wordt beschreven in MS09-062

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/?ln=nl) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (13 oktober 2009): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (14 oktober 2009): De downloadkoppeling voor Windows XP x64 Edition Service Pack 2 voor MS09-055 is gecorrigeerd.
-   V1.2 (18 oktober 2009): De samenvatting voor MS09-054 is herzien voor Firefox-gebruikers.
-   V2.0 (28 oktober 2009): Microsoft Office Visio Viewer 2007, Microsoft Office Visio Viewer 2007 Service Pack 1 en Microsoft Office Visio Viewer 2007 Service Pack 2 zijn toegevoegd als software waarin dit probleem optreedt voor MS09-062 en er zijn opmerkingen toegevoegd voor MS09-062 voor gebruikers van SQL Server 2005 met een afhankelijkheid van Reporting Services SharePoint.
-   V3.0 (2 november 2009): Bijgewerkt met de vermelding van de beschikbaarheid van een hotfix voor MS09-054 om compatibiliteitsproblemen op te lossen. Klanten die deze update al hebben toegepast, kunnen de hotfix van Microsoft Knowledge Base-artikel 976749 installeren.
-   V3.1 (4 november 2009): Er zijn onjuiste verwijzingen verwijderd naar de oorspronkelijke versie van Microsoft Office Visio Viewer 2007 als software waarin dit probleem optreedt in MS09-060 en MS09-062.
-   V4.0 (10 november 2009): Het bulletin is bijgewerkt met informatie over het opnieuw uitbrengen van de update voor Audiocompressiebeheer op Microsoft Windows 2000 Service Pack 4 in MS09-051 om een detectieprobleem op te lossen. Dit is alleen een detectieverandering. Er zijn geen binaire bestanden gewijzigd. Klanten die hun systemen al hebben bijgewerkt, hoeven deze update niet opnieuw te installeren.
-   V4.1 (12 januari 2010): Microsoft Expression Web, Microsoft Expression Web 2, Microsoft Office Groove 2007 en Microsoft Office Groove 2007 Service Pack 1 zijn verwijderd als software waarin dit probleem optreedt voor MS09-062.
-   V4.2 (22 juni 2010): .NET Framework 1.1 Service Pack 1 is verwijderd als een getroffen onderdeel op Windows 7 en Windows Server 2008 R2 voor MS09-061.

*Built at 2014-04-18T01:50:00Z-07:00*
