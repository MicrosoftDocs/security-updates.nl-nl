---
TOCTitle: 'MS08-APR'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor april 2008'
ms:assetid: 'ms08-apr'
ms:contentKeyID: 61231954
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms08-apr(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor april 2008
===================================================================

Gepubliceerd: dinsdag 8 april 2008 | Bijgewerkt: woensdag 18 februari 2009

**Versie:** 1.3

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor april 2008.

Met de release van de bulletins voor april 2008 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 3 april 2008. Ga voor meer informatie over de vooraankondiging van de bulletins naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 9 april 2008 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van april.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357219&eventcategory=4&culture=en-us&countrycode=us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Kritiek (5)
-----------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-018                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Project kan externe code worden uitgevoerd (950183)**](http://technet.microsoft.com/security/bulletin/ms08-018)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Samenvatting**                          | Deze beveiligingsupdate lost een privé gemeld beveiligingslek in Microsoft Project op waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Project-bestand opent. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-021                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in GDI kan externe code worden uitgevoerd (948590)**](http://technet.microsoft.com/security/bulletin/ms08-021)                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Samenvatting**                          | Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in GDI opgelost. Door misbruik van deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd EMF- of WMF-afbeeldingsbestand opent. Een aanvaller die misbruik weet te maken van het beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                                                                                                                                        |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-022                                                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in scripting engines voor VBScript en JScript kan externe code worden uitgevoerd (944338)**](http://technet.microsoft.com/security/bulletin/ms08-022)                                                                                                                                                                                                                                                              |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in de scripting engines voor VBScript en JScript in Windows opgelost. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                          |
| **Software waarin dit probleem optreedt** | **Microsoft Windows. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                      |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-023                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingsupdate van ActiveX kill-bits (948881)**](http://technet.microsoft.com/security/bulletin/ms08-023)                                                                                                                                                                                                                                                                                                                                                                           |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek voor een Microsoft-product opgelost. Deze update bevat ook een kill-bit voor Yahoo! Music Jukebox. Door dit beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina heeft weergegeven in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Mogelijk moet voor deze update het systeem opnieuw worden gestart.                                                                                                                                                                                                                                                                                                               |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Internet Explorer.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                               |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-024                                                                                                                                                                                                                                                                                                                                                           |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Cumulatieve beveiligingsupdate voor Internet Explorer (947864)**](http://technet.microsoft.com/security/bulletin/ms08-024)                                                                                                                                                                                                                                                                     |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina heeft weergegeven in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                           |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                              |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                             |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Internet Explorer.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                      |

Belangrijk (3)
--------------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-020                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in DNS-clients is spoofing mogelijk (945553)**](http://technet.microsoft.com/security/bulletin/ms08-020)                                                                                                                                                                                                                   |
| **Samenvatting**                          | Door deze update wordt een privé gemeld beveiligingslek opgelost. Dit beveiligingslek met betrekking tot spoofing komt voor in Windows DNS-clients en zou ertoe kunnen leiden dat een aanvaller speciaal vervaardigde antwoorden op DNS-aanvragen verzendt, waarbij internetverkeer van legitieme locaties wordt omgeleid, of onderschept en vervalst. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                             |
| **Gevolgen van het beveiligingslek**      | Spoofing                                                                                                                                                                                                                                                                                                                                               |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                  |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                              |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-025                                                                                                                                                                                                                                                                                                                                       |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in Windows-kernel kan leiden tot misbruik van bevoegdheden (941693)**](http://technet.microsoft.com/security/bulletin/ms08-025)                                                                                                                                                                                                                            |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in de Windows-kernel opgelost. Een lokale aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts maken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                    |
| **Gevolgen van het beveiligingslek**      | Misbruik van bevoegdheden                                                                                                                                                                                                                                                                                                                                                     |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                         |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                     |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-019                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft Visio kan externe code worden uitgevoerd (949032)**](http://technet.microsoft.com/security/bulletin/ms08-019)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Samenvatting**                          | Met deze beveiligingsupdate worden privé gemelde beveiligingslekken in Microsoft Office Visio opgelost waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Visio-bestand opent. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

Software waarin het probleem optreedt en Downloadlocaties
---------------------------------------------------------

<span></span>
**Gebruik van deze tabel**

In deze tabel vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of onderdeel in de tabel controleren of er beveiligingsupdates vereist zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.

**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.

#### Windows-besturingssysteem en -onderdelen

 
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000:</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-021"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-022"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-023"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-024"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-020"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-025"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=caac000a-22b6-48cb-aa00-1a0bfe886de2">Microsoft Windows 2000 Service Pack 4</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.1 en JScript 5.1</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0395451f-b719-4f71-a7b4-403d0c7e8fcc">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=ba6d3aeb-e35a-47cc-bace-7bd9d58a9d3f">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b051ae04-fe81-440d-9136-d6b239ca954e">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=75d2dc78-e3a4-4ff6-9e2d-bf1935003e8e">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=41326ade-96b6-47ce-9291-d4e3039471c4">Microsoft Windows 2000 Service Pack 4</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8db9f328-da0e-4fb8-96c4-6d368b47c224">Microsoft Windows 2000 Service Pack 4</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-021"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-022"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-023"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-024"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-020"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-025"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c2763dd8-a03e-4a48-aa86-a7ec00250a7a">Windows XP Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c0124698-3b94-4474-9473-22a2f39a4a56">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9dbf002f-fe53-4cc7-a430-35f45c520d10">Windows XP Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=36c641ad-953f-4b09-ba1c-9c383295e180">Microsoft Internet Explorer 6</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=e771efe8-8881-4f23-b5b0-15651a390ba9">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=893f4cef-0395-4c44-ba28-7a10b6e7dd48">Windows XP Service Pack 2</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0e937f65-abd0-46dd-8883-5bfd70ea1178">Windows XP Service Pack 2</a><br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=166f2ab5-913c-47a9-86fe-b814797b751e">Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87b80ae3-e299-4d15-a135-3b1bcf943652">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=01400970-df68-4daf-aa39-2fc4f969974c">Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=85beacc0-8ca2-4ded-9c24-23348d05c735">Microsoft Internet Explorer 6</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=9364bf81-6505-4788-958d-a4bd29dc98ad">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8fdd1207-6e93-4c43-bacc-fe3623a6ebe7">Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a29bbd13-761f-44fa-8948-e1a8c244bd7a">Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-021"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-022"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-023"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-024"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-020"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-025"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bee91d80-d49a-4d3d-82d6-d5aa63f54979">Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=88518aa6-e334-4529-aa63-0bf2ef417ce3">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ad384fea-53be-4be3-8acb-1cd23a7f5405">Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2</a><br />
(Gemiddeld)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0444b76e-93fa-43c2-b1bc-a5c054529eb5">Microsoft Internet Explorer 6</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=9acd2a03-5530-49c8-9ea1-0bfaf259700d">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=214bd8f5-6eb2-414c-b013-c516a306d692">Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d3b855a6-4648-4771-826d-11a151828eac">Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2</a><br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e3dde449-e062-4ce0-a9f4-433bff23e224">Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=12cefefc-8553-4dca-9850-c653371de61e">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ffc5c893-cb24-4875-b0a7-6d5c7aa4d642">Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Gemiddeld)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5ebb5ef9-615f-4cab-bac5-6f45f1b94952">Microsoft Internet Explorer 6</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a9e406aa-33e2-49b8-ab54-4a7328e46147">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fd123394-a5d6-4b55-be74-2938f52ce922">Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=320fd100-35e1-4345-9399-796393235cbc">Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7886a802-f2b5-489c-b14b-631f4c4c0742">Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fe22a828-cca4-4b51-bbd5-995c65fead21">VBScript 5.6 en JScript 5.6</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=94cf78d3-b6c3-41bc-993e-3af3be0d70f1">Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen</a><br />
(Gemiddeld)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=63da8040-fda2-42c7-8543-26ad6f9811f2">Microsoft Internet Explorer 6</a><br />
(Kritiek)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=75a05d3a-92a0-4a00-95d4-e2b2f6755180">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e0e63f03-904d-47ee-94fc-51a8dea668eb">Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=126426a7-be38-4327-89db-02d99d76589d">Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-021"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-022"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-023"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-024"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-020"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-025"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista en Windows Vista Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9b51deb8-3873-4146-977f-7e3d0840a4c5">Windows Vista en Windows Vista Service Pack 1</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d7f14001-7f42-4ca0-9193-cdf061179b59">Windows Vista en Windows Vista Service Pack 1</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d4e24966-6530-463a-9ee2-f6a9d000f998">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8203d303-c855-4579-9bbf-b06ddf5c1b87">Windows Vista</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9640cd8b-d749-4ddd-8af9-b298cebed969">Windows Vista en Windows Vista Service Pack 1</a><br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4ad6dcd1-6ea5-43bf-8bee-a5f507beadc6">Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d33462b6-7391-482d-babe-fb4cd0beaa21">Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=295cf8f2-265e-4570-b708-21033337fe05">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=73f3a234-3973-4467-be7e-69efa7ee978c">Windows Vista x64 Edition</a><br />
(Belangrijk)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=d56bb4fe-304e-45e0-95f2-fde2f47b2a04">Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-021"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-022"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-023"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-024"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-020"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-025"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 voor 32-bits systemen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=006d5c47-53e6-4ee1-932c-497611804938">Windows Server 2008 voor 32-bits systemen</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=95691924-2813-4a86-9e11-99d853f8e606">Windows Server 2008 voor 32-bits systemen</a><br />
(Laag)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e57b4d94-19ad-4818-8311-a3f94be01a4b">Windows Internet Explorer 7</a>*<br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4497333c-9418-4b91-83dc-0155735421c0">Windows Server 2008 voor 32-bits systemen</a><br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2008 voor x64-systemen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8909f144-655b-4f07-916f-fd967f1efb2b">Windows Server 2008 voor x64-systemen</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=920ae29b-19d0-4089-ac79-f2da824a2256">Windows Server 2008 voor x64-systemen</a><br />
(Laag)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=93e9f52a-c7d0-4033-9c12-740665a219af">Windows Internet Explorer 7</a>*<br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5aefc7a6-79a4-45a2-b534-35d0ec400dda">Windows Server 2008 voor x64-systemen</a><br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 voor Itanium-systemen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b7771a4a-4e4f-48d1-8551-bb8b778ca5a7">Windows Server 2008 voor Itanium-systemen</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=66df79ac-8364-4922-9688-ebc7ec76d89f">Windows Server 2008 voor Itanium-systemen</a><br />
(Laag)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=acf948e8-c4a9-40da-b282-f5e584e77b05">Windows Internet Explorer 7</a><br />
(Kritiek)</td>
<td style="border:1px solid black;">Geen</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3080c26b-7456-41ef-8668-28f15bc7b8ce">Windows Server 2008 voor Itanium-systemen</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

**\*Windows Server 2008 Server Core-installatie is niet getroffen.** De beveiligingslekken die door deze updates worden verholpen, hebben geen invloed op ondersteunde versies van Windows Server 2008 indien Windows Server 2008 is geïnstalleerd met de Server Core-installatieoptie, ook al zijn er mogelijk bestanden die door deze beveilingslekken zijn getroffen aanwezig op het systeem. Gebruikers die deze bestanden op hun systeem hebben, krijgen deze update toch aangeboden omdat de updatebestanden nieuwer zijn (met hogere versienummers) dan de bestanden die zich momenteel op uw systeem bevinden. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Office-pakketen en -software

 
<table style="border:1px solid black;">
<caption>Microsoft Project</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-018"><strong>MS08-018</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritiek</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2000 Service Release 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=fbe46241-b9da-40c6-803d-42eb6234be77">Project 2000 Service Release 1</a><br />
(KB949043)<br />
(Kritiek)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Project 2002 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=07a90718-6597-426d-9dca-a336d60c01b8">Project 2002 Service Pack 1</a><br />
(KB949005)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aaba07d6-e972-4e85-bccd-406aa2c4a4f4">Project 2003 Service Pack 2</a><br />
(KB948962)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>

 
<table style="border:1px solid black;">
<caption>Microsoft Visio</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-019"><strong>MS08-019</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2002 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0056a936-def5-40fa-bcfc-0ab0dd5c3964">Visio 2002 Service Pack 2</a><br />
(KB947896)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 Service Pack 2</a><br />
(KB947650)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2003 Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 Service Pack 3</a><br />
(KB947650)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2007</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007</a><br />
(KB947590)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2007 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007 Service Pack 1</a><br />
(KB947590)<br />
(Belangrijk)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
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
  
### Overige informatie
  
#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows
  
Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.
  
#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:
  
Voor informatie over releases op Windows Update en Microsoft Update die geen beveiligingsreleases zijn, verwijzen wij u naar:
  
-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services voor 2008. Heeft betrekking op alle Windows-inhoud.  
-   [Nieuwe, herziene en vrijgegeven updates voor Microsoft-producten behalve Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).
  
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
  
-   [National Cyber Security Center](http://www.ncsc.go.kr/eng/) in Korea, voor het melden van het probleem dat wordt beschreven in MS08-018  
-   Een anonieme onderzoeker voor het melden van het probleem dat wordt beschreven in MS08-019  
-   Een anonieme onderzoeker voor het melden van een ander probleem dat wordt beschreven in MS08-019  
-   Amit Klein van [Trusteer](http://www.trusteer.com/) voor het melden van een probleem dat wordt beschreven in MS08-020  
-   Alla Berzroutchko van [Scanit](http://www.scanit.be/) voor het melden van een probleem dat wordt beschreven in MS08-020  
-   Roy Arends van [Nominet UK](http://www.nominet.org.uk/) voor het melden van een probleem dat wordt beschreven in MS08-020  
-   Jun Mao van [iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS08-021  
-   Sebastian Apelt van [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS08-021  
-   Thomas Garnier van [SkyRecon](http://www.skyrecon.com/) voor het melden van een probleem dat wordt beschreven in MS08-021  
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS08-021  
-   Peter Ferrie van [Symantec](http://www.symantec.com/) voor het melden van een probleem dat wordt beschreven in MS08-022  
-   Een anonieme onderzoeker die bij [iDefense VCP](http://labs.idefense.com/vcp/) werkt voor het melden van een probleem dat wordt beschreven in MS08-023  
-   Carsten Eiram van [Secunia](http://secunia.com/) voor het melden van een probleem dat wordt beschreven in MS08-024  
-   Thomas Garnier van [SkyRecon](http://www.skyrecon.com/) voor het melden van een probleem dat wordt beschreven in MS08-025
  
#### Ondersteuning
  
-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.  
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.  
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.
  
#### Uitsluiting van aansprakelijkheid
  
De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.
  
#### Revisies
  
-   V1.0 (8 april 2008): Samenvatting van de gepubliceerde bulletins.  
-   V1.1 (9 april 2008): Samenvatting voor Microsoft-beveiligingsbulletin MS08-018 bijgewerkt.  
-   V1.2 (16 april 2008): Informatie over de ontdekker bijgewerkt voor MS08-021 en Software waarin dit probleem optreedt verduidelijkt voor Microsoft Office-suites en Software.  
-   V1.3 (18 februari 2009): Er is een ongewijzigde Server Core-notatie voor Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor x64-systemen toegevoegd voor MS08-024.
  
*Built at 2014-04-18T01:50:00Z-07:00*
