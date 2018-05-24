---
TOCTitle: 'MS07-JUL'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor juli 2007'
ms:assetid: 'ms07-jul'
ms:contentKeyID: 61231947
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms07-jul(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor juli 2007
==================================================================

Gepubliceerd: dinsdag 10 juli 2007 | Bijgewerkt: dinsdag 25 maart 2008

**Versie:** 2.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor juli 2007.

Met de release van de bulletins voor juli 2007 vervangt deze samenvatting van de bulletins de aankondiging van de bulletins, die oorspronkelijk werd uitgebracht op 7 juli 2007. Voor meer informatie over de meldingen voor bulletins gaat u naar het [bericht over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op woensdag 11 juli 2007 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van juli.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032343783&eventcategory=4&culture=en-us&countrycode=us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Kritiek (3)
-----------

<span></span>
| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-036                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Microsoft Excel kan externe code worden uitgevoerd (936542)**](http://technet.microsoft.com/security/bulletin/ms07-036)                                                                                                                                                                                                                                                                                                                                                                                  |
| **Samenvatting**                          | Met deze kritieke update wordt een openbaar gemaakt beveiligingslek en twee privé gemelde beveiligingslekken opgelost. Deze oplossing geldt tevens voor andere beveiligingsproblemen die in de loop van het onderzoek zijn aangetroffen. Door deze beveiligingslekken kan externe code worden uitgevoerd als een gebruiker een speciaal vervaardigd Excel-bestand opent. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Office, Excel**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-039                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Windows Active Directory kan externe code worden uitgevoerd (926122)**](http://technet.microsoft.com/security/bulletin/ms07-039)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Samenvatting**                          | Met deze kritieke beveiligingsupdate wordt een privé gemeld beveiligingslek in Active Directory op Windows 2000 Server en Windows Server 2003 opgelost als gevolg waarvan externe code kan worden uitgevoerd of waardoor een Denial of Service-aanval kan worden veroorzaakt. Misbruik van dit beveiligingslek zal hoogstwaarschijnlijk resulteren in een denial of service. Het kan echter ook zijn dat in dit geval ook uitvoering van externe code mogelijk wordt. Op Windows Server 2003 moet een aanvaller geldige aanmeldingsreferenties hebben om dit beveiligingslek te kunnen misbruiken. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts maken. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Windows**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-040                                                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in .NET Framework kan externe code worden uitgevoerd (931212)**](http://technet.microsoft.com/security/bulletin/ms07-040)                                                                                                                                                                                                                                                                                           |
| **Samenvatting**                          | Met deze update worden drie privé gemelde beveiligingslekken opgelost. Bij twee van deze beveiligingslekken kan externe code op clientsystemen met .NET Framework worden uitgevoerd en bij het andere beveiligingslek kan informatie worden vrijgegeven op servers waarop ASP.NET wordt uitgevoerd. In alle gevallen hebben gebruikers met minder rechten dan beheerders minder last van dit beveiligingslek dan gebruikers met beheerrechten. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                        |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                 |
| **Software waarin dit probleem optreedt** | **.NET Framework**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                         |

Belangrijk (2)
--------------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-037                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Office Publisher kan externe code worden uitgevoerd (936548)**](http://technet.microsoft.com/security/bulletin/ms07-037)                                                                                                                                                                                                                                                                                                                              |
| **Samenvatting**                          | Met deze belangrijke beveiligingsupdate wordt één openbaar gemaakt beveiligingslek opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd wanneer een gebruiker een speciaal ontworpen Microsoft Office Publisher-bestand opent. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. Er is gebruikersinteractie vereist om misbruik te maken van dit beveiligingslek. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Opnieuw opstarten van het systeem is niet vereist.                                                                                                                                                                                                                                                                                                                                   |
| **Software waarin dit probleem optreedt** | **Office, Publisher**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                      |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-041                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Microsoft Internet Information Services kan externe code worden uitgevoerd (939373)**](http://technet.microsoft.com/security/bulletin/ms07-041)                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Samenvatting**                          | Door deze update met hoge prioriteit wordt een privé gemeld beveiligingslek opgelost. Door dit beveiligingslek kan externe code worden uitgevoerd indien een aanvaller speciaal geformuleerde URL-aanvragen naar een webpagina verzendt waarvoor Internet Information Services (IIS) 5.1 als host fungeert op Windows XP Professional Service Pack 2. IIS 5.1 is geen onderdeel van de standaardinstallatie van Windows XP Professional Service Pack 2. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan volledige controle krijgen over het systeem waarop dit probleem voorkomt. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Software waarin dit probleem optreedt** | **Windows XP Professional**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

Matig (1)
---------

<span></span>
| Bulletin-id                               | Microsoft-beveiligingsbulletin MS07-038                                                                                                                                                                                                                                        |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in de firewall van Windows Vista kan informatie worden vrijgegeven (935807)**](http://technet.microsoft.com/security/bulletin/ms07-038)                                                                                                            |
| **Samenvatting**                          | Door deze update met gemiddelde prioriteit wordt een privé gemeld beveiligingslek opgelost. Via dit beveiligingslek kan binnenkomend ongewenst netwerkverkeer toegang tot het netwerk krijgen. Een aanvaller zou mogelijk informatie over de getroffen host kunnen verzamelen. |
| **Maximaal prioriteitsniveau**            | [Matig](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                          |
| **Gevolgen van het beveiligingslek**      | Vrijgeven van informatie                                                                                                                                                                                                                                                       |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                 |
| **Software waarin dit probleem optreedt** | **Windows** **Vista**. Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                      |

Software waarin het probleem optreedt en Downloadlocaties
---------------------------------------------------------

<span></span>
**Gebruik van deze tabel**

In deze tabel vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of onderdeel in de tabel controleren of er beveiligingsupdates vereist zijn. Als een softwareprogramma of -onderdeel in de tabel voorkomt, worden de gevolgen van het beveiligingslek weergegeven en is er een koppeling naar de beschikbare software-update.

**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.

**Software waarin het probleem optreedt en Downloadlocaties**

 
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
[**MS07-036**](http://technet.microsoft.com/security/bulletin/ms07-036)
</td>
<td style="border:1px solid black;">
[**MS07-037**](http://technet.microsoft.com/security/bulletin/ms07-037)
</td>
<td style="border:1px solid black;">
[**MS07-038**](http://technet.microsoft.com/security/bulletin/ms07-038)
</td>
<td style="border:1px solid black;">
[**MS07-039**](http://technet.microsoft.com/security/bulletin/ms07-039)
</td>
<td style="border:1px solid black;">
[**MS07-040**](http://technet.microsoft.com/security/bulletin/ms07-040)
</td>
<td style="border:1px solid black;">
[**MS07-041**](http://technet.microsoft.com/security/bulletin/ms07-041)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Matig**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<th colspan="7">
Windows-software waarin het probleem optreedt
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 2000 Service Pack 4
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=812e62c5-6e19-4b3b-8a10-861b871e1b41)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional Service Pack 2
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
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=fccbfe90-f838-47df-8310-352e2fb47132)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=28e84603-8159-4429-aaff-a1020531e84f)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=107902f9-be94-457f-a936-519efbd64779)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=e5e5b425-fe7d-49d5-973f-f3fd7a1e04eb)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
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
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=e9b64746-6afa-4a30-833d-e058e000c821)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Matig](http://www.microsoft.com/downloads/details.aspx?familyid=0df5d190-3ad7-42d5-8629-43c47ec450cb)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 x64 Edition
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
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Onderdelen van Windows waarin het probleem optreedt
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB928367)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=91d7afe4-069b-4ce8-976e-9a01345a8603)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.0  
(KB930494)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=829a2c5b-11ec-4ed7-91ab-6961034147bc)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB928366)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=281fb2cd-c715-4f05-a01f-0455d2d9ebfb)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB933854)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=2495e656-1e0a-4b83-90da-821e68067a71)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 1.1  
(KB929729)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=7eea368d-7b82-4583-8537-30351718a4e9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB928365)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=ba3ceb78-8e1b-4c38-adfd-e8bc95ae548d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft .NET Framework 2.0  
(KB929916)
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
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=cbc9f3cf-c3c3-45c4-82e3-e11398bc2cd2)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7">
Office-software waarin het probleem optreedt
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Excel 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=83d94d8e-dda6-4d74-b40d-476c2f0a3af4)
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
Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=9d93c0ce-5124-4234-ba84-3c27005e010f)
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
Excel 2003 Viewer
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=11f42977-8828-494a-a183-d1aba827b708)
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
Excel 2007
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=9ab28283-0320-4527-b033-5e80ef32cd34)
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
Office Compatibility Pack voor de bestandsindelingen van Word, Excel en PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=e592ae5b-09ac-4f5b-b457-a54c9850ad4a)
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
Publisher 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=25d272e7-f2dd-4342-92be-7ebc2e770b44)
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
</table>
 
