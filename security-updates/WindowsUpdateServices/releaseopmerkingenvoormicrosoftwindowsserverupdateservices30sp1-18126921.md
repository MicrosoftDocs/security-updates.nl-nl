---
TOCTitle: 'Releaseopmerkingen voor Microsoft Windows Server Update Services 3.0 SP1'
Title: 'Releaseopmerkingen voor Microsoft Windows Server Update Services 3.0 SP1'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18126921
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708525(v=WS.10)'
---

Releaseopmerkingen voor Microsoft Windows Server Update Services 3.0 SP1
========================================================================

In deze releaseopmerkingen zijn bekende problemen beschreven die van invloed zijn op Microsoft® WSUS (Windows® Server Update Services) 3.0 Service Pack 1. Daarnaast bevatten deze releaseopmerkingen aanbevelingen en vereisten voor het installeren van de toepassing. Deze releaseopmerkingen bevatten de volgende secties:

-   Systeemvereisten voor de serverinstallatie van WSUS 3.0 SP1
-   Configuratievereisten voor de serverinstallatie van WSUS 3.0 SP1
-   Systeemvereisten voor de installatie van de externe console van WSUS 3.0 SP1
-   Systeemvereisten voor de clientinstallatie
-   Softwarevereisten voor de serverinstallatie van WSUS SP1
-   Minimale schijfruimtevereisten voor de serverinstallatie van WSUS 3.0 SP1
-   WSUS 3.0 SP1-upgradevereisten
-   Opdrachtregelparameters voor de installatie
-   Installatieproblemen
-   Upgradeproblemen
-   Bekende problemen
-   WSUS 3.0 SP1 onder Windows Server® 2008
-   WSUS 3.0 SP1 onder Windows Small Business Server 2003

Systeemvereisten voor de serverinstallatie van WSUS 3.0 SP1
-----------------------------------------------------------

#### De WSUS 3.0 SP1-server wordt ondersteund onder Windows Server 2008 en Windows Server 2003 Service Pack 1

De WSUS 3.0 SP1-server wordt ondersteund door Windows Server 2008 en Windows Server 2003 Service Pack 1.

#### Windows 2000 Server biedt geen ondersteuning voor WSUS 3.0 SP1-servers

Het besturingssysteem Microsoft Windows® 2000 Server biedt geen ondersteuning voor WSUS 3.0 SP1-servers.

#### WSUS 3.0 SP1 wordt niet ondersteund op servers waarop Terminal Services wordt uitgevoerd

WSUS 3.0 SP1 kan mogelijk wel worden uitgevoerd op servers waarop Terminal Services wordt uitgevoerd, maar hiervoor wordt geen ondersteuning geboden. Het uitvoeren van WSUS 3.0 SP1 op servers waarop Terminal Services wordt uitgevoerd, wordt bovendien afgeraden. WSUS 3.0 SP1 kan niet worden uitgevoerd op servers met Terminal Services die zijn geconfigureerd voor het gebruik van externe SQL Server-implementaties. De installatie zal in een dergelijk geval mogelijk mislukken omdat alle externe aangepaste acties (waaronder de installatie) op een Terminal Services-licentieserver worden uitgevoerd met de systeemaccount, terwijl de systeemaccount van de server mogelijk niet over de juiste machtigingen voor de externe SQL Server beschikt

Configuratievereisten voor de serverinstallatie van WSUS 3.0 SP1
----------------------------------------------------------------

#### IIS moet zijn geïnstalleerd

Voor WSUS 3.0 SP1 is IIS (Internet Information Services) vereist. Deze software wordt onder Windows Server 2008 of Microsoft Windows Server 2003 standaard niet geïnstalleerd. Als u probeert om WSUS 3.0 SP1 te installeren terwijl IIS niet is geïnstalleerd, geeft het installatieprogramma van Windows Server Update Services een foutbericht weer waarin wordt vermeld dat IIS niet is geïnstalleerd.

#### Als IIS in de IIS 5.0-isolatiemodus wordt uitgevoerd, zal de installatie mislukken

Als u voor de server een upgrade hebt uitgevoerd van Windows 2000 Server naar Windows Server 2003, wordt IIS mogelijk uitgevoerd in de IIS 5.0-compatibiliteitsmodus. De IIS 5.0-isolatiemodus kan worden ingeschakeld via IIS-beheer. Als u dit doet, leidt dat tot het mislukken van de installatie. U moet de IIS 5.0-isolatiemodus uitschakelen voordat u WSUS 3.0 SP1 installeert.

#### Als IIS-onderdelen in de 32-bitscompatibiliteitsmodus op een 64-bitsplatform zijn geïnstalleerd, kan de installatie van WSUS 3.0 SP1 mogelijk mislukken

Alle IIS-onderdelen moeten op 64-bits platforms in de native modus worden geïnstalleerd. De installatie kan mislukken als er IIS-onderdelen zijn die in de 32-bitscompatibiliteitsmodus zijn geïnstalleerd.

#### Proxyservers bieden mogelijk alleen ondersteuning voor HTTP of HTTP en HTTPS

Het is in WSUS 3.0 SP1 mogelijk dat een proxyserver alleen ondersteuning biedt voor HTTP. Voordat u de WSUS-server via de configuratiewizard of de beheerconsole configureert, moet u een tweede proxyserver configureren voor HTTPS. Gebruik hiertoe de opdrachtregel (**wsusutil configuresslproxy**).

#### Als twee of meer websites reeds gebruikmaken van poort 80, moet u deze op één na alle verwijderen voordat u WSUS installeert

Als u over twee of meer websites beschikt die gebruikmaken van poort 80 (bijvoorbeeld Windows® SharePoint® Services), moet u deze op één na alle verwijderen voordat u WSUS installeert. Als u dit nalaat, worden de clients van de server mogelijk niet automatisch bijgewerkt.

#### Wanneer u WSUS 3.0 SP1 installeert, moet u mogelijk uw antivirussoftware uitschakelen

