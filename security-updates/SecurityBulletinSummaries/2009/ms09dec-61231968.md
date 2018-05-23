---
TOCTitle: 'MS09-DEC'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor december 2009'
ms:assetid: 'ms09-dec'
ms:contentKeyID: 61231968
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms09-dec(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor december 2009
======================================================================

Gepubliceerd: dinsdag 8 december 2009 | Bijgewerkt: woensdag 13 januari 2010

**Versie:** 2.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor december 2009.

Met de release van de bulletins voor december 2009 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins, die oorspronkelijk werd uitgegeven op 3 december 2009. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 9 december 2009 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van december](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032407802&culture=en-us). Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

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
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-071">MS09-071</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de Internet Authentication Service kan externe code worden uitgevoerd (974318)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Microsoft Windows opgelost. Door de ernstigste beveiligingslekken kan externe code worden uitgevoerd indien berichten die worden ontvangen door de Internet Authentication Service onjuist worden gekopieerd in het geheugen bij het verwerken van PEAP-verificatiepogingen. Op Windows Server 2008 wordt de Internet Authentication Service vervangen door Network Policy Server (NPS). Een aanvaller die de beveiligingslekken weet te misbruiken, kan volledige controle krijgen over het systeem waarin dit probleem optreedt. Servers met de Internet Authentication Service of Network Policy Server worden alleen getroffen wanneer ze PEAP met MS-CHAP v2-verificatie gebruiken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-074">MS09-074</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in Microsoft Office Project kan externe code worden uitgevoerd (967183)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Office Project opgelost. Dit beveiligingslek kan leiden tot het uitvoeren van externe code als een gebruiker een speciaal vervaardigd Project-bestand opent. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-072">MS09-072</a></td>
<td style="border:1px solid black;"><strong>Cumulatieve beveiligingsupdate voor Internet Explorer (976325)</strong><br />
<br />
Met deze beveiligingsupdate worden vier privé gemelde beveiligingslekken en een openbaar gemaakt beveiligingslek in Internet Explorer opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina weergeeft in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. Door een ActiveX-besturingselement dat is gebouwd met Microsoft Active Template Library-headers (ATL) kan ook externe code worden uitgevoerd; dit beveiligingslek wordt beschreven in Microsoft-beveiligingsadvies 973882 en Microsoft-beveiligingsbulletin MS09-035.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-069">MS09-069</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Local Security Authority Subsystem Service kan leiden tot denial of service (974392)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Het beveiligingslek kan leiden tot denial of service als een externe, geverifieerde aanvaller tijdens communicatie via Internet Protocol Security (IPSec) een speciaal vervaardigd ISAKMP-bericht verzendt naar de Local Security Authority Subsystem Service (LSASS) op een systeem waarop dit probleem optreedt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Denial of service</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-070">MS09-070</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Active Directory Federation Services kan externe code worden uitgevoerd (971726)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Microsoft Windows opgelost. Door het ernstigste beveiligingslek kan externe code worden uitgevoerd indien een aanvaller een speciaal vervaardigde HTTP-aanvraag verzendt naar een ADFS-webserver. Een aanvaller moet een geverifieerde gebruiker zijn om misbruik te kunnen maken van deze beveiligingslekken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-073">MS09-073</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in WordPad- en Office-tekstconversieprogramma's kan externe code worden uitgevoerd (975539)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft WordPad- en Microsoft Office-tekstconversieprogramma's opgelost. Door het beveiligingslek kan externe code worden uitgevoerd indien een speciaal vervaardigd Word 97-bestand wordt geopend in WordPad of Microsoft Office Word. Een aanvaller die misbruik weet te maken van dit beveiligingslek kan dezelfde rechten verwerven als de gebruiker. Gebruikers met accounts waarvoor minder bevoegdheden op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersbevoegdheden werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden vermeld volgens bulletin-id en CVE-id.
  
**Gebruik van deze tabel**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins functionerende exploitatiecode verschijnt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de ernst van het probleem te kunnen vaststellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.
  
