---
TOCTitle: 'MS08-FEB'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor februari 2008'
ms:assetid: 'ms08-feb'
ms:contentKeyID: 61231957
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms08-feb(v=Security.10)'
author: SharonSears
ms.author: SharonSears
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor februari 2008
======================================================================

Gepubliceerd: dinsdag 12 februari 2008 | Bijgewerkt: woensdag 13 februari 2008

**Versie:** 1.1

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor februari 2008.

Met de release van de bulletins voor februari 2008 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 7 februari 2008. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar de [mededelingenservice voor Microsoft-beveiligingsbulletin](http://go.microsoft.com/fwlink/?linkid=21163). voor meer informatie over het automatisch ontvangen van berichten met de datums waarop beveiligingsbulletins van Microsoft worden uitgegeven.

Op 13 februari 2008 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van februari.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357215&eventcategory=4&culture=en-us&countrycode=us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Kritiek (6)
-----------

<span></span>
| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-007                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in WebDAV-mini-redirector kan externe code worden uitgevoerd (946026)**](http://technet.microsoft.com/security/bulletin/ms08-007)                                                                                                                                                                                                                                                            |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate wordt een privé gemeld beveiligingslek in de WebDAV-mini-redirector opgelost. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                  |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                          |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-008                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in OLE-automatisering kan externe code worden uitgevoerd (947890)**](http://technet.microsoft.com/security/bulletin/ms08-008)                                                                                                                                                                                                                                                                                                                                                     |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate wordt een privé gemeld beveiligingslek opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina heeft weergegeven. Van dit beveiligingslek kan misbruik worden gemaakt via aanvallen op OLE-automatisering (Object Linking and Embedding). Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                |
| **Software waarin dit probleem optreedt** | **Windows, Office, Visual Basic.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                         |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-009                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Word kan externe code worden uitgevoerd (947077)**](http://technet.microsoft.com/security/bulletin/ms08-009)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Word opgelost waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Word-bestand opent. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Software waarin dit probleem optreedt** | **Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-010                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Cumulatieve beveiligingsupdate voor Internet Explorer (944533)**](http://technet.microsoft.com/security/bulletin/ms08-010)                                                                                                                                                                                                                                                                                                                                                            |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate worden drie privé gemelde beveiligingslekken en één openbaar gemeld beveiligingslek opgelost. In het ergste geval kan er als gevolg van het beveiligingslek externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina heeft weergegeven in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Windows, Internet Explorer.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                       |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-012                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft Office Publisher kan externe code worden uitgevoerd (947085)**](http://technet.microsoft.com/security/bulletin/ms08-012)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate worden twee privé gemelde beveiligingslekken in Microsoft Office Publisher opgelost waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Publisher-bestand opent. Een aanvaller die misbruik weet te maken van het beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Software waarin dit probleem optreedt** | **Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-013                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Office kan externe code worden uitgevoerd (947108)**](http://technet.microsoft.com/security/bulletin/ms08-013)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate wordt een beveiligingslek in Microsoft Office opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd als een gebruiker een speciaal ontworpen Microsoft Office-bestand opent dat een verkeerd ingedeeld object bevat. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Software waarin dit probleem optreedt** | **Office.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

Belangrijk (5)
--------------

<span></span>
| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-003                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in Active Directory kan leiden tot denial of service (946538)**](http://technet.microsoft.com/security/bulletin/ms08-003)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Samenvatting**                          | Met deze belangrijke beveiligingsupdate wordt een privé gemeld beveiligingslek opgelost in implementaties van Active Directory op Microsoft Windows 2000 Server en op Windows Server 2003 en Active Directory Application Mode (ADAM) wanneer geïnstalleerd op Windows XP Professional en Windows Server 2003. Het beveiligingslek kan leiden tot een denial of service. Op Windows Server 2003 en Windows XP Professional moet een aanvaller geldige aanmeldingsreferenties hebben om dit beveiligingslek te kunnen misbruiken. Een aanvaller die dit lek weet te misbruiken, kan ervoor zorgen dat het systeem waarin dit probleem optreedt niet meer reageert of opnieuw wordt opgestart. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Gevolgen van het beveiligingslek**      | Denial of service                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Software waarin dit probleem optreedt** | **Windows, Active Directory, ADAM. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-004                                                                                                                                                                                                                                                                                     |
|-------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in Windows TCP/IP kan leiden tot denial of service (946456)**](http://technet.microsoft.com/security/bulletin/ms08-004)                                                                                                                                                                                  |
| **Samenvatting**                          | Deze belangrijke update lost een privé gemeld beveiligingslek in de verwerking van het Transmission Control Protocol/Internetprotocol (TCP/IP) op. Een aanvaller die dit lek weet te misbruiken, kan ervoor zorgen dat het systeem waarin dit probleem optreedt, niet meer reageert en automatisch opnieuw wordt opgestart. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                  |
| **Gevolgen van het beveiligingslek**      | Denial of service                                                                                                                                                                                                                                                                                                           |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                              |
| **Software waarin dit probleem optreedt** | **Windows. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                             |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-005                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Een beveiligingslek in Internet Information Services kan leiden tot misbruik van bevoegdheden (942831)**](http://technet.microsoft.com/security/bulletin/ms08-005)                                                                                                                                                                                                                                                                                                                                                                              |
| **Samenvatting**                          | Deze belangrijke update lost een privé gemeld beveiligingslek in Internet Information Services (IIS) op. Een lokale aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Gevolgen van het beveiligingslek**      | Misbruik van bevoegdheden                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software waarin dit probleem optreedt** | **Windows, IIS. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-006                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Internet Information Services kan externe code worden uitgevoerd (942830)**](http://technet.microsoft.com/security/bulletin/ms08-006)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Samenvatting**                          | Deze belangrijke update lost een privé gemeld beveiligingslek in Internet Information Services (IIS) op. Er is een beveiligingslek met betrekking tot het uitvoeren van externe code aanwezig in de manier waarop de Internet Information Service invoer verwerkt op ASP-webpagina's. Een aanvaller die dit beveiligingslek weet te misbruiken, zou vervolgens handelingen op de IIS-server kunnen verrichten met dezelfde rechten als de werkprocesidentiteit (WPI). De WPI wordt standaard met netwerkservice-accountbevoegdheden geconfigureerd. IIS-servers met ASP-pagina's waarvan de toepassingsgroepen zijn geconfigureerd met een WPI die gebruikmaakt van een account met beheerdersbevoegdheden lopen mogelijk een groter gevaar dan IIS-servers waarvan de toepassingsgroep is geconfigureerd met de standaard WPI-instellingen. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Software waarin dit probleem optreedt** | **Windows, IIS. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-011                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in het bestandsconversieprogramma van Microsoft Works kan externe code worden uitgevoerd (947081)**](http://technet.microsoft.com/security/bulletin/ms08-006)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Samenvatting**                          | Door deze belangrijke update worden drie privé gemelde beveiligingslekken in het bestandsconversieprogramma van Microsoft Works opgelost. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd Works-bestand (.wps) opent met een versie van Microsoft Office, Microsoft Works of Microsoft Works Suite waarin dit probleem optreedt. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem niet vereist.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Software waarin dit probleem optreedt** | **Office, Works, Works Suite. **Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

Software waarin het probleem optreedt en Downloadlocaties
---------------------------------------------------------

<span></span>
**Gebruik van deze tabel**

In deze tabel vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of onderdeel in de tabel controleren of er beveiligingsupdates vereist zijn. Als een softwareprogramma of -onderdeel in de tabel voorkomt, worden de gevolgen van het beveiligingslek weergegeven en is er een koppeling naar de beschikbare software-update.

**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.

**Software waarin het probleem optreedt en Downloadlocaties**

#### Software waarin het probleem optreedt, en downloadlocaties voor bulletins MS08-003 tot en met MS08-008

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-003**](http://technet.microsoft.com/security/bulletin/ms08-003)
</td>
<td style="border:1px solid black;">
[**MS08-004**](http://technet.microsoft.com/security/bulletin/ms08-004)
</td>
<td style="border:1px solid black;">
[**MS08-005**](http://technet.microsoft.com/security/bulletin/ms08-005)
</td>
<td style="border:1px solid black;">
[**MS08-006**](http://technet.microsoft.com/security/bulletin/ms08-006)
</td>
<td style="border:1px solid black;">
[**MS08-007**](http://technet.microsoft.com/security/bulletin/ms08-007)
</td>
<td style="border:1px solid black;">
[**MS08-008**](http://technet.microsoft.com/security/bulletin/ms08-008)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="7">
Windows-besturingssysteem
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=93b3d0a3-2091-405e-8dd4-10f20dc2be7f)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=afeef3ec-6160-4c1d-94bd-0bfce641d0a2)
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=5c331a3a-93e0-42e4-9cd1-4e32ebdda38d)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=15b7d1c4-4ef4-47b2-9e3b-22eafbdb90d8)
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=e0a15967-7184-4194-8edb-81760e440604)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=b7e725bf-7248-4119-aca5-b7d502c09cfc)
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=cfa0d5c6-a9b0-4c5c-a651-898e9f900799)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=8af82f86-731c-46a0-a025-b62447e2af38)
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=a08e87dc-993b-493b-8af3-be6e98643aeb)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=bca224db-fe0e-411d-a948-1c776ce974f3)
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=5a88522b-ee30-4deb-878b-598e852fd60e)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=8ce9608b-7049-47cd-adc4-22a803877d33)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=ba7a2b42-1c89-45e5-b8a6-049fa500c03a)
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=c67ec357-0f86-4f7d-9af0-d63d8b765f44)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=d7b9c3d1-9c23-4e05-bac6-d0b327feaf53)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=45962232-af78-42cb-bfa0-9ce7de199585)
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=9137108f-e80b-46f1-b547-82da8fb058bf)
</td>
</tr>
<tr>
<th colspan="7">
Onderdelen van Windows waarin het probleem optreedt
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Information Services 5.0 op Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=b24f34fb-40b9-4aa5-b5ac-e3f0a6062753)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Information Services 5.1 op Windows XP Professional Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=73d24fcf-bea9-4b13-9f1c-4e068c53a4ae)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=2b498065-d682-4227-b23e-d234d7d6a3fe)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Information Services 6.0 op Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=103a6bc0-034a-443d-b1d4-81117820dcb2)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=df9875f7-04d6-486e-bdb5-35e9e305fa1d)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Information Services 6.0 op Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=516ef8e8-3cb6-4660-b771-3c7f66917a11)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=6583e798-d16d-419c-aee1-30c3e6c635b3)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Information Services 6.0 op Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=e24fb33c-67b9-4ed4-9317-b5fd535d005a)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=e8286174-8209-409f-8805-e534715a741c)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Information Services 6.0 op Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=5a4a6083-8c67-4403-8e20-7f2b82178124)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=29faa70d-f1ac-4da4-b72a-faf1973cd845)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Information Services 7.0 op Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=8c7018ec-ae80-4a30-93fc-0f7386732514)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Information Services 7.0 op Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=4de2fffc-5793-4acf-98ee-1b801e59ae39)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Active Directory op Microsoft Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=9df0875d-0466-4974-b4c0-1ecc777173b1)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
ADAM wanneer geïnstalleerd op Windows XP Professional Service Pack 2
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=bff7dcb9-5d00-442e-b03c-ce923d213faa)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ADAM wanneer geïnstalleerd op Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2:
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=36e36e1a-ed0d-45a6-b707-766fabc01fbd)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Active Directory op Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=63d3d784-f057-4686-b85e-ab5fbab5a722)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Active Directory wanneer geïnstalleerd op Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=60781cf3-7c6d-4795-a9d0-bc18ee356e94)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Active Directory op Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=835d647a-dce6-476e-b7c4-928a67b0acfb)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
ADAM indien geïnstalleerd op Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=5e97698d-8150-44f9-9d34-87a0db6ba5a7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Active Directory op Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=eda8af09-1a4c-4163-a8bb-97dacdebeae4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Microsoft Office:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 voor Mac
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=36b00c58-192d-488c-a069-730c69f0b6b0)
</td>
</tr>
<tr>
<th colspan="7">
Overige software waarin dit probleem optreedt
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 6.0 Service Pack 6
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=c96420a9-7436-4625-9649-75f1514b0fe3)
</td>
</tr>
</table>
 
