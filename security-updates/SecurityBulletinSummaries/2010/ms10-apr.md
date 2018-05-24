---
TOCTitle: 'MS10-APR'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor april 2010'
ms:assetid: 'ms10-apr'
ms:contentKeyID: 61231978
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms10-apr(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor april 2010
===================================================================

Gepubliceerd: dinsdag 13 april 2010 | Bijgewerkt: dinsdag 13 juli 2010

**Versie:** 4.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor april 2010.

Met de release van de bulletins voor april 2010 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 8 april 2010. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 14 april 2010 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van april.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427721&eventcategory=4&culture=en-us&countrycode=us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

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
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-019">MS10-019</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Windows kan externe code worden uitgevoerd (981210)</strong><br />
<br />
Deze update lost twee privé gemelde beveiligingslekken in Windows Authenticode-controle op die uitvoering van externe code kunnen toestaan. Een aanvaller die misbruik weet te maken van deze beveiligingslekken, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de SMB-client kan externe code worden uitgevoerd (980232)</strong><br />
<br />
Met deze beveiligingsupdate worden een openbaar gemaakt beveiligingslek en enkele privé gemelde beveiligingslekken in Microsoft Windows opgelost. Als gevolg van de beveiligingslekken kan externe code worden uitgevoerd indien een aanvaller een speciaal vervaardigde SMB-reactie naar een door de client gestarte SMB-aanvraag heeft verzonden. Om deze beveiligingslekken te misbruiken, moet een aanvaller de gebruiker overhalen om een SMB-verbinding met een speciaal ontworpen SMB-server tot stand te brengen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-025">MS10-025</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Microsoft Windows Media Services kan externe code worden uitgevoerd (980858)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek opgelost in Windows Media Services, uitgevoerd op Microsoft Windows 2000 Server. Door het beveiligingslek kan externe code worden uitgevoerd indien een aanvaller een speciaal vervaardigd transportinformatiepakket verzendt naar een Microsoft Windows 2000-serversysteem waarop Windows Media Services wordt uitgevoerd. Met aanbevolen procedures voor firewalls en standaardfirewallconfiguraties kunt u netwerken beveiligen tegen aanvallen die vanuit het bedrijfsnetwerk komen. Het wordt aanbevolen op de systemen die met internet zijn verbonden zo min mogelijk poorten bloot te stellen aan deze aanvallen. Op Microsoft Windows 2000 Server is Windows Media Services een optioneel onderdeel dat niet standaard is geïnstalleerd.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-026">MS10-026</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Microsoft MPEG Layer-3-codecs kan externe code worden uitgevoerd (977816)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft MPEG Layer-3 audiocodecs opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd AVI-bestand met een MPEG Layer-3-audiostream opent. Als er een gebruiker met beheerdersrechten is aangemeld, kan een aanvaller die misbruik weet te maken van dit beveiligingslek, volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-027">MS10-027</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Windows Media Player kan externe code worden uitgevoerd (979402)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Media Player opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als speciaal vervaardigde mediacontent op een schadelijke website wordt geopend in Windows Media Player. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-021">MS10-021</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (979683)</strong><br />
<br />
Met deze beveiligingsupdate worden enkele privé gemelde beveiligingslekken in Microsoft Windows opgelost. Het meest ernstige beveiligingslek kan leiden tot misbruik van bevoegdheden als een aanvaller zich lokaal aanmeldt en een speciaal vervaardigde toepassing uitvoert. Een aanvaller moet geldige aanmeldingsreferenties hebben en zich lokaal kunnen aanmelden om misbruik te kunnen maken van de beveiligingslekken. De beveiligingslekken kunnen niet vanaf een externe locatie of door anonieme gebruikers worden misbruikt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-022">MS10-022</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in VBScript kan externe code worden uitgevoerd (981169)</strong><br />
<br />
Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek in VBScript op Microsoft Windows opgelost waardoor externe code kan worden uitgevoerd. Het prioriteitsniveau van deze beveiligingsupdate is Belangrijk voor Microsoft Windows 2000, Windows XP en Windows Server 2003. Op Windows Server 2008, Windows Vista, Windows 7 en Windows Server 2008 R2, kan geen misbruik gemaakt worden van de kwetsbare code. Als de code echter voorkomt, wordt deze update verstrekt als een ingrijpende maatregel zonder prioriteitsniveau.<br />
<br />
Door het beveiligingslek kan externe code worden uitgevoerd als een schadelijke website een speciaal vervaardigd dialoogvenster op een webpagina weergeeft en een gebruiker op F1 drukt, zodat Windows Help wordt gestart met een Windows Help-bestand dat door de aanvaller is geleverd. Als er een gebruiker met beheerdersrechten is aangemeld, kan een aanvaller die misbruik weet te maken van dit beveiligingslek, volledige controle krijgen over een systeem waarin dit probleem optreedt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-023">MS10-023</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Microsoft Office Publisher kan externe code worden uitgevoerd (981160)</strong><br />
<br />
Deze beveiligingsupdate lost een privé gemeld beveiligingslek in Microsoft Office Publisher op waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Publisher-bestand opent. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-024">MS10-024</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in Microsoft Exchange en Windows SMTP-service kunnen leiden tot een denial of service (981832)</strong><br />
<br />
Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek en een privé gemeld beveiligingslek in Microsoft Exchange en Windows SMTP-service opgelost. De ernstigere beveiligingslekken kunnen leiden tot een denial of service als een aanvaller een speciaal vervaardigd DNS-antwoord verzendt naar een computer waarop de SMTP-service wordt uitgevoerd. Het SMTP-onderdeel wordt standaard niet geïnstalleerd op Windows Server 2003, Windows Server 2003 x64 Edition of Windows XP Professional x64 Edition.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Denial of service</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Exchange</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-028">MS10-028</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Microsoft Visio kan externe code worden uitgevoerd (980094)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Microsoft Office Visio opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd Visio-bestand opent. Een aanvaller die erin slaagt misbruik te maken van deze beveiligingslekken, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-029">MS10-029</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in het Windows-onderdeel ISATAP is spoofing mogelijk (978338)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Het prioriteitsniveau van deze beveiligingsupdate is Gemiddeld voor Windows XP, Windows Server 2003, Windows Vista en Windows Server 2008. Windows 7 en Windows Server 2008 R2 zijn niet kwetsbaar omdat deze besturingssystemen de functie omvatten die door deze beveiligingsupdate wordt geïmplementeerd.<br />
<br />
Door dit beveiligingslek kan een aanvaller een IPv4-adres vervalsen (spoofen) zodat het adres filters op basis van het IPv4-bronadres kan omzeilen. De beveiligingsupdate lost het beveiligingslek op door de manier te wijzigen waarop de Windows TCP/IP-stack het IPv6-bronadres controleert in een ISATAP-tunnelpakket.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Matig</a><br />
Spoofing</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden genoemd in afnemende volgorde van de mate van misbruik en vervolgens op CVE-id. Alleen beveiligingslekken met het prioriteitsniveau Kritiek of Belangrijk in de bulletins zijn opgenomen.
  
**Gebruik van deze tabel**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins functionerende exploitatiecode verschijnt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de ernst van het probleem te kunnen vaststellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bulletin-id</th>
<th style="border:1px solid black;" >Titel van beveiligingslek</th>
<th style="border:1px solid black;" >CVE-id</th>
<th style="border:1px solid black;" >Beoordeling van de exploitatie-index</th>
<th style="border:1px solid black;" >Belangrijke opmerkingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-021">MS10-021</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot geheugentoewijzing in Windows-kernel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0236">CVE-2010-0236</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-021">MS10-021</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot het maken van een symbolische koppeling in Windows-kernel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0237">CVE-2010-0237</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-028">MS10-028</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot ontregeld geheugen bij het valideren van parameters in Visio</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0254">CVE-2010-0254</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-027">MS10-027</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot uitvoering van externe code in Media Player</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0268">CVE-2010-0268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-025">MS10-025</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot een stack-gebaseerde bufferoverloop in Media Services</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0478">CVE-2010-0478</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-023">MS10-023</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot bufferoverloop door verwerking van bestandsconversietekstvak in Microsoft Office Publisher</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0479">CVE-2010-0479</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-026">MS10-026</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot stack-overloop in de MPEG Layer-3-audiodecoder</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0480">CVE-2010-0480</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-022">MS10-022</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot gebruik van de Help-toets in VBScript</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0483">CVE-2010-0483</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Consistente exploitatiecode is waarschijnlijk<br />
<br />
Voor Windows Server 2008, Windows 7 en Windows Server 2008 R2:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Kans op werkende exploitatiecode is gering</td>
<td style="border:1px solid black;">Dit beveiligingslek is openbaar gemaakt, zoals beschreven in <a href="http://technet.microsoft.com/security/advisory/981169">Microsoft-beveiligingsadvies 981169</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-028">MS10-028</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot ontregeld geheugen bij het berekenen van indexen in Visio</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0256">CVE-2010-0256</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Inconsistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot transacties in de SMB-client</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0270">CVE-2010-0270</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Inconsistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot het parseren van reacties in de SMB-client</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0476">CVE-2010-0476</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Inconsistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-019">MS10-019</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot handtekeningen in WinVerifyTrust</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0486">CVE-2010-0486</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Inconsistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-019">MS10-019</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot beschadigde validatie van Cabview</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0487">CVE-2010-0487</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Inconsistente exploitatiecode is waarschijnlijk</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot onvolledige reactie in de SMB-client</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3676">CVE-2009-3676</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Kans op werkende exploitatiecode is gering</td>
<td style="border:1px solid black;">Dit beveiligingslek is openbaar gemaakt, zoals beschreven in <a href="http://technet.microsoft.com/security/advisory/977544">Microsoft-beveiligingsadvies 977544</a>.<br />
<br />
Het waarschijnlijke gevolg is een denial of service.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-024">MS10-024</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot MX-records in SMTP-servers</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0024">CVE-2010-0024</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Kans op werkende exploitatiecode is gering</td>
<td style="border:1px solid black;">Het waarschijnlijke gevolg is een denial of service</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot geheugentoewijzing in de SMB-client</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0269">CVE-2010-0269</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Kans op werkende exploitatiecode is gering</td>
<td style="border:1px solid black;">(Geen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms10-020">MS10-020</a></td>
<td style="border:1px solid black;">Beveiligingslek met betrekking tot berichtgrootte in de SMB-client</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0477">CVE-2010-0477</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Kans op werkende exploitatiecode is gering</td>
<td style="border:1px solid black;">Het waarschijnlijke gevolg is een denial of service</td>
</tr>
</tbody>
</table>
  
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
</tr>
<tr>
<th colspan="10">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d7538166-35ee-4c6b-be8c-e83a1fc6cd77)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=13846177-f25f-4dd4-9fe9-ac43e1d4d73d)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=67ccac04-e5c8-4381-9d1a-9b676dd516a6)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=73b3d681-26bb-49c1-849e-1f72484cb978)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=f6394fc2-b9d0-46cf-9265-a0d4aeb1448f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=c0b8b362-a321-4ac9-be98-15c71bb7a043)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=c5f4577e-7546-40e9-8bcd-be11c1b260a6)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)<sup>[1]</sup>
(KB981350)  
(Belangrijk)  
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=421be318-f217-4d12-b7a5-833093189073)  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d5fc47a4-cecb-4817-aafb-45f335061be3)  
(KB981349)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=88a0e872-01de-495b-8eec-d105a970daa7)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="10">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=2a01ddf0-f3ea-47c8-ada2-e69f6c1b5f96)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=6c3ac102-2107-4726-98be-4fbf6b858bfb)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dec38c02-3d4a-41c5-8954-e57f56b8fa5b)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=b1582a74-4a7b-4540-beb1-7c89c86eae87)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Media Player 9 Series op Windows XP Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5c748c6d-84d1-45a9-8a33-9372eb5504d5)  
(Kritiek)  
[Windows Media Player 9 Series op Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9e4277b4-2dc5-4163-a6aa-7e07dd32b721)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=142710fd-9cd4-4dd0-aaba-2aace03c008f)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=aa8ff157-a7b3-4787-80c9-5bc453f0f1c9) op Windows XP Service Pack 2  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=cb21d276-65e9-4c8f-96e3-cf6dc36d0133)  
(KB981349)  
(Belangrijk)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=ba7ef6e5-80ba-4281-a611-6e5be008c1b4)  
(KB981332)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=de447b76-ec89-426b-ac54-3ae3855d1159)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9dc3e1c2-2e9d-4d86-9fce-446c409ad613)  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=9bbff00c-f8f4-4a44-98f2-18a868986ae1)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e64e487e-2727-4396-b0c9-6eaf000214d2)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5a21239-a9a3-4ec5-9de8-7d2fc16fc6b8)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=8afca317-a647-44aa-a771-5d85cd5d62ea)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3c0cb02e-3484-4cdf-8c64-c697ad3e2889)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=896c738d-4058-440f-8d4f-16c678610cd1)  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=d7e8b930-8708-4f0b-b22b-961c2cbc2673)  
(KB981349)  
(Belangrijk)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=153fd9c1-0f8e-4492-87d1-f0381e7feb23)  
(KB981332)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f9a696d-2712-4777-a642-e78a38336e8a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d872bd77-f491-4706-8ff5-081ac0bf3d6f)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=0e7e3deb-f078-4953-9642-675ec69267f2)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ae9b1d0-0dbe-4abd-b315-10cea4ceccd7)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1189304f-d626-426d-960c-a86dc2d2b528)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=9f89746c-181e-4177-a851-ec1826e78b6d)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a7ea2d0-61ce-4b68-ad82-d917b1a56f9d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=28b035b8-d56e-4e93-b811-9a82cf1d4ba9)  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=a142a553-85fc-40e0-9426-8d58f6a4333c)  
(KB981349)  
(Belangrijk)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=72754e1b-3d09-4b9d-8794-689c45a37f66)  
(KB981332)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f781e9e4-87d4-4243-9d44-256424d75fec)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd007a6c-04b3-490c-aff4-d5af3e69d477)  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=99a3f6da-728f-421c-ab41-c4c4751934a4)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=1709fd4e-d7c6-4cbb-8b71-a96b8d6eee58)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=52e4f66b-b76c-46a1-aeff-74efa21fc743)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=b97e7ea1-a163-4ce4-8cbc-5f933773c4b2)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1fc66f54-260a-4219-a0b4-056ba9dd0abe)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=339ddf48-8949-4857-9ef6-1ddcc7c5f8b8)  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=a489b4e3-78d2-411b-b27c-5987b8fc91d1)  
(KB981349)  
(Belangrijk)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=72c3013b-f72f-422b-8a89-2246dea4b378)  
(KB981332)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=644ff070-237b-4a73-b2e2-9fffdafa3927)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=19cfddfe-e8da-4564-9730-babfae4a3ebb)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=06832599-1e9b-4792-8c7b-7b5b3a3d6277)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=811a2b28-655d-4b5d-821e-5a90d556dba3)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b2b6d8b1-63cc-459c-b5fa-1355386273c8)  
(Kritiek)
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
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=8dcb8be8-fb78-4518-aa7e-f8b17f7dfb86)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[VBScript 5.6](http://www.microsoft.com/downloads/details.aspx?familyid=9a8bee82-5f7f-490e-a1eb-481f6d4fc4f5)  
(KB981350)  
(Belangrijk)  
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=7d542ac6-8a5b-4dd7-8688-2b5feb563636)  
(KB981349)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=56c8238d-8b04-4aa5-8719-40550cd7325c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=916f1b09-e79e-4347-9fbc-c0cf07de397d)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="10">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Geen
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=a52225a7-6005-4f2b-8291-db20558f23f8)  
(KB978601  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=6145e2b2-36fd-4360-bd5b-2bd11890fc52)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25eeaeb3-c0a3-4a02-9912-acd0342648ba)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=0e7140bb-42d3-48b3-9f4b-d55b17770de8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista](http://www.microsoft.com/downloads/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Belangrijk)  
[Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=86d7b054-af4f-4d8a-9873-cb5246466374)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=ee5c42c6-16bb-48bf-95c2-c188bb17d04b)  
(KB981349)  
(Geen prioriteitsniveau<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f2a37dbf-4a95-4e8d-a474-ecacd9aee690)  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=196055a6-15d1-4da8-b33d-501e69bf5176)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=9ba7468c-23a4-4994-9a5a-22e96ef586f3)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=5b7efa82-0feb-413a-9f8e-212e7432cd99)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=394c1caa-97e4-47a3-9aac-a4a88508bd31)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=b885aef4-3a5d-4c3e-bef6-5efef2965752)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Belangrijk)  
[Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c84aa24-6331-427a-969c-27f7d39db3d7)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=ea5c5e9c-0ecd-47bc-912d-5adc00d1aa21)  
(KB981349)  
(Geen prioriteitsniveau<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=79093796-4ea9-4c6c-92cc-3fd63c5db918)  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c1d1622-1b67-438d-aae4-1a3954974a36)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
Geen
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=97ffeec8-8b6d-4a30-97b0-4bff2ba5e91d)\*  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=f111735b-68b0-4bcc-9dd8-818a5eca3400)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=51c9c420-4507-4911-a8f5-82331a696882)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=8e9c04c9-898f-4ed2-949d-f4343cc0d9f6)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25e3ce7f-53a0-4049-a65c-011d2143c4c2)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=dbe89813-0a45-463b-928c-1e58f7bb596a)\*\*  
(KB981349)  
(Geen prioriteitsniveau<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=527d6376-efc9-436b-835b-219d38bb28f0)\*\*  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e29ead69-000a-4982-a25c-f3981eda381a)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61ece7bc-e9fa-4ede-ba7d-9e5a4c64b9be)\*  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=49f9f740-023a-4291-becf-838a1d282321)\*  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=91c08251-0085-44cb-9e9c-9a1a84374caf)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=61c26a1f-c885-4474-9843-204c41628889)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[MPEG Layer-3-codecs](http://www.microsoft.com/downloads/details.aspx?familyid=d6f2e1ae-48d3-4d2c-b329-32cff00afee5)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b99e54d-955b-4a06-9a04-b2f4596efd72)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=9db62357-557d-40cd-9826-b7baa6c9de65)\*\*  
(KB981349)  
(Geen prioriteitsniveau<sup>[2]</sup>)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=0c384dbc-21b7-4cbc-b68f-ced971d9b791)\*\*  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f922e64-e3a6-46fe-9a81-b2813ea6a330)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=72e7c7ea-55ef-457b-a03a-49aa9dea2e84)\*  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=bd60779a-8bb1-4107-a344-9b09a50e96ff)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=eb116688-1d6e-4e20-948e-1d347af5d985)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bcf8b919-08a9-487f-8dfd-3ca24328c4f3)  
(Kritiek)
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
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1f9746d-61a2-406f-b707-60646bd5b5bb)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.7](http://www.microsoft.com/downloads/details.aspx?familyid=84c5aaae-9417-42a1-834f-22c1ad46a12f)  
(KB981349)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8c48302c-a1d6-41bc-ad24-7ce7332d4842)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="10">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=8d4a6c65-e171-4570-8f3f-118f06910baf)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=f0dbac52-0f0e-40bc-9371-17fa594424d5)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=389184c5-9001-497d-bdf4-81f97ecb617f)  
(Kritiek)
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
[Windows 7 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=ff58d80c-33ce-4d9e-aaa5-0b1841458931)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c3f76835-0053-4e53-a451-14255e7a4fc0)  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
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
[Authenticode-handtekeningcontrole 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=cf8c6721-05c2-4680-93b4-be36f09c6d15)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=b23efe7d-bca4-4d49-9104-6ae39dc5daa9)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=f3495dae-71f3-421d-a191-d26965f26ad1)  
(Kritiek)
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
[Windows 7 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=7f1dc055-2ec9-407a-9e69-da12338587e3)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=998164b7-4b8c-468b-8d39-f242633c8838)  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-019**](http://technet.microsoft.com/security/bulletin/ms10-019)
</td>
<td style="border:1px solid black;">
[**MS10-020**](http://technet.microsoft.com/security/bulletin/ms10-020)
</td>
<td style="border:1px solid black;">
[**MS10-025**](http://technet.microsoft.com/security/bulletin/ms10-025)
</td>
<td style="border:1px solid black;">
[**MS10-026**](http://technet.microsoft.com/security/bulletin/ms10-026)
</td>
<td style="border:1px solid black;">
[**MS10-027**](http://technet.microsoft.com/security/bulletin/ms10-027)
</td>
<td style="border:1px solid black;">
[**MS10-021**](http://technet.microsoft.com/security/bulletin/ms10-021)
</td>
<td style="border:1px solid black;">
[**MS10-022**](http://technet.microsoft.com/security/bulletin/ms10-022)
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
</td>
<td style="border:1px solid black;">
[**MS10-029**](http://technet.microsoft.com/security/bulletin/ms10-029)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=94dfdaae-8464-4de6-a401-7eb70b3bb34f)\*  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=a2979c02-2a80-4b84-bf6c-4798064bdf28)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=cd1a046e-915d-4904-b753-5a24be10c504)\*  
(Kritiek)
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
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=28389c1d-2a12-4bef-a59b-726bb6449c8b)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=c4039d40-a0c7-4183-ab50-04f690d1c5dc)\*\*  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=eb27cd2b-d514-4405-8650-259a42e35155)\*\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Authenticode-handtekeningcontrole 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=40f622d2-48e7-4eb2-9430-bbd218cb5208)  
(KB978601)  
(Kritiek)  
[Shell-extensie Cab-bestandsviewer 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=5e416d4b-5de7-4688-80c6-245de159e0ce)  
(KB979309)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=541e9e2f-ec1d-42b2-aae5-481c0d435169)  
(Kritiek)
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
[Windows Server 2008 R2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=d4ea3984-5183-47f1-814e-29cb6c90ae06)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=8174463c-5c5e-4095-90c8-fd1e898d4ba5)  
(KB981332)  
(Geen prioriteitsniveau<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
</table>
 
**Opmerkingen voor Windows Server 2008 en Windows Server 2008 R2**

**\*Treedt op bij Server Core-installatie.** Deze update is met hetzelfde prioriteitsniveau van toepassing op ondersteunde edities van Windows Server 2008 en Windows Server 2008 R2, zoals is aangegeven, ongeacht of deze zijn geïnstalleerd met de optie Server Core-installatie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Server Core-installatie niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Opmerkingen voor MS10-022**

<sup>[1]</sup>Deze beveiligingsupdate voert een upgrade van uw installatie van VBScript 5.1 uit naar VBScript 5.6.

<sup>[2]</sup>Op deze update zijn geen prioriteitsniveaus van toepassing omdat het beveiligingslek dat wordt besproken in dit bulletin niet optreedt in deze software. Microsoft raadt gebruikers van deze software echter aan deze beveiligingsupdate toe te passen, als een grondige beschermingsmaatregel tegen mogelijke nieuwe aanvalsvectoren in de toekomst.

**Opmerking voor MS10-024**

Zie ook andere softwarecategorieën onder deze sectie, **Software waarin dit probleem optreedt en downloadlocaties** voor meer updatebestanden onder hetzelfde identificatienummer van het bulletin. Dit bulletin geldt voor meerdere softwarecategorieën.

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
[**MS10-023**](http://technet.microsoft.com/security/bulletin/ms10-023)
</td>
<td style="border:1px solid black;">
[**MS10-028**](http://technet.microsoft.com/security/bulletin/ms10-028)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=943b3830-70d5-46c5-bffc-1b494434b5f7)  
(KB980466)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2d563cbc-d8f7-486b-8c54-25d168085376)  
(KB979364)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Met Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7c2f4610-77bb-4d72-847b-1a06c523b137)  
(KB980469)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=803a7ea0-a9da-46dd-9548-0177d3774be7)  
(KB979356)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office System
</td>
<td style="border:1px solid black;">
[Microsoft Office Publisher 2007 Service Pack 1 en Microsoft Office Publisher 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10ca2f71-0ab2-4344-b7fd-bbbd6a783a96)  
(KB980470)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2007 Service Pack 1 en Microsoft Office Visio 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=56fe020f-4444-4a43-aa98-e99a622f6a69)  
(KB979365)  
(Belangrijk)
</td>
</tr>
</table>
 

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
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS10-024**](http://technet.microsoft.com/security/bulletin/ms10-024)
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
Microsoft Exchange Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e47c90a0-c9c8-43b7-bec7-34107ddde294)  
(KB976703)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2003
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc8391f8-5335-496b-ad4c-bae38509be4a)  
(KB976702)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 1 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=6a894b4e-12b6-4a91-9555-d813956b6aac)  
(KB981407)  
(Geen prioriteitsniveau<sup>[1]</sup>)  
[Microsoft Exchange Server 2007 Service Pack 2 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b8f7f872-16d5-49d6-9867-adc01351c06f)  
(KB981383)  
(Geen prioriteitsniveau<sup>[1]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2010 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=7dcf2390-dff7-4e3a-acca-03f4d43fb79a)  
(KB981401)  
(Geen prioriteitsniveau<sup>[1]</sup>)
</td>
</tr>
</table>
 