| Bulletin-id                                                         | Titel van beveiligingslek                                                                                  | CVE-id                                                                           | Beoordeling van de exploitatie-index                                                                                 | Belangrijke opmerkingen                                                                                                                                                                                                                                                                                             |  
|---------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-069](http://technet.microsoft.com/security/bulletin/ms09-069) | Beveiligingslek in de Local Security Authority Subsystem Service met betrekking tot uitputting van bronnen | [CVE-2009-3675](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3675) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Door het beveiligingslek kan geen externe code worden uitgevoerd maar het beveiligingslek kan wel leiden tot denial of service waarvan een externe, geverifieerde aanvaller misbruik kan proberen te maken.                                                                                                         |  
| [MS09-070](http://technet.microsoft.com/security/bulletin/ms09-070) | Beveiligingslek met betrekking tot Single Sign-On-vervalsing in ADFS                                       | [CVE-2009-2508](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2508) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Door het beveiligingslek kan geen externe code worden uitgevoerd, alleen vervalsing.                                                                                                                                                                                                                                |  
| [MS09-070](http://technet.microsoft.com/security/bulletin/ms09-070) | Beveiligingslek met betrekking tot het uitvoeren van externe code in ADFS                                  | [CVE-2009-2509](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2509) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Alleen een geverifieerde aanvaller kan misbruik maken van het beveiligingslek.                                                                                                                                                                                                                                      |  
| [MS09-071](http://technet.microsoft.com/security/bulletin/ms09-071) | Beveiligingslek in de Internet Authentication Service met betrekking tot geheugenbeschadiging              | [CVE-2009-2505](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2505) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Beperkte mogelijkheid voor het uitvoeren van externe code. Het meest waarschijnlijke resultaat is denial of service.                                                                                                                                                                                                |  
| [MS09-071](http://technet.microsoft.com/security/bulletin/ms09-071) | Beveiligingslek met betrekking tot het negeren van MS-CHAP-verificatie                                     | [CVE-2009-3677](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3677) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Door het beveiligingslek kan geen externe code worden uitgevoerd, maar het beveiligingslek kan wel leiden tot misbruik van bevoegdheden door omzeiling van de netwerkverificatie.                                                                                                                                   |  
| [MS09-072](http://technet.microsoft.com/security/bulletin/ms09-072) | Beveiligingslek met betrekking tot COM-initialisatie in de ATL                                             | [CVE-2009-2493](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2493) | Geen                                                                                                                 | (Aan dit beveiligingslek is reeds een misbruikindexbeoordeling toegewezen in [de samenvatting van het bulletin voor juli](http://technet.microsoft.com/security/bulletin/ms09-jul). Dat komt doordat het beveiligingslek voor het eerst in [MS09-035](http://go.microsoft.com/fwlink/?linkid=158131) is behandeld.) |  
| [MS09-072](http://technet.microsoft.com/security/bulletin/ms09-072) | Beveiligingslek met betrekking tot beschadiging van niet-geïnitialiseerd geheugen                          | [CVE-2009-3671](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3671) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                              |  
| [MS09-072](http://technet.microsoft.com/security/bulletin/ms09-072) | Beveiligingslek met betrekking tot beschadigd geheugen door HTML-objecten                                  | [CVE-2009-3672](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3672) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                              |  
| [MS09-072](http://technet.microsoft.com/security/bulletin/ms09-072) | Beveiligingslek met betrekking tot beschadiging van niet-geïnitialiseerd geheugen                          | [CVE-2009-3673](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3673) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                              |  
| [MS09-072](http://technet.microsoft.com/security/bulletin/ms09-072) | Beveiligingslek met betrekking tot beschadiging van niet-geïnitialiseerd geheugen                          | [CVE-2009-3674](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-3674) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                              |  
| [MS09-073](http://technet.microsoft.com/security/bulletin/ms09-073) | Beveiligingslek met betrekking tot geheugenbeschadiging in het WordPad- en Office-tekstconversieprogramma  | [CVE-2009-2506](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-2506) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                              |  
| [MS09-074](http://technet.microsoft.com/security/bulletin/ms09-074) | Beveiligingslek in Project met betrekking tot geheugenvalidatie                                            | [CVE-2009-0102](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0102) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                              |
  
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
</tr>
<tr>
<th colspan="6">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=5b02d10d-1abd-4d68-826b-71dad543657a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=0cf37247-505a-4dc2-aad7-c8cb1a63b57a)  
(Kritiek)  
[Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7fb6261c-6895-4f79-be2c-bb110874a19c)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=560e01db-5f59-4ef1-9406-f5d7e0fd4128)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=50936f51-b0a9-4e94-85bf-93f9ad74fdd1)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="6">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
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
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4d294be6-19d1-43b5-9c75-f9d30699a2e7)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=facab13f-ea31-4c71-be4c-24e44ded174f)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=def2c038-3b03-4162-a563-a6ebec756f37)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6c003629-77bf-4735-bd4a-c37c4386f869)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=5448b168-6bf7-4bae-9627-b88d76c4d5c5)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c090c4c2-c277-4d8c-91e1-28286bc5443e)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17b5206d-61e9-4663-afc7-80e98bf4d618)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a253c19a-c808-4115-8bd0-cf312d396abd)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=98a56425-4f88-4f0f-963b-dada8dc0d8f8)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0c9af3b5-d015-4025-bbb4-1a5113e9113f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2bbf515-f81a-436b-947b-cbf2db85fdd9)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b9bf156-cd34-460f-b4ad-571e37f54659)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d49b386-133a-4d51-b6f0-cec0c70ef93e)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6659fc40-71ee-44a9-9656-8d3ee02b5bc0)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba030-e2c6-44ac-bb5f-24ae8ec372a2)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0dd50357-64f2-4286-86ba-c512e65eed2a)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a779aae1-7724-4458-94fb-a2343356ecae)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31351b9e-b5bb-4618-990b-1089ea5a3bc2)<sup>[1]</sup>
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9678229-2473-4aae-a814-eca9ea556d17)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a273b47-8a18-4778-9b60-8b560a1ce089)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=287e7921-8aab-42a6-b647-551d0a9adc15)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4de4bbcd-b1b8-4482-8ef7-0d9b4a730e0c)  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e62aba15-5eeb-46a2-a142-bfca94016c55)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8a9bf12-4ad6-49fd-b2b7-f379dc3309d2)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b6eb9d9b-1a43-4b30-a033-19a1db786244)<sup>[2]</sup>
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=257facf3-20a1-49e2-ab4c-c1ae67fe05a0)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=498f5eeb-d03e-42ee-ad6a-9d6f98c66acb)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=9ce1a721-0c6a-4775-9407-9633d817d716)  
(Kritiek)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=72d44de7-dfc5-4667-a59f-2ee73d0e3708)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=f5b003ad-af25-488a-91fb-98835a0bfeac)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=1a7784ef-5d25-4de1-a293-f742b5a3473d)  
(KB973904)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="6">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e4ae4d0-1060-4867-82c5-7e20ea93c2c6)  
(Gemiddeld)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e4ae4d0-1060-4867-82c5-7e20ea93c2c6)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=40d26d40-4203-4013-b3f9-912a5b209fbd)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=47d5ada1-1d60-4233-bdd3-64918b5e1245)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2ca62ea8-67cb-40da-8a65-db6f3607bbab)  
(Gemiddeld)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ca62ea8-67cb-40da-8a65-db6f3607bbab)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3140527a-aa33-462b-b3a6-bfcd78b5aa0c)  
(Kritiek)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1e466b48-422f-4c80-8fdf-ba61111942b1)  
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
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
Geen
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
Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=582a1b15-214e-4f5e-bb5b-95677f4d5968)\*  
(Belangrijk)  
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=582a1b15-214e-4f5e-bb5b-95677f4d5968)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d0570536-756e-4fda-883d-f2a3c4ac5bbd)\*  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=43660133-43e1-41f3-8a82-98c4a739914f)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f6715abb-fd93-44ba-9854-2ecc672622da)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=77e774b4-ec0c-481c-9e93-eee9f44ec71b)\*  
(Belangrijk)  
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=77e774b4-ec0c-481c-9e93-eee9f44ec71b)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0e72d0f1-2ce7-4650-b72c-bb303351aafc)\*  
(Gemiddeld)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=22972970-740f-4c50-93ec-f6d49dd1b360)\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d1f5e9e-a7de-4f96-89c8-510fd51f16e7)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=89defe77-7e82-4bfa-9693-66c93b930da1)  
(Gemiddeld)  
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=89defe77-7e82-4bfa-9693-66c93b930da1)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2c7765a2-3117-4dd8-94b4-0060ca16871b)  
(Gemiddeld)
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
</tr>
<tr>
<th colspan="6">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5af3be0b-2dd2-4039-90e1-2278e9c5aee5)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 voor x64-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9d9a04c8-a019-4943-8e93-c6bfd77c8960)  
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
</tr>
<tr>
<th colspan="6">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-071**](http://technet.microsoft.com/security/bulletin/ms09-071)
</td>
<td style="border:1px solid black;">
[**MS09-072**](http://technet.microsoft.com/security/bulletin/ms09-072)
</td>
<td style="border:1px solid black;">
[**MS09-069**](http://technet.microsoft.com/security/bulletin/ms09-069)
</td>
<td style="border:1px solid black;">
[**MS09-070**](http://technet.microsoft.com/security/bulletin/ms09-070)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
Windows Server 2008 R2 voor x64-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bcb38127-787f-49b0-b3fb-62f6a8628d89)\*  
(Gemiddeld)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2c1b96f2-b3c3-4711-a9ad-b2133ea7bf81)  
(Gemiddeld)
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
</tr>
</table>
 
**Opmerking voor Windows Server 2008 en Windows Server 2008 R2**

**\*De Server Core-installatie wordt niet getroffen door dit beveiligingslek.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de MSDN-artikelen [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) en [Server Core for Windows Server 2008 R2](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**Opmerkingen voor MS09-070**

<sup>[1]</sup> Alleen van toepassing indien bijgewerkt met Windows Server 2003 R2, waarin Active Directory Federation Services is geïmplementeerd.

<sup>[2]</sup> Alleen van toepassing indien bijgewerkt met Windows Server 2003 R2 x64 Edition, waarin Active Directory Federation Services is geïmplementeerd.

**Opmerking voor MS09-073**

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
[**MS09-074**](http://technet.microsoft.com/security/bulletin/ms09-074)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bc3ec3ba-2cec-43ab-b184-c222794231f2)  
(KB975008)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Met Microsoft Office 2003
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b4a4126c-b0b3-4db2-b6f5-0e67519c2a5f)  
(KB975051)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="3">
Overige Microsoft Office-software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-074**](http://technet.microsoft.com/security/bulletin/ms09-074)
</td>
<td style="border:1px solid black;">
[**MS09-073**](http://technet.microsoft.com/security/bulletin/ms09-073)
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
Microsoft Project 2000
</td>
<td style="border:1px solid black;">
[Microsoft Project 2000 Service Release 1](http://www.microsoft.com/downloads/details.aspx?familyid=135c010a-55f4-4385-b67d-96ea06ef881a)  
(KB961083)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Project 2002
</td>
<td style="border:1px solid black;">
[Microsoft Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c55ef8fe-8f66-42fc-a298-de6f8886b3e4)  
(KB961079)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Project 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2ea8ca39-f130-439a-92d5-77e9ef050105)  
(KB961082)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=807426a1-8b78-4681-a606-dc39f4d7b64a)  
(KB977304)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=f3ff8bb6-d047-42f1-9331-b6df85fff9fd)  
(KB974882)  
(Belangrijk)
</td>
</tr>
</table>
 
**Opmerking voor MS09-073**

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

-   Ryan Smith van [Verisign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-072
-   Sam Thomas (http://eshu.co.uk/), die bij [TippingPoint](http://www.tippingpoint.com/) werkt, en [Zero Day Initiative](http://www.zerodayinitiative.com/), voor het melden van een probleem dat wordt beschreven in MS09-072
-   [team509](http://www.team509.com/) in samenwerking met [Verisign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-072
-   Een anonieme onderzoeker die bij [TippingPoint](http://www.tippingpoint.com/) werkt en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS09-072
-   Een anonieme onderzoeker die bij [TippingPoint](http://www.tippingpoint.com/) werkt en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een ander probleem dat wordt beschreven in MS09-072
-   Sean Larsson en Jun Mao van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-073
-   Bing Liu van [FortiGuard Labs van Fortinet](http://www.fortiguard.com/) voor het melden van een probleem dat wordt beschreven in MS09-074

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/?ln=nl) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (8 december 2009): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (9 december 2009): De beschrijving voor MS09-071 in de tabel Samenvattingen is bijgewerkt. De informatie over opnieuw opstarten voor MS09-073 is gecorrigeerd.
-   V2.0 (13 januari 2010): Voor MS09-073 zijn de namen van de updatepakketten **Microsoft Office Word 2002 Service Pack 3 (KB975008)** en **Microsoft Office Word 2003 Service Pack 3 (KB975051)** gewijzigd in respectievelijk **Microsoft Office XP Service Pack 3 (KB975008)** en **Microsoft Office 2003 Service Pack 3 (KB975051)**.

*Built at 2014-04-18T01:50:00Z-07:00*