**Opmerkingen**

**<sup>[1]</sup>** Er is een beveiligingsupdate voor dit besturingssysteem beschikbaar. Zie de tabel voor informatie over de software of het onderdeel waarin het probleem optreedt, en het betreffende beveiligingsbulletin voor details.** **

#### Software waarin het probleem optreedt, en downloadlocaties voor bulletins MS08-009 tot en met MS08-013

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-009**](http://technet.microsoft.com/security/bulletin/ms08-009)
</td>
<td style="border:1px solid black;">
[**MS08-010**](http://technet.microsoft.com/security/bulletin/ms08-010)
</td>
<td style="border:1px solid black;">
[**MS08-011**](http://technet.microsoft.com/security/bulletin/ms08-006)
</td>
<td style="border:1px solid black;">
[**MS08-012**](http://technet.microsoft.com/security/bulletin/ms08-012)
</td>
<td style="border:1px solid black;">
[**MS08-013**](http://technet.microsoft.com/security/bulletin/ms08-013)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="6">
Windows-besturingssysteem
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
Onderdelen van Windows waarin het probleem optreedt
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 5.01 Service Pack 4 op Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=1032a039-468b-4c5f-8c1c-5e54c2832e41)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Service Pack 1 indien geïnstalleerd op Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=87e66dce-5060-4814-8754-829b4e190359)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 voor Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=bb2aa3cb-021f-4890-ab20-2a51f8e17554)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 voor Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=8989f576-8b30-4866-90ec-929d24f3b409)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 voor Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=429b7ed1-fe78-459a-b834-d0f3c69cb703)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 voor Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=e989e23c-38bb-4fe7-a830-d7bdf7659392)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 voor Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=5a097f7a-b696-48d0-b13f-337c5fd14e24)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 voor Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=d4aa293a-6332-4c6c-b128-876f516bd030)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 voor Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=b72af1b6-6e23-4005-aef6-82195b380153)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 voor Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=b2aa6562-881e-4fd6-be1b-53426a0ff4a9)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 voor Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=4bb99afc-be14-4f2e-9570-b7fe09e39131)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 voor Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=6fa80e2c-5e91-4b33-acd9-33f156660ae7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 in Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=0de25b98-f443-4874-a06f-4daae14c16b0)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 in Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=c08ebbe7-639b-4ea2-8304-fab531930abf)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
Microsoft Office:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=5fb74e24-d9ee-4951-9c46-e1c84617f097)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=3e147b1a-f3be-465f-8587-7f3a33d6a6e5)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=f4ac0f34-4604-4bbe-9669-01db645041ca)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 voor Mac
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=36b00c58-192d-488c-a069-730c69f0b6b0)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=a513069b-8244-48e9-b136-01ddd3862802)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Word 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=78c338aa-e410-4422-9e36-562f70d742e9)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Word 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=85cb1aa5-211f-4652-827b-2e79b8ffc2fc)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=fd4ddecd-abd6-4783-b300-32b9d4bad22a)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Publisher 2000
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=d8b085fb-858f-4c7e-96de-edff8f49d62a)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Publisher 2002
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=1135c63a-6ce7-4051-81ba-bfbba8d857fb)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Publisher 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=7078b952-09f6-4c47-8c05-40667e1f1c3b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="6">
Office-software waarin het probleem optreedt
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Bestandsconversieprogramma van Microsoft Works 6 op Microsoft Office 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=30c9c3fe-fb85-43d9-bbc3-0b30d3a20286)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bestandsconversieprogramma van Microsoft Works 6 op Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=30c9c3fe-fb85-43d9-bbc3-0b30d3a20286)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Bestandsconversieprogramma van Microsoft Works 6 op Microsoft Works 8.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=30c9c3fe-fb85-43d9-bbc3-0b30d3a20286)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Bestandsconversieprogramma van Microsoft Works 6 op Microsoft Works Suite 2005
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=30c9c3fe-fb85-43d9-bbc3-0b30d3a20286)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Opmerkingen**

