---
TOCTitle: 'Release-opmerkingen voor Windows Server Update Services 3.0 SP2'
Title: 'Release-opmerkingen voor Windows Server Update Services 3.0 SP2'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21798481
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Dd939886(v=WS.10)'
---

Release-opmerkingen voor Windows Server Update Services 3.0 SP2
===============================================================

In deze release-opmerkingen wordt de release van Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) beschreven. Dit document bevat de volgende secties:

1.  Nieuw in deze release
2.  Systeemvereisten voor de WSUS 3.0 SP2-serverinstallatie
3.  Configuratievereisten en aanbevolen procedures voor de WSUS-server
4.  Vereisten voor Windows Small Business Server
5.  Systeemvereisten voor de installatie van de externe console van WSUS 3.0 SP2
6.  Systeemvereisten voor de clientinstallatie
7.  Upgradevereisten en aanbevelingen
8.  WSUS 3.0 SP2 installeren
9.  Opdrachtregelparameters voor de onbeheerde installatie van WSUS 3.0 SP2
10. Bekende kwesties

Nieuw in deze release
---------------------

-   Integratie met Windows Server® 2008 R2.
-   Ondersteuning voor de functie BranchCache in Windows Server 2008 R2.
-   Ondersteuning voor Windows 7-clients.
-   Verbeteringen voor WUA-client (Windows Update Agent). De nieuwe WUA-client biedt een verzameling prestatieverbeteringen, verbeteringen voor de gebruikerservaring plus een aantal oplossingen voor problemen op basis van klantenfeedback.
    -   Het scannen van een client gaat sneller dan in eerdere versies.
    -   Op computers die door WSUS-servers worden beheerd kunnen nu, in plaats van een volledige scan uit te voeren, ‘gerichte’ scans op diezelfde WSUS-servers worden uitgevoerd.  Hierdoor worden scans voor toepassingen die gebruikmaken van Microsoft Update API' s, zoals Windows Defender, vele malen sneller.
    -   Door verbeteringen voor de gebruikerservaring van WUA W(indows Update Agent) kunnen gebruikers updates beter beheren en meer helderheid geven over de waarde en het gedrag van updates.
    -   Gerepliceerde computers worden duidelijker weergegeven in de WSUS-console. Raadpleeg voor meer informatie het artikel [Een Windows 2000-, Windows Server 2003- of Windows XP-computer met een Windows 2000-, Windows Server 2003- of Windows XP-kopie wordt niet in de WSUS-console weergegeven](http://go.microsoft.com/fwlink/?linkid=159749) (mogelijk in het Engels).
-   Nieuwe functies:
    -   Met regels voor automatische goedkeuring kunt u de deadlinedatum en -tijd voor de goedkeuring voor alle computers of specifieke computergroepen opgeven.
    -   De verbeterde taalselectie op downstreamservers bestaat uit een nieuw waarschuwingsdialoogvenster dat wordt weergegeven wanneer u alleen updates voor opgegeven talen wilt downloaden.
    -   Met nieuwe rapporten voor update- en computerstatus kunt u updates filteren die zijn goedgekeurd voor installatie. U kunt deze rapporten uitvoeren vanuit de WSUS-console of deze functionaliteit via de API (application programming interface) opnemen in uw eigen rapporten.
-   De gebruikersinterface is compatibel met Service Pack 1 en Service Pack 2 voor WSUS 3.0 op de client en de server.
-   Software-updates.
-   Bekende problemen met Windows Update Agent die in deze versie zijn opgelost:
    1.  WSUS 3.0 SP2 en Windows 7 bevatten een nieuwe versie van de Windows Update Agent (voor Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 en Windows Server 2008). In deze versie is het volgende probleem opgelost: API's die worden aangeroepen door niet-lokale systeemaanroepers in een niet-interactieve sessie, mislukken.
    2.  Probleem dat is opgelost in versie 7.2.6001.788 van Windows Update Agent. Met deze update wordt het volgende probleem opgelost: Wanneer u 80 of meer updates tegelijk installeert vanaf de webpagina Windows Update of de webpagina Microsoft Update, ontvangt u mogelijk de foutcode 0x80070057.
    3.  Verbeteringen en problemen die zijn opgelost in versie 7.2.6001.784 van Windows Update Agent. Deze update bevat de volgende verbeteringen: Verbeterde scantijden voor Windows Update, hogere snelheid waarmee handtekeningupdates worden geleverd, ondersteuning van functionaliteit voor het opnieuw installeren van Windows Installer en verbeterde foutberichten.

<span id="BKMK_SysReqWSUS30SP2"></span>
Systeemvereisten voor de WSUS 3.0 SP2-serverinstallatie
-------------------------------------------------------

In deze sectie worden de software- en hardwarevereisten beschreven die nodig zijn voor de installatie van WSUS 3.0 SP2.

### Softwarevereisten voor de WSUS-server

-   U moet een van de volgende ondersteunde besturingssystemen hebben geïnstalleerd:
    -   Windows Server 2008 R2
    -   Windows Server 2008 SP1 of latere versies
 
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Warning(WS.10).gif" />Waarschuwing</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Als WSUS 3.0 SP2 op Windows Server 2008 wordt geïnstalleerd voordat u een update uitvoert naar Windows Server 2008 R2, mislukt de upgrade naar Windows Server 2008 R2. Zie de sectie <a href="#bkmk_knownissues">Bekende kwesties</a> voor meer informatie.
        </td>
        </tr>
        </tbody>
        </table>
 

    -   Windows Server 2003 SP1 of latere versies
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Er gelden extra vereisten voor Windows Small Business Server. Zie de sectie 'Vereisten voor Windows Small Business Server' voor meer informatie.
-   Internet Information Services (IIS) 6.0 of latere versies
-   Microsoft .NET Framework 2.0 of latere versies
-   U moet een van de volgende ondersteunde databases hebben geïnstalleerd:
    -   Microsoft SQL Server 2008 Standard of Enterprise Edition
    -   Microsoft SQL Server 2005 SP3 of latere versies
    -   Interne Windows-database

    Als een van de ondersteunde versies van SQL Server niet is geïnstalleerd, wordt de interne Windows-database geïnstalleerd via de installatiewizard van WSUS 3.0 SP2.
-   Microsoft Management Console 3.0
-   Microsoft Report Viewer Redistributable 2008

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Belangrijk</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Voor Windows Server 2008 R2 is WSUS 3.0 SP2 vereist. Als u Windows Server 2008 R2 installeert, moet u WSUS 3.0 SP2 installeren. Installeer geen WSUS 3.0 SP1 onder Windows Server 2008 R2.

WSUS 3.0 SP2 wordt niet ondersteund voor gebruik met Terminal Services op de front-end server in een externe SQL-configuratie.
</td>
</tr>
</tbody>
</table>
 

### Softwarevereisten voor de WSUS-beheerconsole

-   Een van de volgende ondersteunde besturingssystemen: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 SP2 of latere versies, Windows Small Business Server 2008 of Windows Small Business Server 2003, Windows Vista of Windows XP SP2
-   Microsoft .NET Framework 2.0 of latere versies
-   Microsoft Management Console 3.0
-   Microsoft Report Viewer Redistributable 2008

### Minimale hardwarevereisten voor de WSUS-server

De volgende lijst bevat de minimale hardwarevereisten die nodig zijn voor een basisinstallatie van de server. Raadpleeg de installatiehandleiding van WSUS 3.0 SP2 op [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) voor een uitgebreide lijst met ondersteunde hardwareconfiguraties (mogelijk in het Engels).

-   Zowel de systeempartitie als de partitie waarop u WSUS 3.0 SP2 installeert, moeten zijn geformatteerd met het NTFS-bestandssysteem.
-   Minimaal 1 GB vrije ruimte op de systeempartitie.
-   Minimaal 2 GB vrije ruimte op het volume waarop databasebestanden worden opgeslagen.
-   Minimaal 20 GB vrije ruimte is vereist op het volume waarop de inhoud wordt opgeslagen. 30 GB wordt aanbevolen.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Belangrijk</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">WSUS 3.0 SP2 kan niet op gecomprimeerde stations worden geïnstalleerd.
</td>
</tr>
</tbody>
</table>
 

Configuratievereisten en aanbevolen procedures voor de WSUS-server
------------------------------------------------------------------

Controleer of u de toepasselijke taken in deze sectie hebt uitgevoerd voordat u WSUS 3.0 SP2 installeert.

### IIS

-   Installeer op de pagina Services voor functie van webserver (IIS) van Server Manager de vereiste functies, alle standaardfunctieservices van IIS en de volgende functieservices: **ASP.NET**, **Windows-verificatie**, **Dynamische inhoudcompressie** en **Compatibiliteit met IIS 6-beheer**.
-   Als IIS wordt uitgevoerd in de isolatiemodus van IIS 5.0, mislukt de installatie. Schakel de isolatiemodus van IIS 5.0 uit voordat u WSUS 3.0 SP2 installeert.
-   Als een onderdeel van IIS is geïnstalleerd in de 32-bits compatibiliteitsmodus op een 64-bits platform, kan de installatie van WSUS 3.0 SP2 mislukken. Alle onderdelen van IIS moeten worden geïnstalleerd in de native modus op 64-bits platforms.

### Proxyservers

In WSUS 3.0 SP2 kan een proxyserver alleen HTTP ondersteunen. U wordt aangeraden een tweede proxyserver met HTTPS te configureren via de opdrachtregel (**wsusutil configuresslproxy**) voordat u de WSUS-server configureert via de configuratiewizard of de beheerconsole.

### Websites die worden uitgevoerd op poort 80

Als u twee of meer websites uitvoert op poort 80 (bijvoorbeeld Windows SharePoint Services), moet u één website bewaren en de rest verwijderen voordat u WSUS installeert. Als u dit niet doet, kunnen de clients van de server mogelijk niet automatisch worden bijgewerkt.

### Antivirusprogramma's

Wanneer u WSUS 3.0 SP2 installeert, moet u mogelijk uw antivirusprogramma's uitschakelen voordat u de installatie kunt uitvoeren. Nadat u de antivirussoftware hebt uitgeschakeld, moet u de computer opnieuw opstarten voordat u WSUS installeert. Hiermee voorkomt u dat bestanden worden vergrendeld wanneer de installatieprocedure toegang zoekt tot de bestanden. Schakel het antivirusprogramma weer in wanneer u de installatie hebt voltooid. Bezoek de website van de leverancier van de antivirussoftware voor de exacte procedure voor het in- en uitschakelen van de antivirussoftware en voor de versiegegevens.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Caution(WS.10).gif" />Let op</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Door deze methode kan uw computer of het netwerk kwetsbaarder worden voor aanvallen door kwaadwillende gebruikers of schadelijke software, zoals virussen. Microsoft raadt deze methode niet aan, maar verschaft u deze informatie zodat u zelf kunt beslissen of u de methode al dan niet wilt uitvoeren. Het gebruik van deze methode is voor uw eigen risico.

Met antivirussoftware wordt uw computer beschermd tegen virussen. Download of open geen bestanden van bronnen die u niet vertrouwt, bezoek geen websites die u niet vertrouwt en open geen e-mailbijlagen wanneer uw antivirusprogramma is uitgeschakeld.
</td>
</tr>
</tbody>
</table>
 

### Optie voor geneste triggers in SQL Server

Als u een SQL Server-database wilt gebruiken als gegevensarchief voor Windows Server Update Services, moet de SQL Server-beheerder controleren of de optie voor geneste triggers is ingeschakeld voordat de WSUS-beheerder WSUS 3.0 SP2 installeert. Deze optie is standaard ingeschakeld, maar kan worden uitgeschakeld door een SQL Server-beheerder. Tijdens de installatie van WSUS 3.0 SP2 wordt de optie RECURSIVE\_TRIGGERS ingeschakeld. Dit is een databasespecifieke optie. De optie voor geneste triggers, een algemene serveroptie, wordt echter niet ingeschakeld via WSUS 3.0 SP2 Setup.

### Beperkingen en vereisten voor extern SQL

WSUS 3.0 SP2 ondersteunt het uitvoeren van een compatibele versie van SQL Server-software op een computer die gescheiden is van de computer waarop de WSUS 3.0 SP2-toepassing wordt uitgevoerd. De volgende vereisten gelden voor een externe SQL-installatie.

-   U kunt geen server gebruiken die is geconfigureerd als een domeincontroller voor het externe SQL-paar.
-   U kunt Terminal Services niet uitvoeren op de computer die fungeert als front-end server van een externe SQL-installatie.
-   De front-end computer en de back-end computer moeten zijn gekoppeld aan een Active Directory-domein. Als de front-end en back-end computers zich in verschillende domeinen bevinden, legt u een vertrouwensrelatie tussen de domeinen vast voordat u WSUS Setup uitvoert.
-   Als u WSUS 2.0 al hebt geïnstalleerd in een externe SQL-configuratie en u een upgrade wilt uitvoeren naar WSUS 3.0 SP2, voert u een van de volgende handelingen uit voordat u WSUS installeert:
    1.  Verwijder WSUS 2.0 (via **Software** in het Configuratiescherm) en zorg ervoor dat de bestaande database behouden blijft.
    2.  Installeer SQL Server 2005 SP2 of SQL Server 2008 en voer een upgrade uit op de bestaande database.

### IIS wordt opnieuw gestart tijdens de installatie van WSUS 3.0 SP2.

Door WSUS 3.0 SP2 te installeren wordt IIS zonder voorafgaande melding opnieuw gestart. Dit kan invloed hebben op bestaande websites binnen uw organisatie. U wordt aangeraden de relevante partijen van tevoren op de hoogte te stellen van deze installatie. Als IIS niet actief is, wordt dit tijdens de installatie gestart via WSUS 3.0 SP2 Setup.

Vereisten voor Windows Small Business Server
--------------------------------------------

Als u WSUS 3.0 SP2 installeert op Windows Small Business Server gelden de volgende vereisten.

### Als de virtuele hoofdmap voor IIS is beperkt tot bepaalde IP-adressen of domeinnamen

Bij sommige installaties van Windows Small Business Server is de standaard IIS-website geconfigureerd voor **IP-adres en domeinnaambeperkingen**. Als dit het geval is, kan de Windows Update-client op de server mogelijk niet worden bijgewerkt. Verwijder de beperking voordat u WSUS 3.0 SP2 installeert.

### Als u een ISA-proxyserver gebruikt

-   Als u voor Windows Small Business Server een ISA-proxyserver gebruikt voor toegang tot internet, typt u **proxyserverinstellingen, proxyservernaam, poort** in de gebruikersinterface (UI) **Instellingen**.
-   Als voor ISA Windows-verificatie wordt gebruikt, typt u de proxyserverreferenties in de notatie *DOMEIN*\\*gebruiker*. De gebruiker moet lid zijn van de groep Internetgebruikers.

### Als u een subnet hebt toegevoegd aan het netwerk en geen wizards van Windows Small Business Server hebt gebruikt

Tijdens de installatieprocedure van de WSUS-server worden twee virtuele hoofdmappen voor IIS op de server geïnstalleerd: SelfUpdate en ClientWebService. Daarnaast worden via Setup enkele bestanden in de hoofdmap geplaatst van de standaardwebsite (op poort 80) waarmee clientcomputers automatisch kunnen worden bijgewerkt via de standaardwebsite. De standaardwebsite is echter standaard zodanig geconfigureerd, dat deze elk IP-adres of elke localhost de toegang weigert, behalve de localhost of specifieke subnets van de server. Clientcomputers die zich niet op de localhost of op de specifieke subnets bevinden, kunnen dus niet automatisch worden bijgewerkt. Voer de volgende procedure uit als u een subnet aan het netwerk hebt toegevoegd zonder de wizards van Microsoft Windows Small Business Server te gebruiken:

1.  Vouw in Serverbeheer achtereenvolgens **Geavanceerd beheer**, **Internet Information Services**, **Websites** en **Standaardwebsite** uit, klik met de rechtermuisknop op de virtuele map **Selfupdate** en klik op **Eigenschappen**.
2.  Klik op **Mapbeveiliging**.
3.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik op **Toegang verleend**.
4.  Klik op **OK**, klik met de rechtermuisknop op de virtuele map **ClientWebService** en klik op **Eigenschappen**.
5.  Klik op **Mapbeveiliging**.
6.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik op **Toegang verleend**.

Systeemvereisten voor de installatie van de externe console van WSUS 3.0 SP2
----------------------------------------------------------------------------

U kunt de externe console van WSUS 3.0 SP2 installeren op een van de volgende besturingssystemen:

-   Windows Server 2008 R2, Windows Server 2008 SP1 of latere versies, Windows Server 2003 SP2 of latere versies, Windows Small Business Server 2003, Windows Small Business Server 2005 of Windows Small Business Server 2008, Windows Vista of Windows XP Professional SP3 of latere versies.

Systeemvereisten voor de installatie van de WSUS-client
-------------------------------------------------------

U kunt Automatische updates, de WSUS-clientsoftware, installeren op een van de volgende besturingssystemen:

-   Windows Server 2008 R2, Windows Server 2008 SP1 of latere versies, Windows Server 2003 SP2 of latere versies, Windows Small Business Server 2003, Windows Small Business Server 2005 of Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional SP1, Windows XP Professional SP2, Windows XP Professional SP3 of latere versies, Windows 2000 SP4 of Windows 7-client.

Upgradevereisten en aanbevelingen
---------------------------------

U kunt voor de volgende versies van WSUS een upgrade uitvoeren naar WSUS 3.0 SP2, waarbij u de eerdere versie niet hoeft te verwijderen:

-   WSUS 2.0, 2.0 SP1, 3.0 en 3.0 SP1.

Upgrades van WSUS 1.0 naar WSUS 3.0 SP2 worden niet ondersteund. Verwijder SUS (Software Update Services) 1.0 voordat u WSUS 3.0 SP2 installeert.

Voor Windows Server 2008 R2 is WSUS 3.0 SP2 vereist. Als u Windows Server 2008 R2 installeert, moet u WSUS 3.0 SP2 installeren. Installeer niet WSUS 3.0 SP1 onder Windows Server 2008 R2.

#### Voor u een upgrade uitvoert naar WSUS 3.0 SP2

1.  Controleer op recente fouten in de gebeurtenislogboeken, op problemen met de synchronisatie tussen downstream- en upstreamservers en op problemen met de clientrapportage. Los deze problemen op voordat u de upgrade uitvoert.

2.  U kunt ook DBCC CHECKDB uitvoeren om te controleren of de WSUS-database juist is geïndexeerd. Zie [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) voor meer informatie over DBCC CHECKDB.

3.  Maak een back-up van de WSUS-database. Tijdens de installatie van WSUS 3.0 SP2 wordt de nieuwe database toegevoegd aan de standaardmap: *station*\\WSUS (waarbij *station* het lokale NTFS-station met de grootste hoeveelheid beschikbare ruimte is). Als deze map al een databaseback-up bevat, wordt deze mogelijk overschreven. U wordt aangeraden een databaseback-up van de huidige versie van WSUS op een andere locatie op te slaan voordat u een upgrade uitvoert naar WSUS 3.0 SP2.

4.  Als u de poort die voor WSUS wordt gebruikt, handmatig hebt gewijzigd (waarbij u het hulpprogramma Wsusutil niet hebt gebruikt) en momenteel SUS 1.0 of WSUS 2.0 uitvoert, start u de standaardwebsite voordat u SUS 1.0 of WSUS 2.0 64-bits verwijdert.

5.  Als er actieve verbindingen zijn met een bestaande WSUS-database (bijvoorbeeld als SQL Server Management Studio is geopend) kan de installatie mislukken. Sluit alle verbindingen voordat u WSUS 3.0 SP2 installeert.

### Herstel na een mislukte upgrade

Voer een van de volgende taken uit als u een upgrade van een eerdere versie van WSUS uitvoert naar WSUS 3.0 SP2 en de upgrade mislukt (vanwege een andere reden dan een niet-ondersteunde upgrade vanuit SUS 1.0).

1.  Installeer de eerdere versie van WSUS opnieuw.
2.  Zet de database terug vanuit de gemaakte back-up voordat u de upgrade uitvoert. U kunt geen upgrade uitvoeren als er een WSUS 3.0 SP2-database van een eerdere installatie bestaat. In de meeste gevallen wordt automatisch een back-up gemaakt via WSUS. Zie het bestand WSUSSetup.log voor de locatie.
3.  Bekijk de logboekbestanden om de oorzaak van het probleem vast te stellen en op te lossen.
4.  Installeer WSUS 3.0 SP2.

### Als de computernaam wordt gewijzigd voordat de upgrade naar WSUS 3.0 SP2 wordt uitgevoerd, kan de upgrade mislukken

Als u de computernaam wijzigt nadat u WSUS 2.0 hebt geïnstalleerd en voordat u een upgrade naar WSUS 3.0 SP2 uitvoert, kan de upgrade mislukken.

Gebruik het volgende script om de groepen ASPNET en WSUS Administrators te verwijderen en vervolgens opnieuw toe te voegen. Voer de upgrade vervolgens opnieuw uit.

        ```

### Als u een migratie hebt uitgevoerd van MSDE naar SQL Server 2008 of SQL Server 2005 op WSUS 2.0, moet u een registerwaarde wijzigen.

Als u beschikt over een installatie van WSUS 2.0 en een migratie hebt uitgevoerd naar SQL Server 2008 of SQL Server 2005, moet u de waarde **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** wijzigen van 1 in 0. Als u dit niet doet voordat u de upgrade naar WSUS 3.0 SP2 uitvoert, mislukt de upgrade.

### Als u WSUS 3.0 SP2 verwijdert en de logboekbestanden behoudt, zijn hiervoor mogelijk niet de juiste machtigingen ingesteld wanneer WSUS 3.0 SP2 opnieuw wordt geïnstalleerd.

Als u WSUS 3.0 SP2 verwijdert, kunt u ervoor kiezen de logboekbestanden van de installatie te behouden. Wanneer u WSUS 3.0 SP2 opnieuw installeert, worden de machtigingen voor de oude logboekbestanden mogelijk verwijderd (meestal alleen voor WSUS-beheerders). U wordt aangeraden de machtigingen voor deze logboekbestanden te bevestigen na de installatie.

### Als WSUS 2.0-clients updates met de status Niet van toepassing bevatten, worden de updates even weergegeven als Onbekend na de upgrade naar WSUS 3.0 SP2.

Als een bestaande WSUS 2.0-server clients bevat met updates met de status **Niet van toepassing**, worden deze updates mogelijk kort weergegeven met de status **Onbekend** wanneer u een upgrade hebt uitgevoerd naar WSUS 3.0 SP2. De updatestatus wordt hersteld naar **Niet van toepassing** wanneer de volgende keer een scan wordt uitgevoerd op de client.

WSUS 3.0 SP2 installeren
------------------------

De stapsgewijze installatiehandleiding bij WSUS op [http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) bevat instructies voor het installeren van WSUS 3.0 SP2 via Windows Server Manager of het bestand WSUSSetup.exe.

Voor volledige informatie over de installatie en het gebruik van WSUS, raadpleegt u:

De installatiehandleiding bij WSUS op [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832).

De WSUS Operations Guide op [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838).

Opdrachtregelparameters voor de onbeheerde installatie van WSUS 3.0 SP2
-----------------------------------------------------------------------

Met het installatieprogramma via de opdrachtregel van WSUS kunt u een onbeheerde installatie van WSUS 3.0 SP2 uitvoeren. In de volgende tabel vindt u de opdrachtregelparameters voor de installatie van WSUS 3.0 SP2.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Optie</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Stille installatie uitvoeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Verwijderen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Vereisten controleren. Hiermee wordt het systeem gecontroleerd en worden ontbrekende vereisten gerapporteerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Opdrachtregelparameters en de beschrijvingen weergeven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Upgrade van de eerdere versie van WSUS. (Upgrades van SUS 1.0 worden niet ondersteund.) De enige geldige parameter met deze optie is /q (stille installatie). De enige geldige eigenschap met deze optie is DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
In de volgende tabel vindt u de opdrachtregeleigenschappen voor WSUS 3.0 SP2.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Eigenschap</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=inhoud lokaal gehost, 1=hosten op Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Pad naar map met inhoud. De standaardwaarde is <em>WSUSInstallationDrive\WSUS\WSUSContent</em>, waarbij <em>WSUSInstallationDrive</em> het lokale station met de grootste hoeveelheid beschikbare ruimte is.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Pad naar gegevensmap voor interne Windows-database.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">De naam moet in de volgende notatie worden opgegeven: <em>ServerName</em>\<em>SQLInstanceName</em>. Als de database-instantie op het lokale systeem staat, gebruikt u de omgevingsvariabele %COMPUTERNAME%. Als er geen instantie van de database op het systeem staat, is de variabele standaard %COMPUTERNAME%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=poort 8530, 1=poort 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Pad en bestandsnaam van logboekbestand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=de WSUS-server installeren, 1=alleen console installeren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=inventarisfuncties niet installeren, 1=inventarisfuncties installeren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=database behouden, 1=databasebestanden verwijderen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=inhoud behouden, 1=inhoudsbestanden verwijderen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=logboekbestanden behouden, 1=logboekbestanden verwijderen (gebruikt met de installatieschakeloptie /u)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=huidige database gebruiken, 1=database maken</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Vensteringang voor het retourneren van voortgangsberichten van Windows Installer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=deelnemen aan programma voor verbetering van de gebruikerservaring van Microsoft Update, 0=niet deelnemen aan programma voor verbetering van de gebruikerservaring van Microsoft Update</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=de locatie van de inhoud niet naar de database wegschrijven, 0=de locatie van de inhoud naar de database wegschrijven (voor NLB)</td>
</tr>
</tbody>
</table>
  
### Voorbeeld van gebruik
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (installeren in stille modus met poort 8530) WSUSSetup.exe /q /u (WSUS verwijderen)  
```
 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Belangrijk</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Als u WSUS 3.0 SP2 installeert in de stille modus (/q) en niet alle vereiste onderdelen op de computer zijn geïnstalleerd, wordt een bestand gegenereerd met de naam WSUSPreReqCheck.xml. Dit bestand wordt opgeslagen in de map %TEMP%.
</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_KnownIssues"></span>
Bekende kwesties
----------------

-   Wanneer de installatiewizard van WSUS is voltooid, wordt de gebruiker gevraagd op **Voltooien** te klikken. Een enkele keer wordt een foutdialoogvenster weergegeven met het volgende bericht: **Er is een fout opgetreden tijdens het communiceren met de server, en deze wizard moet worden gesloten. U kunt de wizard WSUS-server configureren opnieuw starten vanaf de pagina Opties in de WSUS-console.** Als u wilt controleren of de installatieselecties zijn opgeslagen, opent u de pagina **Opties** in de WSUS-beheerconsole en bevestigt u de instellingen in elke sectie.
-   **Gelokaliseerde versies van de WUA-client (Windows Update Agent) worden later uitgebracht dan de WSUS 3.0 SP2-versie**. Dit komt doordat dit afhankelijk is van de lokalisatieplanning van Windows 7. In de periode tussen de release van de WSUS 3.0 SP2  en van de gelokaliseerde versie van de WUA-client ondersteunt de WUA-client maar vijf talen (Engels, Duits, Frans, Spaans en Japans).
-   **De nieuwe rapporten voor update- en computerstatus die in deze SP2-versie zijn ingevoerd, werken niet in een omgeving waar downstream WSUS 3.0 SP1-servers worden beheerd vanaf een WSUS 3.0 SP2-server**. Als de nieuwe rapporten worden uitgevoerd voor een SP1-server wordt het volgende foutbericht weergegeven: Er is een fout opgetreden tijdens het genereren van het rapport. Probeer het rapport nogmaals uit te voeren of neem contact op met uw netwerkbeheerder als het probleem zich blijft voordoen. Het probleem wordt niet opgelost door het rapport opnieuw uit te voeren en het is ook niet netwerk-gerelateerd. De nieuwe rapporten hangen af van API-functionaliteit die niet bestaat in SP1. De beheerconsole van SP2 blokkeert de nieuwe rapporten niet wanneer deze een SP1-server beheert.
-   **Het uitvoeren van een update naar WSUS 3.0 SP2 mislukt wanneer SSL wordt geconfigureerd zonder certificaatnaam**. Bij het configureren van SSL is een certificaatnaam vereist.
-   **Als WSUS 3.0 SP2 Windows Internal Database uitvoert en op Windows Server 2008 is geïnstalleerd, wordt het uitvoeren van een update naar Windows Server 2008 R2** voorkomen. Voor u doorgaat met het uitvoeren van de update naar Windows Server 2008 R2 wordt een foutbericht van het compatibiliteitsrapport weergegeven, waarin u wordt gevraagd de Windows Internal Database uit te schakelen. Het is noodzakelijk Windows Internal Database bij te werken voordat de upgrade naar Windows Server 2008 R2 kan worden voortgezet. Raadpleeg [Het meest recente servicepack voor interne Windows-database ophalen](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104) voor instructies en meer informatie over upgraden Windows Internal Database (mogelijk in het Engels).

Copyrightvermelding
-------------------

De informatie in dit document, URL's en andere verwijzingen naar websites op internet inbegrepen, is onderhevig aan wijziging zonder voorafgaande kennisgeving. Tenzij anders vermeld, zijn alle in de voorbeelden in dit document vermelde bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen fictief. Eventuele overeenkomsten met bestaande bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen berusten geheel op toeval. De gebruiker is verantwoordelijk voor naleving van alle geldende wetten inzake auteursrecht. Behoudens de in of krachtens de Auteurswet van 1912 gestelde uitzonderingen mag niets uit deze uitgave worden verveelvoudigd en/of openbaar gemaakt door middel van druk, fotokopie, microfilm of op welke andere wijze dan ook en evenmin in een gegevensopzoeksysteem worden opgeslagen zonder voorafgaande schriftelijke toestemming van Microsoft Corporation.

Microsoft is mogelijk in het bezit van octrooien, aanvragen voor octrooien, merken, auteursrechten of andere intellectuele eigendomsrechten met betrekking tot materiaal in dit document. De aanschaf van dit document geeft u geen licentie ten aanzien van deze octrooien, merken, auteursrechten of andere intellectuele eigendomsrechten, tenzij expliciet vermeld in een schriftelijke gebruiksrechtovereenkomst van Microsoft.

© 2009 Microsoft Corporation. Alle rechten voorbehouden.

Microsoft, Active Directory, ActiveX, Authenticode, Excel, InfoPath, Internet Explorer, MSDN, Outlook, Visual Studio, Win32, Windows, Windows Server en Windows Vista zijn handelsmerken van de Microsoft-groep van bedrijven.

Alle andere merken zijn eigendom van hun respectieve eigenaren.