**Opmerkingen**

**<sup>[1]</sup>** Er is een beveiligingsupdate voor dit besturingssysteem beschikbaar. Zie de tabel voor informatie over de software of het onderdeel waarin het probleem optreedt, en het betreffende beveiligingsbulletin voor details.** **

** **

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging voor thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn verkrijgbaar via [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) en [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security\_patch''. Ten slotte kunt u beveiligingsupdates downloaden uit de Windows Update-catalogus. Zie [Microsoft Knowledge Base-artikel 323166](http://support.microsoft.com/kb/323166) voor meer informatie over de Windows Update-catalogus.

**Richtlijnen voor detecteren en implementeren**

Microsoft heeft richtlijnen voor detecteren en implementeren uitgebracht voor de beveiligingsupdates van deze maand. Aan de hand van deze richtlijnen kunnen IT-professionals zien hoe zij met de diverse hulpprogramma's de beveiligingsupdate moeten implementeren, zoals Windows Update, Microsoft Update, Office Update, de Microsoft Baseline Security Analyzer (MBSA), de Office Detection Tool, Microsoft Systems Management Server (SMS), de Extended Security Update Inventory Tool en de Enterprise Update Scan Tool (EST). Zie [Microsoft Knowledge Base-artikel 910723](http://support.microsoft.com/kb/910723) voor meer informatie.

**Microsoft Baseline Security Analyzer en** **Enterprise** **Update Scan Tool**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

Als MBSA 1.2.1 detectie voor een bepaalde beveiligingsupdate niet kan ondersteunen, geeft Microsoft een versie van Enterprise Update Scan Tool (EST) voor de desbetreffende beveiligingsupdate uit. Ga voor meer informatie over EST naar [Enterprise Update Scan Tool](http://support.microsoft.com/default.aspx?id=894193).

**Opmerking** Na 9 oktober 2007 zal het bestand MSSecure.XML, dat door MBSA 1.2.1 wordt gebruikt, niet langer worden bijgewerkt. Na deze datum zullen geen nieuwe beveiligingsupdates worden toegevoegd aan het bestand MSSecure.XML, dat door MBSA 1.2.1 wordt gebruikt, en zullen geen nieuwe versies van Enterprise Scan Tool meer worden uitgegeven. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie.

**Software Update Services**

Met Microsoft Software Update Services (SUS) kunnen beheerders snel en betrouwbaar de meest recente essentiële updates en beveiligingsupdates implementeren voor Windows 2000- en Windows Server 2003-servers, alsmede voor desktopsystemen met Windows 2000 Professional of Windows XP Professional.

Ga naar de website [Software Update Services](http://go.microsoft.com/fwlink/?linkid=21133) voor meer informatie over de implementatie van deze beveiligingsupdate met Software Update Services.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders snel en betrouwbaar de nieuwste essentiële updates en beveiligingsupdates implementeren voor Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders met SMS 2003 beveiligingsupdates kunnen implementeren. SMS 2.0-gebruikers kunnen ook het [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) gebruiken voor de implementatie van beveiligingsupdates. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking:** SMS maakt gebruik van de Microsoft Baseline Security Analyzer en de Microsoft Office Detection Tool om brede ondersteuning te kunnen bieden voor het zoeken en uitvoeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

Dit hulpprogramma is **niet** beschikbaar via Software Update Services (SUS).

#### Belangrijke niet-beveiligingsupdates op MU, WU, WSUS en SUS

Planning voor deze maand:

-   Microsoft heeft op Microsoft Update (MU) en Windows Server Update Services (WSUS) vier belangrijke updates uitgegeven die **geen beveiligingsupdates** zijn.
-   Microsoft heeft voor Windows Update (WU) en Software Update Services (SUS) één belangrijke update uitgegeven die **geen beveiligingsupdate is**.

De informatie geldt **alleen** voor belangrijke **niet-beveiligingsupdates** op Microsoft Update, Windows Update, Windows Server Update Services en Software Update Services, die op dezelfde dag als de samenvatting van de beveiligingsbulletins zijn uitgegeven. Er wordt **geen** informatie gegeven over **niet-beveiligingsupdates** die op andere dagen zijn uitgegeven.

#### Veiligheidsstrategieën en community

**Strategieën voor updatebeheer**

Op de website [Security Guidance for Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) kunt u extra informatie vinden over aanbevelingen van Microsoft voor het toepassen van beveiligingsupdates.

**Verkrijgen van andere beveiligingsupdates**

Op de volgende locaties zijn updates verkrijgbaar voor andere beveiligingsproblemen:

-   Beveiligingsupdates zijn verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord 'security\_patch'.
-   Updates voor consumentenplatforms zijn verkrijgbaar op de website [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   U kunt de beveiligingsupdates van deze maand die op Windows Update staan, via het ISO CD-imagebestand met beveiligingsupdates en essentiële updates vanaf het Downloadcentrum ophalen. Zie [Microsoft Knowledge Base-artikel 913086](http://support.microsoft.com/kb/913086) voor meer informatie.

**IT Pro Security-community**

Leer de beveiliging te verbeteren en uw IT-infrastructuur te optimaliseren en bespreek beveiligingsonderwerpen met andere IT-professionals op de website [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Dankbetuiging

Microsoft [bedankt](http://go.microsoft.com/fwlink/?linkid=21127) de volgende partijen voor de samenwerking bij het verbeteren van de beveiliging voor klanten:

-   Dinis Cruz van [OWASP](http://www.owasp.org/) voor het melden van een probleem dat wordt beschreven in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Paul Craig van [Security Assessment](http://www.smsiinc.com/) voor het melden van een probleem dat wordt beschreven in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Jeroen Frijters van [Sumatra](http://www.sumatra.nl/) voor het melden van een probleem dat wordt beschreven in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   [ProCheckUp](http://www.procheckup.com/) in samenwerking met [UK CPNI](http://www.cpni.gov.uk/) voor het melden van een probleem dat wordt beschreven in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040).
-   Ferruh T. Mavituna van [Portcullis Computer Security Ltd.](http://www.portcullis-security.com/) voor de samenwerking met Microsoft en het leveren van aanvullende informatie over een probleem dat in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040) wordt beschreven.
-   Johannes Gumbel van [TrueSec](http://www.truesec.com/) voor de samenwerking met Microsoft en het leveren van aanvullende informatie over een probleem dat in [MS07-040](http://technet.microsoft.com/security/bulletin/ms07-040) wordt beschreven.
-   Peter Winter-Smith van [NGSSoftware](http://www.nextgenss.com/) voor het melden van een probleem dat wordt beschreven in [MS07-039](http://technet.microsoft.com/security/bulletin/ms07-039).
-   Neel Mehta van [IBM Internet Security Systems x-Force](http://xforce.iss.net/) voor het melden van een probleem dat wordt beschreven in [MS07-039](http://technet.microsoft.com/security/bulletin/ms07-039).
-   [eEye](http://www.eeye.com/) voor het melden van een probleem dat wordt beschreven in [MS07-037](http://go.microsoft.com/fwlink/?linkid=93488).
-   Jim Hoagland en Ollie Whitehouse van [Symantec](http://www.symantec.com/) voor het melden van een probleem dat wordt beschreven in [MS07-038](http://technet.microsoft.com/security/bulletin/ms07-038).
-   Jonathan Afek en Adi Sharabani van [Watchfire](http://www.watchfire.com/) voor het samenwerken met Microsoft en het aanleveren van aanvullende informatie over een probleem dat wordt beschreven in [MS07-041](http://technet.microsoft.com/security/bulletin/ms07-041).
-   Peter Winter-Smith van [NGSSoftware](http://www.nextgenss.com/) voor de samenwerking met Microsoft en het leveren van aanvullende informatie over een probleem dat in [MS07-041](http://technet.microsoft.com/security/bulletin/ms07-041) wordt beschreven.

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (10 juli 2007): Samenvatting van de gepubliceerde bulletins.
-   V2.0 (25 maart 2008): Windows Vista Service Pack 1, Windows Vista x64 Edition Service Pack 1, Windows Server 2008, Windows Server 2008 voor Itanium-systemen en Windows Server 2008 x64 Edition zijn toegevoegd aan het overzicht met software waarin dit probleem optreedt.

*Built at 2014-04-18T01:50:00Z-07:00*
