---
TOCTitle: 'MS07-NOV'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor november 2007'
ms:assetid: 'ms07-nov'
ms:contentKeyID: 61231951
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms07-nov(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor november 2007
======================================================================

Gepubliceerd: dinsdag 13 november 2007

**Versie:** 1.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor november 2007.

Met de release van de bulletins voor november 2007 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins, die oorspronkelijk werd uitgegeven op 8 november 2007. Voor meer informatie over de vooraankondiging over bulletins gaat u naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar de [mededelingenservice voor Microsoft-beveiligingsbulletin](http://go.microsoft.com/fwlink/?linkid=21163). voor meer informatie over het automatisch ontvangen van berichten met de datums waarop beveiligingsbulletins van Microsoft worden uitgegeven.

Op 14 november 2007 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft tijdens een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van november](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344694&eventcategory=4&culture=en-us&countrycode=us). Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Kritiek (1)
-----------

<span></span>
| Bulletin-id                               | Microsoft Security Bulletin MS07-061                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|-------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in Windows met betrekking tot de afhandeling van URI's kan externe code worden uitgevoerd (943460)**](http://technet.microsoft.com/security/bulletin/ms07-061)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Samenvatting**                          | Met deze update wordt een openbaar gemaakt beveiligingslek opgelost. Er bestaat een beveiligingslek met betrekking tot het uitvoeren van externe code dat wordt veroorzaakt door de manier waarop de Windows-shell speciaal vervaardigde URI's afhandelt die aan de shell worden doorgegeven. Wanneer de Windows-shell de URI's onvoldoende valideert, kan een aanvaller het beveiligingslek misbruiken en code uitvoeren. Microsoft heeft alleen ontdekt op welke manieren dit beveiligingslek kan worden misbruikt op systemen met Internet Explorer 7. Het beveiligingslek bevindt zich echter in een Windows-bestand, Shell32.dll, dat onderdeel uitmaakt van alle ondersteunde edities van Windows XP en Windows Server 2003. |
| **Maximaal prioriteitsniveau**            | [Kritiek](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update wordt het systeem opnieuw opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Software waarin dit probleem optreedt** | **Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

Belangrijk (1)
--------------

<span></span>
| Bulletin-id                               | Microsoft Security Bulletin MS07-062                                                                                                                                                                                                                                                                                                                                           |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door een beveiligingslek in DNS is spoofing mogelijk (941672)**](http://technet.microsoft.com/security/bulletin/ms07-062)                                                                                                                                                                                                                                                   |
| **Samenvatting**                          | Door deze update met hoge prioriteit wordt een privé gemeld beveiligingslek opgelost. Dit beveiligingslek met betrekking tot spoofing komt voor in Windows DNS-servers en zou ertoe kunnen leiden dat een aanvaller speciaal vervaardigde antwoorden op DNS-aanvragen stuurt, waardoor internetverkeer van legitieme locaties kan worden omgeleid, of onderschept en vervalst. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                     |
| **Gevolgen van het beveiligingslek**      | Spoofing                                                                                                                                                                                                                                                                                                                                                                       |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Bij deze update is het opnieuw starten van het systeem vereist, behalve in bepaalde situaties.                                                                                                                                                                       |
| **Software waarin dit probleem optreedt** | **Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                |

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
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS07-061**](http://technet.microsoft.com/security/bulletin/ms07-061)
</td>
<td style="border:1px solid black;">
[**MS07-062**](http://technet.microsoft.com/security/bulletin/ms07-062)
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
</tr>
<tr>
<th colspan="3">
Windows-besturingssysteem
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Server Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=c80fcd9b-d0f8-44db-96fc-bf2ead054ff4)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=8ba1c2f9-1bde-4e97-b327-21259c5e5104)
</td>
<td style="border:1px solid black;">
** **
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=4ef7fdd7-8887-4c64-a70c-c6ae734d7c5f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=4ef7fdd7-8887-4c64-a70c-c6ae734d7c5f)
</td>
<td style="border:1px solid black;">
** **
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=e5d8a866-2c1f-4035-8325-c1be61a75c3b)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=ed8e2cb4-bcd9-40fc-9ad6-46b364d0656d)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=e5d8a866-2c1f-4035-8325-c1be61a75c3b)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=ed8e2cb4-bcd9-40fc-9ad6-46b364d0656d)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=bf26da08-15b8-4d65-ba12-4cc74c7a1326)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=d1323e14-ffa7-4d03-a2a7-9240c192a75e)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=bf26da08-15b8-4d65-ba12-4cc74c7a1326)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=d1323e14-ffa7-4d03-a2a7-9240c192a75e)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=1c055f11-3273-4a4c-a33f-bf61ac9ec4c5)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=f3ad67de-85ad-452d-a1e0-0af3faf969d6)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Kritiek](http://www.microsoft.com/downloads/details.aspx?familyid=1c055f11-3273-4a4c-a33f-bf61ac9ec4c5)
</td>
<td style="border:1px solid black;">
[Belangrijk](http://www.microsoft.com/downloads/details.aspx?familyid=f3ad67de-85ad-452d-a1e0-0af3faf969d6)
</td>
</tr>
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

**Opmerking** Na 9 oktober 2007 zal het bestand MSSecure.XML, dat door MBSA 1.2.1 wordt gebruikt, niet langer worden bijgewerkt. Na deze datum zullen geen nieuwe beveiligingsupdates worden toegevoegd aan het bestand MSSecure.XML, dat door MBSA 1.2.1 wordt gebruikt, en zullen geen nieuwe versies van Enterprise Scan Tool meer worden uitgegeven. Dit betreft niet de Security Update Inventory Tool (SUIT) of Extended Security Update Inventory Tool (ESUIT) voor SMS 2.0 en SMS 2003. Ga voor meer informatie naar [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134).

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders snel en betrouwbaar de nieuwste essentiële updates en beveiligingsupdates implementeren voor Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders met SMS 2003 beveiligingsupdates kunnen implementeren. SMS 2.0-gebruikers kunnen ook het [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) gebruiken voor de implementatie van beveiligingsupdates. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking:** SMS maakt gebruik van de Microsoft Baseline Security Analyzer en de Microsoft Office Detection Tool om brede ondersteuning te kunnen bieden voor het zoeken en uitvoeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:

Planning voor deze maand:

-   Microsoft heeft voor Microsoft Update (MU) en Windows Server Update Services (WSUS) drie belangrijke updates uitgegeven die **geen beveiligingsupdate** zijn.
-   Microsoft heeft geen belangrijke **niet-beveiligingsupdates** voor Windows op Windows Update (WU) vrijgegeven.

De informatie geldt **alleen** voor belangrijke **niet-beveiligingsupdates** op Microsoft Update, Windows Update en Windows Server Update Services, die op dezelfde dag als de samenvatting van de beveiligingsbulletins zijn uitgegeven. Er wordt **geen** informatie gegeven over **niet-beveiligingsupdates** die op andere dagen zijn uitgegeven.

#### Veiligheidsstrategieën en community

**Strategieën voor updatebeheer**

Op de website [Security Guidance for Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) kunt u extra informatie vinden over aanbevelingen van Microsoft voor het toepassen van beveiligingsupdates.

**Verkrijgen van andere beveiligingsupdates**

Op de volgende locaties zijn updates verkrijgbaar voor andere beveiligingsproblemen:

-   Beveiligingsupdates zijn verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.
-   Updates voor consumentenplatforms zijn verkrijgbaar op de website [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   U kunt de beveiligingsupdates van deze maand die op Windows Update staan, via het ISO CD-beeldbestand met beveiligingsupdates en essentiële updates vanaf het Microsoft Downloadcentrum ophalen. Zie [Microsoft Knowledge Base-artikel 913086](http://support.microsoft.com/kb/913086) voor meer informatie.

**IT Pro Security-community**

Leer de beveiliging te verbeteren en uw IT-infrastructuur te optimaliseren en bespreek beveiligingsonderwerpen met andere IT-professionals op de website [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Dankbetuiging

Microsoft [bedankt](http://go.microsoft.com/fwlink/?linkid=21127) de volgende partijen voor de samenwerking bij het verbeteren van de beveiliging voor klanten:

-   Jesper Johansson voor het samenwerken met ons aan een probleem dat in MS07-061 wordt beschreven
-   Carsten H. Eiram van [Secunia](http://corporate.secunia.com/) voor het samenwerken met ons aan een probleem dat in MS07-061 wordt beschreven
-   Aviv Raff van [Finjan](http://www.finjan.com/) voor het samenwerken met ons aan een probleem dat in MS07-061 wordt beschreven
-   Petko Petkov van [GNUCITIZEN](http://www.gnucitizen.org/) voor het samenwerken met ons aan een probleem dat in MS07-061 wordt beschreven
-   Alla Berzroutchko van [Scanit](http://www.scanit.be/) voor het melden van een probleem dat wordt beschreven in MS07-062
-   Amit Klein van [Trusteer](http://www.trusteer.com/) voor het melden van een probleem dat wordt beschreven in MS07-062

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (13 november 2007): Samenvatting van de gepubliceerde bulletins.

*Built at 2014-04-18T01:50:00Z-07:00*
