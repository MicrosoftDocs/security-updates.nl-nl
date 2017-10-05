---
TOCTitle: 'MS08-AUG'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor augustus 2008'
ms:assetid: 'ms08-aug'
ms:contentKeyID: 61231955
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms08-aug(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor augustus 2008
======================================================================

Gepubliceerd: dinsdag 12 augustus 2008 | Bijgewerkt: woensdag 15 oktober 2008

**Versie:** 3.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor augustus 2008.

Met de release van de bulletins voor augustus 2008 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 7 augustus 2008. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 13 augustus 2008 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van augustus.](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374631&culture=en-us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Kritiek (6)
-----------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-046                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Een beveiligingslek in het Microsoft Windows Image Color Management System kan uitvoering van externe code mogelijk maken (952954)**](http://technet.microsoft.com/security/bulletin/ms08-046)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Samenvatting**                          | Deze update lost een privé gemeld beveiligingslek in het Microsoft Image Color Management (ICM) op dat uitvoering van externe code in de context van de huidige gebruiker kon toestaan. Als er een gebruiker met beheerdersrechten is aangemeld, kan een aanvaller die misbruik weet te maken van dit beveiligingslek, volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-045                                                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Cumulatieve beveiligingsupdate voor Internet Explorer (953838)**](http://technet.microsoft.com/security/bulletin/ms08-045)                                                                                                                                                                                                                                                                                                                  |
| **Samenvatting**                          | Met deze beveiligingsupdate worden vijf privé gemelde beveiligingslekken en een openbaar gemaakt beveiligingslek opgelost. Door al deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina weergeeft in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                          |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Internet Explorer.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                   |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in het ActiveX-besturingselement voor de Microsoft Access Snapshot Viewer kan externe code worden uitgevoerd (955617)**](http://technet.microsoft.com/security/bulletin/ms08-041)                                                                                                                                                                                                                                                                                                            |
| **Samenvatting**                          | Deze beveiligingsupdate lost een privé gemeld beveiligingslek in het ActiveX-besturingselement voor de Snapshot Viewer voor Microsoft Access op. Een aanvaller kan het beveiligingslek misbruiken door een speciaal ontworpen webpagina te maken. Als een gebruiker die webpagina bekijkt, kan via het beveiligingslek code vanaf een externe locatie worden uitgevoerd. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                             |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                 |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-043                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft Excel kan externe code worden uitgevoerd (954066)**](http://technet.microsoft.com/security/bulletin/ms08-043)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Samenvatting**                          | Met deze beveiligingsupdate worden vier privé gemelde beveiligingslekken in Microsoft Office Excel opgelost waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Excel-bestand opent. Een aanvaller die misbruik weet te maken van het beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-051                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft PowerPoint kan externe code worden uitgevoerd (949785)**](http://technet.microsoft.com/security/bulletin/ms08-051)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Samenvatting**                          | Deze beveiligingsupdate lost drie privé gemelde beveiligingslekken in Microsoft Office PowerPoint en Microsoft Office PowerPoint Viewer op die uitvoering van externe code kunnen toestaan indien een gebruiker een speciaal vervaardigd PowerPoint-bestand opent. Een aanvaller die de beveiligingslekken weet te misbruiken, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-044                                                                                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft Office-filters kan externe code worden uitgevoerd (924090)**](http://technet.microsoft.com/security/bulletin/ms08-044)                                                                                                                                                                                                                                              |
| **Samenvatting**                          | Met deze beveiligingsupdate worden vijf privé gemelde beveiligingslekken opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen afbeeldingsbestand weergeeft in Microsoft Office. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                     |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                        |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                    |

Belangrijk (5)
--------------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-047                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in IPsec-beleidverwerking kan leiden tot vrijgeven van informatie (953733)**](http://technet.microsoft.com/security/bulletin/ms08-047)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Samenvatting**                          | Deze update lost een privé gemeld beveiligingslek op in de manier waarop bepaalde Windows IPsec-regels (Internet Protocol Security) worden toegepast. Door dit beveiligingslek kunnen systemen worden ingesteld op het negeren van IPsec-beleid en het uitzenden van netwerkverkeer in leesbare tekst. Dit zou tot gevolg kunnen hebben dat informatie wordt vrijgegeven op het netwerk die gecodeerd had moeten worden. Een aanvaller die het verkeer op het netwerk weergeeft, zou de inhoud van het verkeer kunnen zien en wijzigen. Het beveiligingslek betreft een 'denial-of-service'-probleem. Een aanvaller kan geen code uitvoeren of zichzelf rechtstreeks gebruikersrechten toekennen. Hiermee kan informatie worden achterhaald die verder kan worden misbruikt om het systeem of het netwerk waarin dit probleem optreedt schade toe te brengen. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Gevolgen van het beveiligingslek**      | Vrijgeven van informatie                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-049                                                                                                                                                                                                                                                                                                                                                                                                           |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in het gebeurtenissysteem kan externe code worden uitgevoerd (950974)**](http://technet.microsoft.com/security/bulletin/ms08-049)                                                                                                                                                                                                                                                                                      |
| **Samenvatting**                          | Deze update lost twee privé gemelde beveiligingslekken in Microsoft Windows Event System op die uitvoering van externe code kunnen toestaan. Een aanvaller die misbruik weet te maken van het beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige beheerdersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                             |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                         |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-048                                                                                                                                                                                                                                                                                                                                                                         |
|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingsupdate voor Outlook Express en Windows Mail (951066)**](http://technet.microsoft.com/security/bulletin/ms08-048)                                                                                                                                                                                                                                                                                 |
| **Samenvatting**                          | Deze beveiligingsupdate lost een privé gemeld beveiligingslek in Outlook Express en Windows Mail op. Door dit beveiligingslek kan informatie worden vrijgegeven als een gebruiker een speciaal ontworpen webpagina bezoekt met Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                      |
| **Gevolgen van het beveiligingslek**      | Vrijgeven van informatie                                                                                                                                                                                                                                                                                                                                                                                        |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Mogelijk moet voor deze update het systeem opnieuw worden gestart.                                                                                                                                                                                                                                    |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Outlook Express, Windows Mail.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                        |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-050                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in Windows Messenger kan leiden tot vrijgeven van informatie (955702)**](http://technet.microsoft.com/security/bulletin/ms08-050)                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Samenvatting**                          | Deze beveiligingsupdate lost een openbaar gemeld beveiligingslek in ondersteunde versies van Windows Messenger op. Tengevolge van dit beveiligingslek kan met een script van een ActiveX-besturingselement informatie onrechtmatig worden vrijgegeven in de context van de aangemelde gebruiker. Een aanvaller kan de status wijzigen, contactinformatie verkrijgen en audio- en video-chatsessies starten zonder dat de aangemelde gebruiker dit weet. Een aanvaller kan ook de aanmeldings-ID van de gebruiker verkrijgen en extern aanmelden op de Messenger-client die de gebruiker imiteert. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Vrijgeven van informatie                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Detectie**                              | Microsoft Baseline Security Analyzer kan bespeuren of op uw computersysteem deze update alleen is vereist voor Windows Messenger 4.7 op ondersteunde edities van Windows XP. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                                                                                                          |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Windows Messenger.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-042                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Word kan externe code worden uitgevoerd (955048)**](http://technet.microsoft.com/security/bulletin/ms08-042)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek voor Microsoft Word opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd Word-bestand opent. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Software waarin dit probleem optreedt** | **Microsoft Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

Software waarin het probleem optreedt en Downloadlocaties
---------------------------------------------------------

<span></span>
**Gebruik van deze tabel**

In deze tabel vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of onderdeel in de tabel controleren of er beveiligingsupdates vereist zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.

**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.

#### Windows-besturingssysteem

 
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
</tr>
<tr>
<th colspan="7">
Microsoft Windows 2000:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://technet.microsoft.com/security/bulletin/ms08-046)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://technet.microsoft.com/security/bulletin/ms08-045)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://technet.microsoft.com/security/bulletin/ms08-047)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://technet.microsoft.com/security/bulletin/ms08-049)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://technet.microsoft.com/security/bulletin/ms08-048)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://technet.microsoft.com/security/bulletin/ms08-050)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=db455d17-435f-46d7-b2dd-5babb5a1eeb3)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1557b93b-ecba-4f42-b89d-db0ee067d65b)  
(Kritiek)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa780735-5928-4c46-89a4-63a814954796)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=1b2ad648-7dc9-407a-99f6-f39922746027)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 5.5 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6257bfae-35f0-4c0e-b960-bca7aa6f86f7)  
(Belangrijk)  
[Microsoft Outlook Express 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dab178f7-c282-41f4-acb1-a86e6aa4c91b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://technet.microsoft.com/security/bulletin/ms08-046)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://technet.microsoft.com/security/bulletin/ms08-045)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://technet.microsoft.com/security/bulletin/ms08-047)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://technet.microsoft.com/security/bulletin/ms08-049)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://technet.microsoft.com/security/bulletin/ms08-048)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://technet.microsoft.com/security/bulletin/ms08-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d313f42c-f43f-48ea-82ef-3bc33077c7fa)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=69af2f30-138e-4b15-ab8d-4fce44cc0bc2)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8e2125c7-52cb-4052-82a3-2d3c6a953752)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=01a34aa4-a456-4efc-a93a-c3c682b0181c)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=91469f2f-461c-4a67-8738-d42520427f6b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=8f588f7e-c4ed-42a0-b157-54b1eda60474)  
(KB946648)  
(Belangrijk)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3150c6b8-f50b-4b84-a7ce-c8daf77c080c)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4780b89e-9735-4d3f-8def-34e7337ff604)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=39b41e4b-3237-409d-a818-ab0517c5e7cf)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=246b2686-e330-47a2-b4d4-68f218ad4021)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=2220aece-79d2-426f-90ec-24a17470567a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=a5fc5457-832f-4ee8-be60-4cc8518d1c10)  
(KB946648)  
(Belangrijk)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://technet.microsoft.com/security/bulletin/ms08-046)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://technet.microsoft.com/security/bulletin/ms08-045)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://technet.microsoft.com/security/bulletin/ms08-047)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://technet.microsoft.com/security/bulletin/ms08-049)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://technet.microsoft.com/security/bulletin/ms08-048)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://technet.microsoft.com/security/bulletin/ms08-050)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=828d8fdc-8534-4621-85a5-08aec255496f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0617a5dd-dce9-4de0-b0a0-ce38efe13524)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3c2e2fd-1cb9-491b-937c-053dd59a65bf)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=92a3d08f-c117-4b24-bc78-2b913d270df6)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=30f2244a-f6fd-4fc1-a871-abf6958cb660)  
(Laag)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=302315a8-ccb2-47c2-9104-b8e1d1f49aa0)  
(KB954723)  
(Gemiddeld)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0a13776f-d543-41df-b904-d51e368c81cc)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=32a63f52-9fe6-48e3-bb4e-7d4dda5e0a90)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88a26b76-f7df-45c9-8ed0-7d3cd71c1987)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6bfbb6d8-5106-4adf-83cb-35ffc6e8eaf8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=3287f006-cbb2-4c6d-820c-32833e08035a)  
(Laag)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=be94d138-7d7b-489e-baa6-e214950be6b9)  
(KB954723)  
(Gemiddeld)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=9566493f-4260-4072-947a-527887d2cd63)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1855997e-a3be-46b1-a0bc-bb55eb0045fe)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=97d0d37d-5d76-4bc3-8cbd-1e3976c82acf)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=45356565-697f-41b3-9879-3edd11dbcb7e)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Outlook Express 6](http://www.microsoft.com/downloads/details.aspx?familyid=c8570e40-355b-4a9b-933d-53ae021cbda5)  
(Laag)
</td>
<td style="border:1px solid black;">
[Windows Messenger 4.7](http://www.microsoft.com/downloads/details.aspx?familyid=e4b72618-536b-4a21-bd91-d91be9ca24e5)  
(KB954723)  
(Gemiddeld)  
[Windows Messenger 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=a8d9eb73-5f8c-4b9a-940f-9157a3b3d774)  
(KB899283)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://technet.microsoft.com/security/bulletin/ms08-046)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://technet.microsoft.com/security/bulletin/ms08-045)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://technet.microsoft.com/security/bulletin/ms08-047)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://technet.microsoft.com/security/bulletin/ms08-049)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://technet.microsoft.com/security/bulletin/ms08-048)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://technet.microsoft.com/security/bulletin/ms08-050)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista en Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=13cba012-dd20-48f9-8e44-e4cb104c4cad)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f21a8a2-9861-4fef-9d1e-caf5f7822c1a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6418c78f-f008-4028-beb1-5a5ea8e797a1)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=3851bcf8-f971-4d38-b27f-97396854aac0)  
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
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ead919c2-d548-47b7-9cd6-80f991266428)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa04a754-fbfb-42a7-89d2-14373e3f4742)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e03ccfb0-3ea3-4c59-adcf-9882d7086013)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=3bf7eb8a-b347-4661-be2d-682adc713769)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-046**](http://technet.microsoft.com/security/bulletin/ms08-046)
</td>
<td style="border:1px solid black;">
[**MS08-045**](http://technet.microsoft.com/security/bulletin/ms08-045)
</td>
<td style="border:1px solid black;">
[**MS08-047**](http://technet.microsoft.com/security/bulletin/ms08-047)
</td>
<td style="border:1px solid black;">
[**MS08-049**](http://technet.microsoft.com/security/bulletin/ms08-049)
</td>
<td style="border:1px solid black;">
[**MS08-048**](http://technet.microsoft.com/security/bulletin/ms08-048)
</td>
<td style="border:1px solid black;">
[**MS08-050**](http://technet.microsoft.com/security/bulletin/ms08-050)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b52ff2f-d2f5-4c20-b6cf-86d86c56b0f8)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=c3363df6-39dc-4910-9ce5-66553155378e)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=0640f95e-1eee-4dd1-b4dd-2b82b7e984b9)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=dc3c4b63-acd3-4469-8d47-e0562d99ee65)\*\*  
(Laag)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=df9814a6-5be0-4ac1-a767-a0eae8d5ee5d)\*\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=39dd1722-412b-469d-a475-b6513764838c)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=51a93538-5e94-4f81-a6e0-d497a7b4899d)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=5f973f54-2322-4b41-8c1a-3e712c0da8ae)\*\*  
(Laag)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ffc3cfcb-73fe-4a6d-9595-e9d7a5b3d3f7)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=e9c6cd46-30ad-46ee-9c8b-d0b446e660c4)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=390da130-749d-4890-aad7-be91e15b32bb)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Mail](http://www.microsoft.com/downloads/details.aspx?familyid=9226cd85-1445-4976-a126-757c5d142ffd)  
(Laag)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
</table>
 
**\*Windows Server 2008 Server Core-installatie is getroffen.** Voor ondersteunde edities van Windows Server 2008 is deze update van toepassing met hetzelfde prioriteitsniveau, ongeacht of Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 Server Core-installatie is niet getroffen.** Het beveiligingslek dat wordt beschreven in deze update heeft geen invloed op ondersteunde edities van Windows Server 2008 als Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Office-pakketen en -software

 
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
Microsoft Office-pakketten, -systemen en -onderdelen
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://technet.microsoft.com/security/bulletin/ms08-041)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://technet.microsoft.com/security/bulletin/ms08-043)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://technet.microsoft.com/security/bulletin/ms08-051)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://technet.microsoft.com/security/bulletin/ms08-044)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://technet.microsoft.com/security/bulletin/ms08-042)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8
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
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=458985c3-9c6f-4049-81cd-0d0389c81f11)  
(KB955428)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=54e4031d-298f-480c-88d5-0ad3b2b62ba9)  
(KB955441)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf8688e-e5b9-4e53-a1a1-8cf1acfdb80b)  
(KB951582)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7c044d8-778a-4985-b25b-4f7f6e4abadd)  
(KB949007)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3ab323ec-9f92-453c-b7c7-9a95a9efcaea)  
(KB921595)  
(Kritiek)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=34b655f8-1922-4246-94ca-ed381c3e3b13)  
(KB955440)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9bbf7550-f5c4-4b9b-bd86-1e7be6c42eb5)  
(KB951551)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f8921074-7985-4d42-ac2b-d2f3b1d466ba)  
(KB948995)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c7146dfc-e1be-4d13-877b-1d9bcacc4a64)  
(KB954463)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 en Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Access 2003 Service Pack 2 en Microsoft Office Access 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fd698517-a504-427d-9e5f-fde8f102142c)  
(KB955439)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Excel 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Belangrijk)  
[Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fc612e9a-bdf3-4952-8ada-0de5a50973f0)  
(KB951548)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*  
(KB948988)  
(Belangrijk)  
[Microsoft Office PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7a7c21f0-5e0e-4dee-9710-1ce3d565913f)\*\*  
(KB948988)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0df2f6e-1102-461d-829f-5f3e2d7eb4b3)  
(KB921598)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Belangrijk)  
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=13a37b76-9fec-426f-8176-3c95f934efe0)  
(KB954464)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office System en 2007 Microsoft Office System Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Belangrijk)  
[Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2753e8d6-e156-49ef-af2d-4c521c808ffd)  
(KB951546)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
(Belangrijk)  
[Microsoft Office PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd618a-e9c5-4f1e-b9a5-b2e47ec98ef1)  
(KB951338)  
(Belangrijk)
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
Overige Office-software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://technet.microsoft.com/security/bulletin/ms08-041)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://technet.microsoft.com/security/bulletin/ms08-043)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://technet.microsoft.com/security/bulletin/ms08-051)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://technet.microsoft.com/security/bulletin/ms08-044)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://technet.microsoft.com/security/bulletin/ms08-042)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project 2002 Service Pack 1
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
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bf566ce6-23da-45e5-9c2b-c47331d30e79)  
(KB921596)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SnapShot Viewer voor Microsoft Access
</td>
<td style="border:1px solid black;">
[SnapShot Viewer voor Microsoft Access](http://www.microsoft.com/downloads/details.aspx?familyid=7c22bb32-7ce3-4ff2-8366-ba2eb5135833)  
(KB957198)  
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
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office PowerPoint Viewer 2003
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=911c8872-dec8-4b8e-9708-93dcabd3e036)  
(KB949041)  
(Belangrijk)
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
Microsoft Office Excel Viewer 2003 en Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
(Belangrijk)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d7ed9e75-15f2-4950-98b3-93023ba0f4c1)  
(KB951589)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=b574d906-7f09-49b0-80bf-e84dee8c4583)  
(KB955472)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Converter Pack
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
[Microsoft Office Converter Pack](http://www.microsoft.com/downloads/details.aspx?familyid=199b08c7-6d79-4930-8f0c-31034629c485)  
(KB925256)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 en Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Belangrijk)  
[Service Pack 1 voor het Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=7afdae9b-9c74-4af7-9844-0e54221ea3b9)  
(KB951596)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f)(KB954038)  
(Belangrijk)  
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=84ce5d58-0010-4945-bce9-67a41f898f2f) (KB954038)  
(Belangrijk)
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
Microsoft Office SharePoint Server 2007 en Microsoft Office SharePoint Server 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*  
(KB953397)  
(Belangrijk)  
[Microsoft Office SharePoint Server 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7731749-b026-4765-808a-e151b990f0e1)\*  
(KB953397)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 x64 Edition en Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*  
(KB953397)  
(Belangrijk)  
[Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fc95ab88-2d31-44e1-a702-7cb10e83695b)\*  
(KB953397)  
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
</tr>
<tr>
<th colspan="6">
Microsoft Office voor Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-041**](http://technet.microsoft.com/security/bulletin/ms08-041)
</td>
<td style="border:1px solid black;">
[**MS08-043**](http://technet.microsoft.com/security/bulletin/ms08-043)
</td>
<td style="border:1px solid black;">
[**MS08-051**](http://technet.microsoft.com/security/bulletin/ms08-051)
</td>
<td style="border:1px solid black;">
[**MS08-044**](http://technet.microsoft.com/security/bulletin/ms08-044)
</td>
<td style="border:1px solid black;">
[**MS08-042**](http://technet.microsoft.com/security/bulletin/ms08-042)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 voor Mac
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=ebd3af0c-3f62-4d18-bf45-881655683bd5)  
(KB956343)  
(Belangrijk)
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
Microsoft Office 2008 voor Mac
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9515c70d-be80-4ade-856a-ea542f7d84e1)  
(KB956344)  
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
</tr>
</table>
 
**\*Opmerking voor Microsoft Office SharePoint Server 2007, Microsoft Office SharePoint Server 2007 Service Pack 1, Microsoft Office SharePoint Server 2007 x64 Edition en Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1 (MS08-043):** De update in het beveiligingsbulletin MS08-043 geldt voor servers waarop Excel Services is geïnstalleerd, zoals de standaardconfiguratie van Microsoft Office SharePoint Server 2007 Enterprise en Microsoft Office SharePoint Server 2007 for Internet Sites. Microsoft Office SharePoint Server 2007 Standard wordt zonder Excel Services geleverd.

**\*\*Opmerking voor Microsoft Office PowerPoint 2003 Service Pack 2 en Microsoft Office PowerPoint 2003 Service Pack 3 (MS08-051):** Microsoft heeft nieuwe updatepakketten (versie 2) op het Microsoft Downloadcentrum geplaatst. Klanten die handmatig versie 1 van deze update vanaf het Microsoft Downloadcentrum hebben geïnstalleerd, moeten versie 2 van deze update opnieuw installeren. Klanten die deze update via Microsoft Update of Office Update hebben geïnstalleerd, hoeven deze update niet opnieuw te installeren. Zie bulletin [MS08-051](http://technet.microsoft.com/security/bulletin/ms08-051) voor meer informatie, waaronder andere installatieopties of tijdelijke oplossingen.

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

-   [ISC/SANS](http://isc.sans.org/) voor het melden van een probleem dat wordt beschreven in MS08-042
-   [VeriSign iDefense VCP](http://www.idefense.com/vcp) voor het melden van een probleem dat wordt beschreven in MS08-043
-   [TippingPoint](http://www.tippingpoint.com/) en de [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS08-043
-   Jeremy Funk voor het melden van een probleem dat wordt beschreven in MS08-043
-   Shaun Colley van [NGS Software](http://www.nextgenss.com/) voor het melden van een probleem dat wordt beschreven in MS08-044
-   Damian Put, die werkt voor het [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/), voor het melden van een probleem dat is beschreven in MS08-044
-   Een anonieme onderzoeker die bij [iDefense VCP](http://labs.idefense.com/) werkt, voor het melden van een probleem dat wordt beschreven in MS08-044
-   Damian Put, die voor [iDefense VCP](http://labs.idefense.com/) werkt, voor het melden van een probleem dat wordt beschreven in MS08-044
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS08-045
-   Tavis Ormandy van het [Google Security Team](http://www.google.com/) voor het melden van een probleem dat wordt beschreven in MS08- 045
-   Sam Thomas, die samenwerkt met [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/), voor het melden van een probleem dat wordt beschreven in MS08-045.
-   [TippingPoint](http://www.tippingpoint.com/) en de [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS08-045
-   Jun Mao van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS08-046
-   Jorge Luis Alvarez Medina van [Core Security Technologies](http://www.coresecurity.com/) voor het melden van een probleem dat wordt beschreven in MS08-048
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS08-049
-   Haifei Li van [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com) van Fortinet voor het melden van een probleem dat wordt beschreven in MS08-050
-   Vadim Pogulievsky van [Malicious Code Research Center](http://www.finjan.com/securitylab.aspx?id=547) voor het melden van een probleem dat wordt beschreven in MS08-050.
-   Ruben Santamarta van [Reversemode.com](http://reversemode.com/), die werkt voor [iDefense Labs](http://labs.idefense.com/), voor het melden van een probleem dat wordt beschreven in MS08-051
-   ADLab van [Venustech](http://www.venustech.com.cn/) voor het melden van een probleem dat wordt beschreven in MS08-051

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (12 augustus 2008): Samenvatting van de gepubliceerde bulletins.
-   V2.0 (20 augustus 2008): Aan MS08-043 in 'Software waarin dit probleem optreedt' en 'Downloadlocaties' is een opmerking toegevoegd waarin wordt uitgelegd dat deze update geldt voor servers waarop Excel Services is geïnstalleerd, zoals de standaardconfiguratie van Microsoft Office SharePoint Server 2007 Enterprise en Microsoft Office SharePoint Server 2007 for Internet Sites. Microsoft Office SharePoint Server 2007 Standard wordt zonder Excel Services geleverd. Ook is er aan MS08-051 in 'Software waarin dit probleem optreedt' en 'Downloadlocaties' een opmerking toegevoegd dat Microsoft nieuwe updatepakketten (versie 2) voor Microsoft Office PowerPoint 2003 Service Pack 2 en Microsoft Office PowerPoint 2003 Service Pack 3 op het Microsoft Downloadcentrum heeft geplaatst. Klanten die handmatig versie 1 van deze update vanaf het Microsoft Downloadcentrum hebben geïnstalleerd, moeten versie 2 van deze update opnieuw installeren. Klanten die deze update via Microsoft Update of Office Update hebben geïnstalleerd, hoeven deze update niet opnieuw te installeren.
-   V3.0 (15 oktober 2008): Update voor Microsoft Access Snapshot Viewer opgenomen (MS08-041). Gebruikers die de update voor Microsoft Office 2000 Service Pack 3, Office XP Service Pack 2, Office 2003 Service Pack 2 of Office 2003 Service Pack 3 hebben geïnstalleerd, hoeven de update voor de zelfstandige Snapshot Viewer voor Microsoft Access niet opnieuw te installeren.

*Built at 2014-04-18T01:50:00Z-07:00*