**Opmerkingen voor MS10-024**

<sup>[1]</sup>Op deze update zijn geen prioriteitsniveaus van toepassing omdat het beveiligingslek dat wordt besproken in dit bulletin niet optreedt in deze software. Microsoft raadt klanten van deze software echter aan deze update toe te passen. Deze bevat een ingrijpende maatregel die extra bronpoortentropie toevoegt aan DNS-transacties die zijn gestart door de SMTP-service.

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

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders de nieuwste essentiële updates en beveiligingsupdates snel en betrouwbaar implementeren voor Microsoft Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 voor Microsoft Windows-besturingssysteem Windows 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar; zie ook [System Center Configuration Manager 2007.](http://technet.microsoft.com/en-us/library/bb735860.aspx) Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren. Gebruikers van SMS 2.0 kunnen ook met de Security Update Inventory Tool (SUIT) beveiligingsupdates implementeren. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking** SMS maakt gebruik van de Microsoft Baseline Security Analyzer om brede ondersteuning te kunnen bieden voor het zoeken en installeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool (die deel uitmaakt van het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)) gebruiken.

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

-   Mark Rabinovich van [Visuality Systems Ltd.](http://www.visualitynq.com/) voor het melden van een probleem dat wordt beschreven in MS10-020
-   Laurent Gaffié van [stratsec](http://www.stratsec.net/) voor het melden van een probleem dat wordt beschreven in MS10-020
-   Matthew 'j00ru' Jurczyk en Gynvael Coldwind van [Hispasec](http://www.hispasec.com/) [Virustotal](http://www.virustotal.com/) voor het melden van vijf problemen die worden beschreven in MS10-021
-   Tavis Ormandy van [Google, Inc.](http://www.google.com/) voor het melden van twee problemen die worden beschreven in MS10-021
-   Martin Tofall van [Obsidium Software](http://www.obsidium.de/) voor het melden van een probleem dat wordt beschreven in MS10-021
-   Lionel d'Hauenens, werkzaam bij [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/) voor het melden van een probleem dat wordt beschreven in MS10-023
-   Fabien Perigaud van [CERT-LEXSI](http://cert.lexsi.com/) voor het melden van een probleem dat wordt beschreven in MS10-025
-   Fabien Perigaud van [CERT-LEXSI](http://cert.lexsi.com/), het [VUPEN Vulnerability Research Team](http://www.vupen.com/)en het Vulnerability Research Team, [TELUS Security Labs](http://telussecuritylabs.com/), [Core Security Technologies](http://www.coresecurity.com/) en het [NSFOCUS Security Team](http://www.nsfocus.com/) voor de samenwerking en het verstrekken van details van een kwaliteitsprobleem in de oorspronkelijke beveiligingsupdate voor MS10-025
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS10-026
-   Een anonieme onderzoeker, werkzaam bij [Zero Day Initiative](http://www.zerodayinitiative.com/) van [TippingPoint](http://www.tippingpoint.com/) voor het melden van een probleem dat wordt beschreven in MS10-027
-   Bing Liu van [FortiGuard Labs](http://www.fortiguard.com/) van Fortinet voor het melden van twee problemen die worden beschreven in MS10-028
-   Gabi Nakibly van het National EW Research & Simulation Center (in Rafael) voor het melden van een probleem dat wordt beschreven in MS10-029

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (13 april 2010): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (14 april 2010): De opstartvereisten voor MS10-025 in de sectie **Samenvattingen** zijn gecorrigeerd. Ook is de Server Core-notatie voor Windows Server 2008 en Windows Server 2008 R2 aangepast en nu alleen nog van toepassing op de update KB978601 voor MS10-019.
-   V2.0 (21 april 2010): Herzien om klanten te melden dat de oorspronkelijke beveiligingsupdate voor MS10-025 systemen niet heeft beschermd tegen het beveiligingslek dat in het bulletin werd beschreven. Microsoft raadt klanten aan een van de tijdelijke oplossingen toe te passen die in MS10-025 worden beschreven om de gevolgen voor de getroffen systemen te beperken tot er een herziene beveiligingsupdate beschikbaar is.
-   V3.0 (27 april 2010): Gewijzigd om de opnieuw uitgebrachte beveiligingsupdate voor MS10-025 aan te bieden.
-   V4.0 (13 juli 2010): Herzien om de opnieuw uitgebrachte beveiligingsupdate voor Windows Server 2008 en Windows Server 2008 R2 voor MS10-024 aan te bieden.

*Built at 2014-04-18T01:50:00Z-07:00*