Wanneer u WSUS 3.0 SP1 installeert, moet u mogelijk uw antivirussoftware uitschakelen voordat u de installatie kunt uitvoeren. Start nadat u uw antivirussoftware hebt uitgeschakeld, de computer eerst opnieuw op voordat u WSUS installeert. U voorkomt door de computer opnieuw op te starten dat bestanden vergrendeld zijn op het moment dat het installatieproces over toegang tot deze bestanden moet beschikken. Schakel nadat de installatie is voltooid, uw antivirussoftware opnieuw in. Bezoek de website van de leverancier van uw antivirussoftware voor informatie over de exacte procedure voor het uitschakelen en het opnieuw inschakelen van uw versie van de desbetreffende antivirussoftware.

| ![](/security-updates/images/Cc708525.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Deze tijdelijke oplossing maakt uw computer of netwerk kwetsbaarder voor aanvallen van kwaadwillenden en/of voor aanvallen via schadelijke software, zoals virussen. Het gebruik van deze tijdelijke oplossing wordt niet aanbevolen. Deze informatie wordt slechts verschaft met het doel u in staat te stellen om een dergelijke tijdelijke oplossing naar eigen goeddunken wel of niet te implementeren. Het gebruik van deze tijdelijke oplossing is geheel voor eigen risico. |

| ![](/security-updates/images/Cc708525.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antivirussoftware is ontworpen met het oogmerk om uw computer tegen virussen te beschermen. U moet wanneer uw antivirussoftware is uitgeschakeld, geen bestanden downloaden of openen van bronnen die u niet vertrouwt. Daarnaast moet u geen websites bezoeken die u niet vertrouwt en u moet geen e-mailbijlagen openen. |

#### Het is voor WSUS 3.0 SP1 noodzakelijk dat de optie voor geneste triggers in SQL Server is ingeschakeld

Deze optie is standaard ingeschakeld, maar kan door een SQL Server-beheerder worden uitgeschakeld.

Wanneer u van plan bent om een SQL Server-database te gebruiken als het gegevensarchief voor Windows Server Update Services, moet de SQL Server-beheerder controleren of de optie voor geneste triggers is uitgeschakeld voordat de WSUS 3.0 SP1-beheerder WSUS 3.0 SP1 installeert en de database instelt als het gegevensarchief.

Het installatieprogramma van WSUS 3.0 SP1 schakelt de optie RECURSIVE\_TRIGGERS in. Dit is een databasegebonden optie. De optie voor geneste triggers wordt echter niet ingeschakeld. Dit is een algemene serveroptie.

U kunt als volgt controleren of de optie voor geneste triggers is ingeschakeld:

**sp\_configure 'nested triggers'**

Voer de volgende opdracht uit via een batchbestand op de computer waarop SQL Server wordt uitgevoerd om de optie voor geneste triggers in SQL Server in te schakelen:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Als SQL Server Management Studio niet op uw server is geïnstalleerd, is het raadzaam om SQL-scripts vanaf de opdrachtregel uit te voeren. U kunt het hulpprogramma Microsoft SQL Server 2005 Command Line Query downloaden via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). Als u het programma wilt starten, voert u **sqlcmd** uit.

Als u voor het uitvoeren van SQL-scripts gebruik wilt maken van Windows Internal Database, moet u SQL Server Native Client downloaden. U vindt deze software op dezelfde downloadpagina.

#### Beperkingen en vereisten met betrekking tot externe SQL-installaties

WSUS 3.0 SP1 biedt ondersteuning voor de mogelijkheid om de databasesoftware op een andere computer uit te voeren dan de rest van de WSUS 3.0 SP1-toepassing. Er is een aantal vereisten voor het configureren van een externe SQL-installatie:

-   U kunt geen server gebruiken die is geconfigureerd als een domeincontroller voor de back-end van het externe SQL-paar.
-   Terminal Server mag niet worden uitgevoerd op de computer die zal fungeren als de front-end-server van een externe SQL-installatie.
-   U moet voor de databasesoftware op de back-end-computer minimaal gebruikmaken van Microsoft SQL Server 2005 Service Pack 1 (verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143) als op deze computer Windows Server 2003 en SQL Server 2005 Service Pack 2 worden uitgevoerd wanneer het een back-end-computer met Windows Server® 2008 betreft.
-   Zowel de front-end-computer als de back-end-computer moet met een Active Directory-domein zijn verbonden. Als beide computers zich in verschillende domeinen bevinden, moet u tussen de desbetreffende domeinen een vertrouwensrelatie tot stand brengen voordat u het WSUS-installatieprogramma uitvoert.
-   Als u een upgrade naar WSUS 3.0 SP1 wilt uitvoeren in gevallen waarin WSUS 2.0 reeds met gebruik van een externe SQL-configuratie is geïnstalleerd, moet u WSUS 2.0 (via het onderdeel **Software** van het Configuratiescherm) van de back-end-computer verwijderen. U moet er tegelijkertijd voor zorgen dat de bestaande database intact blijft. Vervolgens moet u SQL Server 2005 SP1 of SP2 installeren en een upgrade van de bestaande database uitvoeren. Installeer ten slotte WSUS 3.0 SP1 op de front-end-computer.

Systeemvereisten voor de installatie van de externe console van WSUS 3.0 SP1
----------------------------------------------------------------------------

De externe console van WSUS 3.0 SP1 kan op de volgende platforms worden geïnstalleerd:

-   Windows Server 2008
-   Windows Vista® of hoger
-   Windows Server 2003 SP1 of hoger
-   Windows XP SP2 of hoger

Systeemvereisten voor de clientinstallatie
------------------------------------------

Automatische updates van de WSUS-clientsoftware. Hiertoe kan WSUS met de volgende besturingssystemen worden gebruikt:

-   Windows Vista of hoger
-   Windows Server 2008 of hoger
-   Microsoft Windows Server 2003 (elke editie)
-   Microsoft Windows XP Professional SP2 of hoger
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 of Windows 2000 Advanced Server met SP4

Softwarevereisten voor de serverinstallatie van WSUS 3.0 SP1
------------------------------------------------------------

In de volgende tabel wordt de vereiste software voor Windows Server 2003 SP1-platforms weergegeven. Vereiste software voor Windows Server 2008 komt aan bod in de sectie waarin het gebruik wordt beschreven van WSUS 3.0 SP1 onder Windows Server 2008.

Controleer of de WSUS 3.0 SP1-server aan deze lijst met vereisten voldoet voordat u het installatieprogramma van WSUS 3.0 SP1 uitvoert. Als het bij een of meer van deze updates noodzakelijk is dat de computer opnieuw wordt opgestart zodra de installatie is voltooid, moet u de computer opnieuw opstarten voordat u WSUS 3.0 SP1 installeert.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Vereiste</th>
<th style="border:1px solid black;" >Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Installeer deze software via het besturingssysteem.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package</td>
<td style="border:1px solid black;">Zie de informatie over Microsoft .NET Framework Version 2.0 Redistributable Package (x86) op de <a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=68935). Zie de informatie over Microsoft .NET Framework Version 2.0 Redistributable Package (x64) op de <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=70637)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0 voor Windows Server 2003</td>
<td style="border:1px solid black;">Dit is een vereiste voor het gebruik van de WSUS 3.0 SP1-gebruikersinterface. Zie de informatie over Microsoft Management Console 3.0 voor Windows Server 2003 (KB907265) op de <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=70412). Bij 64-bitsplatforms: zie de informatie over Microsoft Management Console 3.0 voor Windows Server 2003 x64 Edition (KB907265) op de <a href="http://go.microsoft.com/fwlink/?linkid=70638">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=70412).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dit is een vereiste voor het gebruik van de WSUS 3.0 SP1-gebruikersinterface. Zie de informatie over Microsoft Report Viewer Redistributable 2005 op de <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (optioneel)</td>
<td style="border:1px solid black;">WSUS 3.0 SP1 installeert Windows Internal Database als er geen compatibele versie van SQL Server is geïnstalleerd. Als u van plan bent om een volwaardige SQL Server-database te gebruiken, moet u (ten minste) gebruikmaken van SQL Server 2005 SP1 (verkrijgbaar via het <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Downloadcentrum</a> (http://go.microsoft.com/fwlink/?LinkId=66143) wanneer het een installatie onder Windows Server 2003 betreft of van SQL Server 2005 SP2 (verkrijgbaar via het <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Downloadcentrum</a> (http://go.microsoft.com/fwlink/?LinkId=84823) wanneer het een installatie onder Windows Server 2008 betreft.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc708525.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                           |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Het WSUS 3.0 SP1-installatieprogramma installeert Windows® Internal Database en migreert vervolgens de database bij gevallen waarin WSUS 2.0 reeds is geïnstalleerd en als WSUS 2.0 daarbij gebruikmaakt van SQL Server 2000, SQL Server Desktop Engine 2000 of van een SQL Server-database die ouder is dan SQL Server 2005 SP1 (of SQL Server 2005 SP2 onder Windows Server 2008). |
  
Minimale schijfruimtevereisten voor de serverinstallatie van WSUS 3.0 SP1  
-------------------------------------------------------------------------
  
Hierna worden de minimale schijfruimtevereisten voor de installatie van Windows Server Update Services weergegeven:
  
-   1 GB op de systeempartitie  
-   2 GB voor het volume waarop de databasebestanden worden opgeslagen  
-   20 GB voor het volume waarop de inhoud wordt opgeslagen
  
| ![](/security-updates/images/Cc708525.Important(WS.10).gif)Belangrijk                                                                       |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0 SP1 kan niet op een gecomprimeerd station worden geïnstalleerd. Ga na of het station waarop u de software wilt installeren, is gecomprimeerd. |
  
WSUS 3.0 SP1-upgradevereisten  
-----------------------------
  
#### Controleer of de WSUS-installatie op de juiste wijze wordt uitgevoerd en maak een back-up van de WSUS-database voordat u een upgrade uitvoert
  
Als u een upgrade naar WSUS 3.0 SP1 uitvoert vanaf een vorige versie van deze software, moet u controleren of de huidige installatie op de juiste wijze wordt uitgevoerd. Maak vervolgens voordat u de upgrade uitvoert, een back-up van de WSUS-database.
  
1.  Controleer de gebeurtenislogboeken en ga na of er sprake is van recente fouten, van synchronisatieproblemen tussen stroomafwaartse en stroomopwaartse servers of van problemen met clients die niet rapporteren. Zorg ervoor dat dergelijke problemen zijn verholpen voordat u doorgaat.  
2.  Het is verstandig om DBCC CHECKDB uit te voeren, zodat u kunt nagaan of de WSUS-database op de juiste wijze is geïndexeerd. Zie [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948) voor meer informatie over DBCC CHECKDB.  
3.  Maak een back-up van de WSUS-database.
  
#### Als u de poort hebt gewijzigd die door WSUS wordt gebruikt, moet u de software installeren voordat u een upgrade uitvoert
  
Wanneer u de poort voor WSUS aanpast, moet u daartoe gebruikmaken van het hulpprogramma WSUSUTIL. Het wordt afgeraden om de poort handmatig te wijzigen. Als u de poort handmatig hebt aangepast en als u reeds eerder een upgrade van Software Update Services 1.0 naar WSUS 2.0 hebt uitgevoerd:
  
1.  Als u WSUS 3.0 nog niet hebt geïnstalleerd, moet u WSUS 2.0 verwijderen. Zorg er daarbij voor dat de database en de inhoud behouden blijven. (Als u WSUS 3.0 reeds hebt geïnstalleerd, moet u WSUS 3.0 verwijderen. Zorg er daarbij voor dat de database en de inhoud behouden blijven).  
2.  Start de standaardwebsite, schakel SUS 1.0 tijdelijk opnieuw in en zorg ervoor dat deze software toegankelijk is voor het programma waarmee de installatie wordt verwijderd (de zogeheten uninstaller).  
3.  Verwijder SUS 1.0.  
4.  Installeer WSUS 3.0.
  
#### Software Update Services 1.0 moet worden verwijderd
  
De installatie van WSUS 3.0 SP1 zal mislukken als Software Update Services 1.0 op dezelfde machine is geïnstalleerd. U moet Software Update Services 1.0 verwijderen voordat u WSUS 3.0 SP1 installeert.
  
#### Het is niet mogelijk om onder een 64-bitsbesturingssysteem een upgrade van WSUS 2.0 naar WSUS 3.0 SP1 uit te voeren
  
WSUS 2.0 wordt niet ondersteund onder 64-bitsbesturingssystemen. Het is niet mogelijk om onder een 64-bitsbesturingssysteem een upgrade van WSUS 2.0 naar WSUS 3.0 SP1 uit te voeren.
  
Opdrachtregelparameters voor de installatie  
-------------------------------------------
  
U kunt WSUS 3.0 SP1-installaties zonder toezicht uitvoeren met behulp van het WSUS-installatieprogramma voor installaties vanaf de opdrachtregel. In de volgende tabel worden de opdrachtregelparameters voor het installatieprogramma van WSUS 3.0 SP1 weergegeven.
  
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
<td style="border:1px solid black;">Een installatie op de achtergrond uitvoeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Het product verwijderen. Indien er een exemplaar van Windows Internal Database is geïnstalleerd, wordt dit ook verwijderd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Controleren of het systeem aan de vereisten voldoet. Het product wordt niet geïnstalleerd. Het systeem wordt geïnspecteerd en eventuele gedetecteerde vereisten waaraan het systeem niet voldoet, worden gerapporteerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">De opdrachtregelparameters en de bijbehorende beschrijvingen weergeven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Een upgrade vanaf de vorige versie van WSUS uitvoeren. (U moet niet proberen om een upgrade uit te voeren vanaf SUS 1.0). De enige geldige parameter bij deze optie is /q (installatie op de achtergrond). De enige geldige eigenschap bij deze optie is DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
In de volgende tabel worden de opdrachtregeleigenschappen voor WSUS 3.0 SP1 weergegeven.
  
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
<td style="border:1px solid black;">0=inhoud op lokale host, 1=host op Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Het pad naar de inhoudmap. De standaardwaarde is <em>WSUS-installatiestation</em><strong>\WSUS\WSUS-inhoud</strong>, waarbij <em>WSUS-installatiestation</em> staat voor het lokale station met de grootste hoeveelheid vrije schrijfruimte.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Het pad naar de gegevensmap van Windows Internal Database.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">De naam moet worden weergegeven in de notatie <em>Servernaam</em>\<em>naam van SQL-exemplaar</em>. Als het database-exemplaar zich op de lokale computer bevindt, kunt u de omgevingsvariabele %COMPUTERNAAM% gebruiken. Als er geen bestaand exemplaar aanwezig is, is de standaardwaarde %COMPUTERNAAM%\WSUS.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=poort 8530, 1=poort 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Het pad en de bestandsnaam van het logboekbestand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=de WSUS-server installeren, 1=alleen de console installeren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=inventarisatiefuncties niet installeren, 1=inventarisatiefuncties installeren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=database behouden, 1=database verwijderen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=inhoudbestanden behouden, 1=inhoudbestanden verwijderen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=logboekbestanden behouden, 1=logboekbestanden verwijderen (wordt gebruikt met de installatieparameter /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=huidige database gebruiken, 1=database maken</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Window-koppeling voor het retourneren van MSI-voortgangsberichten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=aanmelden voor het Microsoft Update-programma voor kwaliteitsverbetering, 0=niet aanmelden voor het Microsoft Update-programma voor kwaliteitsverbetering</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=de inhoudlocatie niet naar de database schrijven, 0=de inhoudlocatie naar de database schrijven (voor NLB)</td>
</tr>
</tbody>
</table>
  
#### Voorbeeld van het gebruik
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](/security-updates/images/Cc708525.Important(WS.10).gif)Belangrijk                                                                                                                                                                                    |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u WSUS 3.0 SP1 in de stille modus (/q) installeert, terwijl niet alle vereiste software op de machine is geïnstalleerd, wordt er tijdens de installatie een bestand met de naam WSUSPreReqCheck.xml gegenereerd. Dit bestand wordt opgeslagen in de map %TEMP%. |
  
Installatieproblemen  
--------------------
  
#### IIS wordt tijdens de installatie van WSUS 3.0 SP1 opnieuw gestart
  
ISS wordt door het installatieprogramma van WSUS 3.0 SP1 zonder voorafgaande melding opnieuw gestart. Dit kan van invloed zijn op bestaande websites binnen uw organisatie. Als IIS niet wordt uitgevoerd, wordt deze software door het installatieprogramma van WSUS 3.0 SP1 gestart.
  
#### Als er sprake is van geopende verbindingen met een bestaande WSUS-database, zal de installatie mogelijk mislukken
  
Als u vanaf een bestaande installatie een upgrade naar WSUS 3.0 SP1 uitvoert terwijl er sprake is van geopende verbindingen met de bestaande WSUS-database (bijvoorbeeld wanneer SQL Server Management Studio is geopend), zal de installatie mogelijk mislukken. Verbreek alle verbindingen en installeer WSUS 3.0 SP1 opnieuw.
  
#### Het installatieprogramma van WSUS geeft een verkeerde map voor de databasebestanden weer
  
In het installatieprogramma van WSUS wordt in het scherm **Gereed voor installatie** ten onrechte vermeld dat de databaselocatie zich bevindt in de hoofdmap van de databaselocatie. Wanneer de standaardlocatie bijvoorbeeld %systeemstation%\\WSUS\\databasebestandenvanUpdateServices is, wordt de locatie %systeemstation%\\WSUS weergegeven.
  
#### De Help wordt weergegeven in de standaardtaal in plaats van in het Nederlands als WSUS is geïnstalleerd op een machine met andere talen voor de meertalige gebruikersinterface dan het Nederlands
  
Als WSUS is geïnstalleerd op een machine met andere taalpakketten voor de meertalige gebruikersinterface dan het taalpakket voor het Nederlands, kunt u WSUS toch installeren wanneer de lokale instelling van de gebruiker Nederlands is. De gebruikersinterface wordt in dat geval weergegeven in het Nederlands, maar voor de Help is een tijdelijke oplossing nodig als u deze in het Nederlands wilt weergeven. Kopieer het Nederlandstalige CHM-bestand voor de Help (*WSUSInstallDir*\\documentatie\\mui\\0409\\WSUS30Help.chm) naar de hoofdmap voor de documentatie (*WSUSInstallDir*\\documentatie\\WSUS30Help.chm). Vervolgens wordt de Help voor alle talen op de juiste wijze weergegeven.
  
Upgradeproblemen  
----------------
  
#### Herstellen na een mislukte upgrade
  
Als de upgrade om welke reden dan ook mislukt wanneer u vanaf een vorige versie van WSUS (WSUS 3.0, WSUS 2.0 SP1 of WSUS 2.0) een upgrade naar WSUS 3.0 SP1 uitvoert:
  
1.  Installeer de vorige versie van WSUS opnieuw.  
2.  Herstel de database met behulp van de back-up die u hebt gemaakt voordat u hebt geprobeerd om de upgrade uit te voeren. (In de meeste gevallen wordt er door WSUS automatisch een back-up gemaakt. Zie het bestand WSUSSetup.log voor de locatie).  
3.  Controleer de logboeken, zodat u de oorzaak van het mislukken kunt achterhalen en corrigeer het probleem.  
4.  Probeer opnieuw of u de WSUS-upgrade kunt uitvoeren.
  
#### Het is niet mogelijk om een upgrade van WSUS 2.0 naar WSUS 3.0 SP1 uit te voeren als er een WSUS 3.0 SP1-database uit een vorige installatie bestaat
  
Als u WSUS 3.0 SP1 reeds eerder hebt geïnstalleerd en als u WSUS 2.0 vervolgens opnieuw hebt geïnstalleerd, moet u de WSUS 3.0 SP1-database van de desbetreffende machine verwijderen voordat u probeert om WSUS 3.0 SP1 opnieuw te installeren.
  
#### Wanneer u de computernaam wijzigt voordat u een upgrade naar WSUS 3.0 SP1 uitvoert, kan dat ertoe leiden dat de upgrade mislukt
  
De upgrade kan mislukken als u de computernaam wijzigt voordat u een upgrade naar WSUS 3.0 SP1 uitvoert en nadat u WSUS 2.0 hebt geïnstalleerd.
  
Gebruik het volgende script om de groepen ASPNET en WSUS-administrators te verwijderen en opnieuw toe te voegen. Voer de upgrade vervolgens opnieuw uit.
  
U moet *&lt;databaselocatie&gt;* vervangen door de map waarin de database is geïnstalleerd en u moet *&lt;inhoudmap&gt;* vervangen door de lokale opslagmap.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Het installatieprogramma zal de vorige databaseback-up overschrijven
  
Het installatieprogramma van WSUS 3.0 SP1 zal de database toevoegen aan de standaardmap. Dit is de map *station*\\WSUS (waarbij *station* staat voor het lokale NTFS-station dat over de grootste hoeveelheid vrije schrijfruimte beschikt). Als deze map een databaseback-up bevat, wordt deze mogelijk overschreven. Beheerders moet een databaseback-up van de huidige versie opslaan op een andere locatie voordat ze een upgrade naar WSUS 3.0 SP1 uitvoeren.
  
#### Als u voor een WSUS 2.0-installatie een migratie van MSDE naar SQL Server 2000 of SQL Server 2005 uitvoert, moet u een registerwaarde wijzigen
  
Als u over een WSUS 2.0-installatie beschikt en als u een migratie vanaf SQL Server 2000 of SQL Server 2005 hebt uitgevoerd, moet u de waarde van **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** wijzigen van 1 in 0. Als u dit niet hebt gedaan voordat u een WSUS 3.0 SP1 uitvoert, zal de upgrade mislukken.
  
#### Als het installatieprogramma van WSUS 2.0 wordt gestart en geannuleerd, wordt de WSUS-registersleutel verwijderd
  
Als u het installatieprogramma van WSUS 2.0 start en vervolgens annuleert, wordt de WSUS-registersleutel verwijderd. Dit veroorzaakt mogelijk problemen als u WSUS 3.0 SP1 reeds hebt geïnstalleerd. Hetzelfde probleem treedt op als u het verwijderen van WSUS 2.0 start en annuleert en als u vervolgens probeert om een upgrade van WSUS 2.0 naar WSUS 3.0 SP1 uit te voeren.
  
#### Als u WSUS 3.0 SP1 verwijdert, terwijl de logboekbestanden blijven bestaan, beschikken deze mogelijk niet over de juiste machtigingen nadat de installatie opnieuw is uitgevoerd
  
Wanneer u WSUS 3.0 SP1 verwijdert, wordt u de mogelijkheid geboden om de logboekbestanden van de installatie te behouden. Wanneer u WSUS 3.0 SP1 vervolgens opnieuw installeert, verliezen de oude logboekbestanden hun machtigingen (deze bestanden zijn gewoonlijk alleen toegankelijk voor WSUS-administrators). U moet vervolgens de machtigingen voor deze logboekbestanden herstellen.
  
#### Als WSUS 2.0-clients over updates met de status Niet van toepassing beschikken, worden deze gedurende een korte periode na de upgrade naar WSUS 3.0 SP1 aangeduid als Onbekend
  
Als een WSUS 2.0-server over clients met updates met de status **Niet van toepassing** beschikt, worden deze updates gedurende een korte periode nadat er een upgrade naar WSUS 3.0 SP1 heeft plaatsgehad, weergegeven met de status **Onbekend**. De eerstvolgende keer dat er door de client een scanbewerking wordt uitgevoerd, wordt de status opnieuw ingesteld op **Niet van toepassing**.
  
Bekende problemen  
-----------------
  
#### Probleemoplossingen bij meerdere downloadfouten of het herhaaldelijk mislukken van clientsynchronisatiebewerkingen
  
Er is mogelijk sprake van een beschadigde downloadcache van de client als WSUS 3.0 SP1-clients meerdere downloadfouten rapporteren of als het synchroniseren van clients met de WSUS 3.0 SP1-server gedurende een langere periode mislukt. U kunt proberen om dit probleem te verhelpen door de downloadcache van de client uit het bestandssysteem te verwijderen.
  
De downloadcache van de client verwijderen:
  
1.  Verwijder alle bestanden en submappen op de volgende locatie op de clientcomputer: **%windir%\\SoftwareDistributie\\Download**  
2.  Probeer om de update te installeren door de clientcomputer opnieuw met WSUS 3.0 SP1 te synchroniseren. Deze installatiepoging moet vervolgens mislukken met de fout: **WU\_E\_DM\_NOTDOWNLOADED, "De update is niet gedownload."**  
3.  Nadat deze fout wordt weergegeven, zal de clientcomputer het downloaden automatisch opnieuw starten, zodat de installatie kan worden voortgezet.
  
#### Probeer opnieuw of u de synchronisatiebewerking kunt uitvoeren als de synchronisatiebewerking mislukt
  
Als het synchroniseren mislukt, moet u eerst opnieuw proberen of u de server kunt synchroniseren. Als de daaropvolgende synchronisatiepogingen eveneens mislukken, kunt u de informatie in de [Handleiding voor de bewerkingen van Windows Server Update Services 3.0](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072) gebruiken om het probleem op te lossen.
  
#### Het rechtstreeks in de database wijzigen van de WSUS 3.0 SP1-configuratie wordt niet ondersteund
  
De configuratiegegevens van Windows Server Update Services worden opgeslagen in een SQL Server-database. Het rechtstreeks in de database wijzigen van de configuratiegegevens wordt echter niet ondersteund. Onderneem geen pogingen om de configuratiegegevens van WSUS 3.0 SP1 rechtstreeks in de database te wijzigen. U moet de configuratiegegevens van WSUS 3.0 SP1 wijzigen via de WSUS 3.0 SP1-console of via aangeroepen WSUS 3.0 SP1 API’s.
  
#### Mislukte downloads worden niet tijdig gerapporteerd wanneer u gebruikmaakt van schijfquota’s
  
Wanneer de quotalimiet is bereikt in gevallen waarin u gebruikmaakt van schijfquota’s, worden mislukte updatedownloads op de WSUS-server mogelijk niet tijdig gerapporteerd. U kunt dit probleem vermijden door geen gebruik te maken van quota’s of door de quota’s te verhogen.
  
#### Als WSUS 3.0 SP1 wordt geïmplementeerd via SSL, is het mogelijk dat de implementatie op de clientcomputers mislukt met de foutcode 0x8024400a
  
Het implementeren van de software op clientcomputers kan in sommige gevallen mislukken met de foutcode 0x8024400a wanneer deze communiceren met een WSUS 3.0 SP1-server die gebruikmaakt van SSL. Zie het artikel [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593) voor bijgewerkte informatie over dit probleem.
  
#### De domeinaccount voor de groep WSUS-administrators wordt niet verwijderd wanneer WSUS wordt verwijderd
  
De groep WSUS-administrators wordt op domeincontrollers gemaakt als een domeinaccount (geen lokale account). Dit heeft tot gevolg dat alle installaties die gebruikmaken van deze domeinaccount, zouden worden uitgeschakeld als de account wordt verwijderd wanneer WSUS wordt verwijderd. Daarom wordt de domeinaccount van de groep WSUS-administrators niet verwijderd wanneer WSUS wordt verwijderd.
  
#### Als een downstream-server wordt geconverteerd naar een upstream-server, moeten catalogussite-updates opnieuw worden geïmporteerd
  
Wanneer u een downstream-server converteert naar een upstream-server, moet u tevens alle catalogussite-updates opnieuw importeren. Als u dat nalaat, zullen nieuwe versies van catalogussite-updates niet met deze server worden gesynchroniseerd.
  
#### Als u gebruikmaakt van IIS met SSL, is ongecodeerde toegang nog steeds mogelijk, tenzij u de optie Beveiligd kanaal (SSL) vereisen inschakelt
  
Als u IIS zo hebt ingesteld dat er via het installeren van een certificaat gebruik moet worden gemaakt van SSL, is het nog steeds mogelijk om de site te openen via ongecodeerde http-toegang, tenzij u de optie **Beveiligd kanaal (SSL) vereisen** inschakelt. Zie de documentatie voor [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084) voor meer informatie.
  
#### Het importeren van catalogussites kan mislukken als er geen lees- en schrijfmachtiging voor de map %windir%\\TEMP is ingesteld
  
Als tijdens het importeren blijkt dat de Network Service-account niet is voorzien van een lees- en schrijfmachtiging voor de map %windir%\\TEMP, kan het importeren mislukken met het volgende bericht: Server kan de aanvraag niet uitvoeren. ---&gt; Kan het bestand C:\\WINDOWS\\TEMP\\*tempbestandsnaam*.dll niet vinden.
  
#### De synchronisatie verloopt mogelijk langzaam wanneer u synchroniseert tussen WSUS 3.0 SP1 en een stroomafwaartse replicaserver waarop WSUS 2.0 wordt uitgevoerd
  
Als u WSUS 3.0 SP1 installeert op een stroomopwaartse server en als u vervolgens probeert om te synchroniseren met een stroomafwaartse replicaserver waarop WSUS 2.0 wordt uitgevoerd, kunnen er prestatieproblemen optreden. Zie het artikel [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669) voor informatie over het oplossen van dit probleem.
  
#### Als de e-mailserver tijdelijk onbereikbaar of uitgeschakeld is, mislukt het verzenden van kennisgevingen per e-mail, zonder dat er een melding wordt weergegeven
  
Als de e-mailserver van het netwerk offline is, zal het verzenden van kennisgevingen per e-mail mislukken zonder dat er een melding wordt weergegeven. In een dergelijk geval wordt echter wel de gebeurtenis 10052 (HealthCoreEmailNotificationRed) in het gebeurtenislogboek vastgelegd.
  
#### Gewijzigde instellingen op een upstream-server worden niet onmiddellijk aan de downstream-server doorgegeven
  
Wanneer de configuratie van de stroomopwaartse server wordt gewijzigd, kan het even duren voordat deze configuratiewijzigingen daadwerkelijk van kracht worden. Als u een instelling op de upstream-server wijzigt (u selecteert bijvoorbeeld een nieuwe taal) en als u vervolgens op de downstream-server een synchronisatie in werking stelt, wordt de desbetreffende wijziging niet weergegeven. De wijziging zal pas bij de volgende geplande synchronisatie aan de downstream-server worden doorgegeven. De wachttijd neemt toe naarmate het aantal aanwezige updates op de stroomopwaartse server groter is.
  
#### Wanneer u WSUS 3.0 SP1 verwijdert, wordt het database-exemplaar niet verwijderd
  
Als WSUS 3.0 SP1 wordt verwijderd, wordt het database-exemplaar niet verwijderd. Dit exemplaar wordt mogelijk gedeeld met een of meer andere toepassingen, die zouden mislukken wanneer het database-exemplaar wordt verwijderd.
  
Als het noodzakelijk is dat Windows Internal Database wordt verwijderd, kunt u daartoe de volgende opdrachten gebruiken:
  
(op 32-bitsplatforms)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(op 64-bitsplatforms)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Als u Windows Internal Database Service Pack 2 uit Windows Server 2008 wilt verwijderen, kunt u daartoe gebruikmaken van serverbeheer.
  
Het is echter mogelijk dat de standaard MDF- en LDF-bestanden niet worden verwijderd, waardoor een volgende WSUS 3.0 SP1-installatie zal mislukken. Deze bestanden kunnen worden verwijderd uit de map %windir%\\SYSMSI\\SSEE.
  
#### Als de upstream-server van de downstream-server wordt gewijzigd, worden updates met de status Onbekend gerapporteerd als Niet van toepassing
  
Als een stroomafwaartse server een synchronisatiebewerking vanaf een andere stroomopwaartse server start, worden updates met de status **Onbekend** op de nieuwe stroomopwaartse server gerapporteerd als **Niet van toepassing**. Deze status is tijdelijk. De status zal, nadat de clients met de downstream-server zijn gesynchroniseerd, de eerstvolgende keer dat de downstream-serverstatus wordt gerapporteerd, worden bijgewerkt.
  
#### De verbinding met alle servers gaat verloren als tijdens het uitvoeren van de wizard Server opschonen op een van de servers een time-out optreedt wanneer deze wizard via een externe console op meerdere servers tegelijk wordt uitgevoerd
  
De wizard Server opschonen kan vanuit één externe console op meerdere servers tegelijk worden uitgevoerd. Als er tijdens het opschonen op een van de servers een time-out optreedt, gaat de verbinding tussen de console en alle servers verloren. Er gaan geen gegevens verloren, maar de beheerder moet wel de externe verbinding van de afzonderlijke servers opnieuw instellen.
  
#### Het snel achtereenvolgens tot stand brengen en verbreken van de verbinding heeft tot gevolg dat in de configuratiewizard het foutbericht Er is geen synchronisatiefout opgetreden wordt weergegeven
  
Wanneer u WSUS configureert, moet u een verbinding met de stroomopwaartse server (Microsoft Update of de stroomopwaartse server op het intranet) tot stand brengen, zodat er basisinformatie over de server kan worden overgebracht. Als u op **Verbinding maken** en onmiddellijk op **Verbinding verbreken** klikt, wordt het onterechte foutbericht Er is geen synchronisatiefout opgetreden weergegeven.
  
WSUS 3.0 SP1 onder Windows Server 2008  
--------------------------------------
  
#### Ondersteunde versies
  
WSUS 3.0 SP1 ondersteunt zowel de 32-bits als de 64 bits versie van Windows Server 2008.
  
#### Vereisten
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Vereiste</th>
<th style="border:1px solid black;" >Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">Installeer deze software via het besturingssysteem. Zorg ervoor dat de volgende onderdelen zijn ingeschakeld
<ul>
<li>Windows-verificatie<br />
<br />
</li>
<li>Statische inhoud<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>Compatibiliteit met 6.0-beheer<br />
<br />
</li>
<li>Compatibiliteit met IIS 6.0-metabase<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Version 2.0 Redistributable Package (x86)</td>
<td style="border:1px solid black;">Dit hoeft onder Windows Server 2008 niet te worden geïnstalleerd, omdat deze software al is geïnstalleerd als onderdeel van het besturingssysteem.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">Dit hoeft onder Windows Server 2008 niet te worden geïnstalleerd, omdat deze software al is geïnstalleerd als onderdeel van het besturingssysteem.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dit is een vereiste voor het gebruik van de WSUS-gebruikersinterface. Zie de informatie over Microsoft Report Viewer Redistributable 2005 op de <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Downloadcentrum</a>-website (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### De wizard Beveiliging configureren gebruiken
  
Wanneer u onder Windows Server 2008 de wizard Beveiliging configureren uitvoert, kunt u de WSUS-rol en de bijbehorende afhankelijkheden inschakelen. Als u de wizard Beveiliging configureren wilt uitvoeren, klik u op **Start**, wijst u **Systeembeheer** aan en klikt u vervolgens op **wizard Beveiliging configureren**.
  
De volgende bekende problemen treden op in gevallen waarin de wizard Beveiliging configureren wordt gebruikt met de WSUS-rol:
  
-   **De interne database van Windows wordt ingeschakeld ook al wordt deze door WSUS mogelijk niet gebruikt.** U configureert WSUS voor het gebruik van een database (de interne database van Windows of een SQL Server-database). Als u in de wizard Beveiliging configureren de WSUS-rol inschakelt, terwijl WSUS is geïnstalleerd met SQL Server, wordt de service voor de interne database van Windows ingeschakeld, indien deze op de computer is geïnstalleerd. Deze wordt door WSUS echter niet gebruikt. Wanneer u een SQL Server-database gebruikt in plaats van de interne database van Windows, moet u de service voor de interne database van Windows uitschakelen.  
-   **Firewallregels voor WSUS worden op een aangepaste website standaard niet ingeschakeld.** Als u WSUS op een aangepaste website (poort 8530 of 8531) installeert, worden de vereiste firewallregels niet automatisch ingeschakeld. Dit geldt ook wanneer u in de wizard Beveiliging configureren de WSUS-functie hebt geselecteerd. U moet de toepasselijke firewallregels voor WSUS inschakelen, afhankelijk van de vraag of SSL (Secure Sockets Layer) wel of niet voor de WSUS-server is geconfigureerd.
  
WSUS 3.0 SP1 onder Windows Small Business Server 2003  
-----------------------------------------------------
  
#### Als de virtuele hoofdmap van IIS beperkt is tot bepaalde IP-adressen en domeinnamen, kan de WSUS 3.0 SP1-server niet worden bijgewerkt
  
Bij sommige installaties van Windows Small Business Server is de standaard IIS-website ingesteld op **IP-adres en domeinnaambeperkingen**. Als dat het geval is, kan de Windows Update-client op de server mogelijk niet worden bijgewerkt.
  
#### WSUS 3.0 SP1 installeren onder Small Business Server—Integratieproblemen
  
-   Als Windows Small Business Server 2003 voor internettoegang gebruikmaakt van een ISA-proxyserver, moeten het volgende in de gebruikersinterface van **Instellingen** worden ingevoerd: **proxyserverinstellingen, proxyservernaam, poort**.  
-   Als ISA gebruikmaakt van Windows-verificatie, moeten er referenties voor de proxyserver worden ingevoerd. Gebruik hiertoe de notatie *DOMEIN*\\*gebruiker*. Daarnaast moet de gebruiker lid zijn van de groep Internetgebruikers.
  
#### Als u een subnet aan uw netwerk hebt toegevoegd zonder dat u daartoe gebruik hebt gemaakt van de wizards van Windows Small Business Server, moet u de volgende procedure uitvoeren
  
Tijdens het installatieproces van WSUS-server worden twee virtuele IIS-hoofdmappen op de server geïnstalleerd: SelfUpdate en ClientWebService. Ook worden sommige bestanden onder de basismap van de standaardwebsite (op poort 80) geplaatst, zodat clientcomputers automatisch via de standaardwebsite kunnen worden bijgewerkt. De standaardwebsite is standaard zo geconfigureerd dat de toegang tot andere IP-adressen dan die van de lokale host of tot specifieke subnetten die aan de server zijn gekoppeld, wordt geweigerd. Dit heeft tot gevolg dat clientcomputers niet kunnen worden bijgewerkt wanneer deze niet op de lokale host of op de desbetreffende specifieke subnetten zijn ingesteld. Als u een subnet aan uw netwerk hebt toegevoegd zonder dat u daartoe gebruik hebt gemaakt van de wizards van Microsoft Windows Small Business Server 2003, moet u de volgende procedure uitvoeren:
  
1.  Vouw in Serverbeheer **Geavanceerd beheer** uit, vouw **Internet Information Services** uit, vouw **Websites** uit, vouw **Standaardwebsite** uit, klik met de rechtermuisknop op de virtuele map **Zelfupdate** en klik vervolgens op **Eigenschappen**.  
2.  Klik op **Mapbeveiliging**.  
3.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik vervolgens op **Toegang verleend**.  
4.  Klik op **OK**, klik met de rechtermuisknop op de virtuele map **ClientWebService** en klik vervolgens op **Eigenschappen**.  
5.  Klik op **Mapbeveiliging**.  
6.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik vervolgens op **Toegang verleend**.
  
Copyright  
---------
  
De informatie in dit document, met inbegrip van URL's en andere verwijzingen naar internetwebsites, kan zonder voorafgaande kennisgeving worden gewijzigd. Tenzij anderszins vermeld, zijn alle in dit document vermelde bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen fictief. Eventuele overeenkomsten met bestaande bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen of gebeurtenissen berusten geheel op toeval. U bent er zelf voor verantwoordelijk om aan alle van toepassing zijnde copyrightwetten te voldoen. Behoudens de in of krachtens de geldende wetgeving op het gebied van auteursrechten gestelde uitzonderingen, mag niets uit deze uitgave worden verveelvoudigd en/of openbaar worden gemaakt door middel van druk, fotokopie, microfilm, of op welke andere wijze dan ook en evenmin in een gegevensopzoeksysteem worden opgeslagen zonder de voorafgaande uitdrukkelijke schriftelijke toestemming van Microsoft Corporation.
  
Microsoft is mogelijk in het bezit van octrooien, aanvragen voor octrooien, merken, auteursrechten of andere intellectuele eigendomsrechten met betrekking tot materiaal in dit document. Tenzij uitdrukkelijk vermeld in een schriftelijke gebruiksrechtovereenkomst van Microsoft, kunt u geen gebruiksrecht op deze octrooien, merken, auteursrechten of andere rechten op intellectueel eigendom ontlenen aan dit document.
  
©2007 Microsoft Corporation. Alle rechten voorbehouden
  
Microsoft, SQL Server, Windows en Windows Server zijn merken of gedeponeerde handelsmerken van Microsoft Corporation in de Verenigde Staten en/of andere landen.
  
Alle andere handelsmerken zijn eigendom van hun respectieve eigenaren.