**<sup>[1]</sup>** Er is een beveiligingsupdate voor dit besturingssysteem beschikbaar. Zie de tabel voor informatie over de software of het onderdeel waarin het probleem optreedt, en het betreffende beveiligingsbulletin voor details.** **

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

System Center Configuration Manager (SCCM) 2007 gebruikt WSUS 3.0 voor het detecteren van updates. Ga naar [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx) voor meer informatie over het software-updatebeheer van SCCM 2007.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar; zie ook [System Center Configuration Manager 2007.](http://technet.microsoft.com/en-us/library/bb735860.aspx) Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren. SMS 2.0-gebruikers kunnen ook het [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) gebruiken voor de implementatie van beveiligingsupdates. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking:** SMS maakt gebruik van de Microsoft Baseline Security Analyzer en de Microsoft Office Detection Tool om brede ondersteuning te kunnen bieden voor het zoeken en uitvoeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:

Planning voor deze maand:

-   Microsoft heeft voor Microsoft Update (MU) en Windows Server Update Services (WSUS) zeven belangrijke updates uitgegeven die **geen beveiligingsupdate** zijn.
-   Microsoft heeft twee belangrijke updates voor Windows die **geen beveiligingsupdates** zijn, uitgegeven op Windows Update (WU) en WSUS.

De informatie geldt **alleen** voor belangrijke **niet-beveiligingsupdates** op Microsoft Update, Windows Update en Windows Server Update Services, die op dezelfde dag als de samenvatting van de beveiligingsbulletins zijn uitgegeven. Er wordt **geen** informatie gegeven over **niet-beveiligingsupdates** die op andere dagen zijn uitgegeven.

#### Veiligheidsstrategieën en community

**Strategieën voor updatebeheer**

Op de website [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) kunt u extra informatie vinden over aanbevelingen van Microsoft voor het toepassen van beveiligingsupdates.

**Verkrijgen van andere beveiligingsupdates**

Op de volgende locaties zijn updates verkrijgbaar voor andere beveiligingsproblemen:

-   Beveiligingsupdates zijn verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.
-   Updates voor consumentenplatforms zijn verkrijgbaar op de website [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   U kunt de beveiligingsupdates van deze maand die op Windows Update staan, via het ISO CD-beeldbestand met beveiligingsupdates en essentiële updates vanaf het Microsoft Downloadcentrum ophalen. Zie [Microsoft Knowledge Base-artikel 913086](http://support.microsoft.com/kb/913086) voor meer informatie.

**IT Pro Security-community**

Leer de beveiliging te verbeteren en uw IT-infrastructuur te optimaliseren en bespreek beveiligingsonderwerpen met andere IT-professionals op de website [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Dankbetuiging

Microsoft [bedankt](http://go.microsoft.com/fwlink/?linkid=21127) de volgende partijen voor de samenwerking bij het verbeteren van de beveiliging voor klanten:

-   Thomas Garnier van [SkyRecon](http://www.skyrecon.com/) voor het melden van een probleem dat wordt beschreven in MS08-003.
-   Tomas Potok, Martin Dominik, Martin Luptak en Eva Juhasova van [Whitestein Technologies](http://www.whitestein.com/) voor het melden van een probleem dat wordt beschreven in MS08-004
-   Steven van [COSEINC Vulnerability Research Lab](http://www.coseinc.com/) voor het melden van een probleem dat wordt beschreven in MS08-007
-   Ryan Smith en Alex Wheeler van [IBM ISS X-Force](http://www.iss.net/) voor het melden van een probleem dat wordt beschreven in MS08-008
-   Rubén Santamarta van [ReverseMode.com](http://reversemode.com/) voor het melden van een probleem dat wordt beschreven in MS08-009
-   Shane Macaulay en Riley Hassell of [Security Objectives](http://www.security-objectives.com/) voor het melden van een probleem dat wordt beschreven in MS08-010
-   Een anonieme onderzoeker die bij [TippingPoint](http://www.tippingpoint.com/) werkt en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS08-010.
-   hyy, die voor [VeriSign iDefense VCP](http://idefense.com/) werkt, voor het samen met Microsoft werken aan een probleem dat wordt beschreven in MS08-010
-   ADLab van [Venustech](http://www.venustech.com.cn/) voor het melden van een probleem dat wordt beschreven in MS08-010
-   [VeriSign iDefense VCP](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS08-011
-   Damian Put, die voor [VeriSign iDefense VCP](http://labs.idefense.com/) werkt, voor het melden van een probleem dat wordt beschreven in MS08-011
-   [IBM Internet Security Systems X-Force](http://xforce.iss.net/) voor het melden van een probleem dat wordt beschreven in MS08-011
-   Piotr Bania voor het melden van een probleem dat wordt beschreven in MS08-012
-   Bing Liu van [Fortinet Security Research](http://www.fortinet.com/) voor het melden van een probleem dat wordt beschreven in MS08-012
-   Bing Liu van [Fortinet Security Research](http://www.fortinet.com/) voor het melden van een probleem dat wordt beschreven in MS08-012
-   Shaun Colley van [NGSSoftware](http://www.ngssoftware.com/) voor het melden van een probleem dat wordt beschreven in MS08-013

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (12 februari 2008): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (13 februari 2008): Samenvatting van bulletin bijgewerkt. In MS08-005 is de verwijzing naar de downloadkoppeling voor Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2 bijgewerkt voor verwijzing naar Internet Information Services 6.0. De downloadkoppeling verwees klanten op de juiste wijze naar de update voor IIS 6.0, maar de referentiekoppeling verwees klanten naar IIS 5.1.

*Built at 2014-04-18T01:50:00Z-07:00*
