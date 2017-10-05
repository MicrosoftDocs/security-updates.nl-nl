---
TOCTitle: 'Opmerkingen over de release van Microsoft Windows Server Update Services 3.0'
Title: 'Opmerkingen over de release van Microsoft Windows Server Update Services 3.0'
ms:assetid: '94d1385f-4872-4c29-8822-3a4ec5e45ae4'
ms:contentKeyID: 18126876
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708491(v=WS.10)'
---

Opmerkingen over de release van Microsoft Windows Server Update Services 3.0
============================================================================

In deze releaseopmerkingen worden de bekende kwesties beschreven die kunnen optreden in Microsoft® Windows® Server Update Services 3.0 (WSUS 3.0). Verder bevat dit bestand aanbevelingen en vereisten voor de installatie van het programma. Deze opmerkingen bestaan uit de volgende gedeelten:

-   Systeemvereisten voor het installeren van WSUS 3.0 op een server
-   Configuratievereisten voor het installeren van WSUS 3.0 op een server
-   Systeemvereisten voor het installeren van WSUS 3.0 op een externe console
-   Configuratievereisten voor externe consoles met WSUS 3.0
-   Systeemvereisten voor het installeren van een client
-   Softwarevereisten voor het installeren van WSUS 3.0 op een server
-   Minimale schijfruimte voor het installeren van WSUS 3.0 op een server
-   Upgradevereisten voor WSUS 3.0
-   Opdrachtregelparameters voor de installatie
-   Installatie- en upgradeproblemen
-   Bekende problemen
-   WSUS 3.0 op Windows Server® 2008
-   WSUS 3.0 onder Windows Small Business Server 2003

| ![](images/Cc708491.note(WS.10).gif)Opmerking                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U kunt een exemplaar van dit document downloaden via het [Downloadcentrum van Microsoft](http://go.microsoft.com/fwlink/?linkid=71220) ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)). |

Belangrijke opmerking over de configuratie: U moet het wachtwoord van de proxyserver in de configuratiewizard overschrijven
---------------------------------------------------------------------------------------------------------------------------

Indien u een proxyserver gebruikt waarvoor verificatie met behulp van een gebruikersnaam/wachtwoord is vereist, worden er mogelijk geen updates gesynchroniseerd door de WSUS-server als u het wachtwoord van de proxyserver niet overschrijft terwijl u de configuratiewizard voor WSUS-servers uitvoert. Omdat de configuratiewizard automatisch wordt gestart aan het einde van de installatie, kan dit probleem synchronisatiefouten veroorzaken nadat u een upgrade naar WSUS 3.0 hebt uitgevoerd vanaf een oudere versie van WSUS.

U kunt dit probleem voorkomen door de configuratiewizard te annuleren na de upgrade of door het juiste proxywachtwoord opnieuw in te voeren wanneer de wizard wordt uitgevoerd. Als u dit probleem wilt herstellen wanneer het optreedt, gaat u naar **Bron- en proxyserver bijwerken** op de pagina **Opties**, voert u het proxywachtwoord opnieuw in en slaat u de instelling op.

Systeemvereisten voor het installeren van WSUS 3.0 op een server
----------------------------------------------------------------

#### WSUS 3.0-server wordt ondersteund onder Windows Server 2003 Service Pack 1 en Windows Server 2008

De WSUS 3.0-server wordt ondersteund onder Windows Server 2003 Service Pack 1 en Windows Server 2008.

#### Windows 2000 Server wordt niet ondersteund voor WSUS 3.0-servers

Microsoft Windows® 2000 Server is geen ondersteund besturingssysteem voor WSUS 3.0-servers.

#### WSUS 3.0 wordt niet ondersteund door servers waarop Terminal Services wordt uitgevoerd

Hoewel WSUS 3.0 mogelijk werkt op servers waarop Terminal Services wordt uitgevoerd, wordt dit niet ondersteund of aanbevolen. WSUS 3.0 werkt niet op een server waarop Terminal Services wordt uitgevoerd in configuraties met externe SQL Server-implementaties. Aangezien alle externe aangepaste acties (waaronder installatie) op een Terminal Server-licentieserver worden uitgevoerd als de systeemaccount en de systeemaccount van de server mogelijk geen machtigingen heeft op de externe SQL Server, kan de installatie mislukken.

Configuratievereisten voor het installeren van WSUS 3.0 op een server
---------------------------------------------------------------------

#### IIS moet zijn geïnstalleerd

Voor Microsoft Windows Server Update Services 3.0 is Internet Information Services (IIS) nodig. IIS wordt niet standaard geïnstalleerd in Microsoft Windows Server 2003 of Windows Server 2008. Als u WSUS 3.0 zonder IIS installeert, wordt er een foutbericht weergegeven met de mededeling dat IIS niet is geïnstalleerd.

#### Als IIS in de IIS 5.0-isolatiemodus wordt uitgevoerd, mislukt de installatie

Als u de server van Windows 2000 Server hebt bijgewerkt naar Windows Server 2003, wordt IIS mogelijk in IIS 5.0-compatibiliteitsmodus uitgevoerd. Het is ook mogelijk dat de IIS 5.0-isolatiemodus is ingeschakeld in IIS Manager. Hierdoor mislukt de installatie. U moet de IIS 5.0-isolatiemodus uitschakelen voordat u WSUS 3.0 installeert.

#### Als een onderdeel van IIS is geïnstalleerd in de 32-bits compatibiliteitsmodus op een 64-bits platform, kan de installatie van WSUS 3.0 mislukken

Alle onderdelen van IIS moeten worden geïnstalleerd in de native modus op 64-bits platforms. De installatie kan mislukken als een onderdeel van IIS in de 32-bits compatibiliteitsmodus is geïnstalleerd.

#### HTTP en HTTPS moeten beide door proxyservers worden ondersteund

Wanneer u de hoofdserver voor WSUS configureert (de WSUS-server die de updates rechtstreeks vanuit Microsoft Update ophaalt) en er bevindt zich een proxyserver tussen de WSUS-server en internet, moet die proxyserver HTTP en HTTPS ondersteunen.

#### Als er al twee of meer websites worden uitgevoerd op poort 80, verwijdert u deze allemaal op één na voordat u WSUS installeert

Als er al twee of meer websites worden uitgevoerd op poort 80 (bijvoorbeeld Windows® SharePoint® Services), moet u deze allemaal op één na verwijderen voordat u WSUS installeert Als u dit niet doet, kunnen de clients van uw server mogelijk niet automatisch worden bijgewerkt.

#### Wanneer u WSUS 3.0 installeert, moet u mogelijk uw antivirusprogramma's uitschakelen

Wanneer u WSUS 3.0 wilt installeren, moet u mogelijk uw antivirusprogramma's uitschakelen voordat u de installatie kunt uitvoeren. Nadat u het antivirusprogramma hebt uitgeschakeld, moet u de computer opnieuw opstarten voordat u WSUS installeert. Hiermee voorkomt u dat bestanden worden vergrendeld wanneer de installatieprocedure toegang zoekt tot de bestanden. Vergeet niet om na het voltooien van de installatie het antivirusprogramma weer in te schakelen. Bezoek de website van de leverancier van het antivirusprogramma voor de exacte procedure voor het in- en uitschakelen van het antivirusprogramma en voor de versiegegevens.

| ![](images/Cc708491.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Door deze methode kan uw computer of netwerk kwetsbaarder worden voor aanvallen door kwaadwillende gebruikers of schadelijke software, zoals virussen. Microsoft raadt deze methode niet aan, maar verschaft u deze informatie zodat u zelf kunt beslissen of u de methode al dan niet wilt uitvoeren. Het gebruik van deze methode is voor uw eigen risico. |

| ![](images/Cc708491.note(WS.10).gif)Opmerking                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Een antivirusprogramma is ontworpen om uw computer beter te beveiligen tegen virussen. Download of open geen bestanden van bronnen die u niet vertrouwt, bezoek geen websites die u niet vertrouwt en open geen e-mailbijlagen wanneer uw antivirusprogramma is uitgeschakeld. |

#### WSUS 3.0 vereist dat de optie voor geneste triggers in SQL Server is ingeschakeld

Deze optie is standaard ingeschakeld, maar kan worden uitgeschakeld door een SQL Server-beheerder.

Als u van plan bent een SQL Server-database als gegevensarchief voor Windows Server Update Services te gebruiken, moet de SQL Server-beheerder controleren of de optie voor geneste triggers is ingeschakeld voordat de WSUS 3.0-beheerder WSUS 3.0 installeert en de database opgeeft tijdens de installatie.

WSUS 3.0 Setup schakelt de optie RECURSIVE\_TRIGGERS in, hetgeen een database-specifieke optie is. De optie voor geneste triggers wordt echter niet ingeschakeld, omdat dit een algemene optie is die geldt voor de hele server.

Als u wilt controleren of de optie voor geneste triggers is ingeschakeld, gebruikt u de volgende opdracht:

**sp\_configure 'nested triggers'**

Als u de optie voor geneste triggers in SQL Server wilt inschakelen, voert u de volgende opdracht uit vanuit een batchbestand op de computer waarop SQL Server wordt uitgevoerd:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Als SQL Server Management Studio niet op uw server is geïnstalleerd, kunt u ook SQL-scripts uitvoeren vanaf de opdrachtregel. U kunt het opdrachtregelhulpprogramma voor Microsoft SQL Server 2005 ophalen van het [Downloadcentrum van Microsoft](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). Begin met de opdracht **sqlcmd**.

Als u SQL-scripts op Windows Internal Database wilt uitvoeren, moet u ook de SQL Native Client van dezelfde downloadpagina downloaden.

#### Beperkingen en vereisten voor extern SQL

WSUS 3.0 biedt ondersteuning voor het uitvoeren van databasesoftware op een computer die gescheiden is van de computer met de rest van de WSUS 3.0-toepassing. Er bestaan enige vereisten voor het configureren van een externe SQL-installatie

-   U kunt geen server gebruiken die als een domeincontroller is geconfigureerd voor de back-endcomputer van een SQL-paar.
-   U moet niet Terminal Server uitvoeren op de computer die u wilt gebruiken als de front-endserver van een externe SQL-installatie.
-   U moet ten minste Microsoft SQL Server 2005 Service Pack 1 (beschikbaar in het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143) voor databasesoftware op de back-endcomputer als op deze computer Windows Server 2003 wordt uitgevoerd en SQL Server 2005 Service Pack 2 als er Windows Server® 2008 wordt uitgevoerd.
-   Zowel de front-end- als de back-endcomputer moet worden verbonden met een Active Directory-domein. Als de computers zich in verschillende domeinen bevinden, moet u een vertrouwensrelatie tussen verschillende domeinen instellen voordat u WSUS installeert.
-   Als WSUS 2.0 al is geïnstalleerd in een configuratie met externe SQL en u een upgrade naar WSUS 3.0 wilt uitvoeren, moet u WSUS 2.0 van de back-endcomputer verwijderen (met behulp van het onderdeel **Software** in het Configuratiescherm). Daarbij moet u ervoor zorgen dat de bestaande database intact blijft. Vervolgens moet u SQL Server 2005 SP1 of SP2 installeren en de bestaande database bijwerken. Ten slotte moet u WSUS 3.0 installeren op de front-endcomputer.

#### WSUS kan niet worden geïnstalleerd als er al bepaalde vooruitgaven van Internet Explorer 7 en Terminal Services zijn geïnstalleerd.

De installatie van WSUS mislukt als er bepaalde voorlopige versies van Internet Explorer 7 en Terminal Services aanwezig zijn.

Systeemvereisten voor het installeren van WSUS 3.0 op een externe console
-------------------------------------------------------------------------

De externe console voor WSUS 3.0 kan op de volgende platformen worden geïnstalleerd:

-   Windows Server 2008
-   Windows Vista®
-   Windows Server 2003 SP1
-   Windows XP SP2

Configuratievereisten voor externe consoles met WSUS 3.0
--------------------------------------------------------

#### U moet over een breedbandverbinding tussen een externe beheerconsole en een WSUS 3.0-server beschikken

Er kunnen prestatieproblemen optreden als u de WSUS 3.0-server via een langzame WAN-verbinding verbindt met een externe beheerconsole. U kunt het aantal updates en computers dat wordt weergegeven, beperken door update- en computerweergaven te filteren, maar het wordt aanbevolen om een breedbandverbinding tussen de console en WSUS 3.0-servers te gebruiken. Als er prestatieproblemen optreden met de externe console, raden wij u aan om de server via Terminal Server te verbinden voor extern beheer.

Systeemvereisten voor het installeren van een client
----------------------------------------------------

De WSUS-clientsoftware wordt automatisch bijgewerkt. De software kan met WSUS op al de volgende besturingssystemen worden gebruikt:

-   Windows Vista
-   Windows Server 2008
-   Elke versie van Microsoft Windows Server 2003
-   Microsoft Windows XP Professional SP2
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 of Windows 2000 Advanced Server met SP4.

Softwarevereisten voor het installeren van WSUS 3.0 op een server
-----------------------------------------------------------------

In de volgende tabel wordt de vereiste software voor Windows Server 2003 SP1-platformen weergegeven. De vereiste software voor Windows Server 2008 wordt besproken in het gedeelde over WSUS 3.0 op Windows Server 2008.

Zorg dat de WSUS 3.0-server voldoet aan de vereisten in deze lijst voordat u WSUS 3.0 installeert. Als een van deze updates vereist dat de computer opnieuw wordt opgestart wanneer de installatie is voltooid, moet u de server opnieuw starten voordat u WSUS 3.0 installeert.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Vereiste</th>
<th>Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">IIS (Microsoft Internet Information Services)</td>
<td style="border:1px solid black;">Moet worden geïnstalleerd vanuit het besturingssysteem.
Zie Kwestie 1: IIS moet zijn geïnstalleerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herdistribueerbaar pakket (x86) voor Microsoft .NET Framework versie 2.0</td>
<td style="border:1px solid black;">Raadpleeg het artikel met informatie over het herdistribueerbare pakket (x86) voor Microsoft .NET Framework versie 2.0 in het <a href="http://go.microsoft.com/fwlink/?linkid=68935">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=68935). Raadpleeg voor 64-bits platforms het artikel over het herdistribueerbare pakket (x64) voor Microsoft .NET Framework versie 2.0 in het (<a href="http://go.microsoft.com/fwlink/?linkid=70637">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70637)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0 voor Windows Server 2003</td>
<td style="border:1px solid black;">Dit is een vereiste om de gebruikersinterface van WSUS 3.0 te kunnen gebruiken. Raadpleeg het artikel met informatie over Microsoft Management Console 3.0 voor Windows Server 2003 (KB907265) in het <a href="http://go.microsoft.com/fwlink/?linkid=70412">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70412). Raadpleeg voor 64-bits platforms het artikel over Microsoft Management Console 3.0 voor Windows Server 2003 x64 (KB907265) in het <a href="http://go.microsoft.com/fwlink/?linkid=70638">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70638).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dit is een vereiste om de gebruikersinterface van WSUS 3.0 te kunnen gebruiken. Raadpleeg het artikel met informatie over het herdistribueerbare pakket voor Microsoft Report Viewer 2005 in het <a href="http://go.microsoft.com/fwlink/?linkid=70410">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (optioneel)</td>
<td style="border:1px solid black;">WSUS 3.0 installeert Windows Internal Database voor u als er nog geen compatibele versie van SQL Server is geïnstalleerd. Als u een volledige SQL Server-database wilt installeren, moet u (ten minste) SQL Server 2005 SP1 gebruiken (beschikbaar in het <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Downloadcentrum</a> (http://go.microsoft.com/fwlink/?LinkId=66143) onder Windows Server 2003 of SQL Server 2005 SP2 (beschikbaar in het <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Downloadcentrum</a> op http://go.microsoft.com/fwlink/?LinkId=84823) voor op Windows Server 2008.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708491.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                        |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als WSUS 2.0 al is geïnstalleerd en SQL Server 2000, SQL Server Desktop Engine 2000 of een andere SQL Server-database ouder dan SQL Server 2005 SP1 (or SQL Server 2005 SP2 op Windows Server 2008) gebruikt, wordt Windows® Internal Database geïnstalleerd door het installatieprogramma van WSUS 3.0 en wordt de database hiernaar gemigreerd. |
  
Minimale schijfruimte voor het installeren van WSUS 3.0 op een server  
---------------------------------------------------------------------
  
Hier volgen de minimale eisen die worden gesteld aan de schijfruimte voor het installeren van Windows Server Update Services:
  
-   1 GB op de systeempartitie  
-   2 GB voor het volume waarop de databasebestanden worden opgeslagen  
-   20 GB voor het volume waarop de inhoud wordt opgeslagen
  
| ![](images/Cc708491.Important(WS.10).gif)Belangrijk                                                             |  
|----------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0 kan niet op gecomprimeerde stations worden geïnstalleerd. Controleer of het station dat u hebt geselecteerd, niet is gecomprimeerd. |
  
Upgradevereisten voor WSUS 3.0  
------------------------------
  
#### Controleer of de WSUS-installatie op de juiste wijze wordt uitgevoerd en maak een back-up van de WSUS-database voordat u de upgrade uitvoert.
  
Als u een upgrade naar WSUS 3.0 vanaf een vorige versie uitvoert, controleert u of de huidige installatie op de juiste wijze wordt uitgevoerd en maakt u een back-up van de WSUS-database voordat u de upgrade uitvoert.
  
1.  Controleer de logboeken op recente fouten, synchronisatieproblemen tussen downstream-servers en upstream-servers of problemen met clients waarvan geen rapporten worden ontvangen. Zorg dat dergelijke problemen worden opgelost voordat u verdergaat.  
2.  Mogelijk wilt u DBCC CHECKDB uitvoeren om te controleren of de WSUS-database op de juiste wijze is geïndexeerd. Zie [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) voor meer informatie over CHECKDB (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Maak een back-up van de WSUS-database.
  
#### Software Update Services 1.0 moet worden verwijderd
  
De installatie van WSUS 3.0 kan niet worden uitgevoerd als Software Update Services 1.0 op dezelfde machine is geïnstalleerd. U moet Software Update Services 1.0 verwijderen voordat u WSUS 3.0 installeert.
  
#### Een bètaversie van WSUS 3.0 kan niet worden bijgewerkt naar de RTM-versie van WSUS 3.0, maar de RC-versie kan wel naar de RTM-versie worden bijgewerkt
  
Als op uw computer al een bètaversie van WSUS 3.0 is geïnstalleerd, moet u deze verwijderen en de database verwijderen voordat u de RTM-versie van WSUS 3.0 installeert. Alleen de RC-versie kan naar de RTM-versie worden bijgewerkt.
  
#### Er kan geen upgrade van WSUS 2.0 naar WSUS 3.0 worden uitgevoerd in een 64-bits besturingssysteem
  
WSUS 2.0 wordt niet ondersteund in 64-bits besturingssystemen. In 64-bits besturingssystemen kan dus geen upgrade van WSUS 2.0 naar WSUS 3.0 worden uitgevoerd.
  
Opdrachtregelparameters voor de installatie  
-------------------------------------------
  
Met behulp van de opdrachtregelparameters voor WSUS kunt u een installatie zonder toezicht van WSUS 3.0 uitvoeren. In de volgende tabel vindt u de opdrachtregelparameters voor WSUS 3.0.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Optie</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Een installatie op de achtergrond uitvoeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Het product verwijderen. Het exemplaar van Windows Internal Database wordt ook verwijderd als dit is geïnstalleerd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Alleen vereisten controleren. Het product wordt niet geïnstalleerd, maar het systeem wordt gecontroleerd en er wordt gerapporteerd of er vereisten ontbreken.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Opdrachtregelparameters en de bijbehorende beschrijvingen weergeven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Upgrade uitvoeren vanaf versie 2.0 van WSUS. De enige geldige parameter bij deze optie is /q (installatie op de achtergrond). De enige geldige eigenschap bij deze optie is DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
In de volgende tabel vindt u de opdrachtregeleigenschappen voor WSUS 3.0.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Eigenschap</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=inhoud lokaal gehost, 1=hosten op Microsoft Update</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Pad naar map met inhoud. Het standaardpad is <em>WSUSInstallatiestation</em><strong>\WSUS\WSUSContent</strong>, waarbij <em>WSUSInstallatiestation</em> het lokale station met de meeste beschikbare schijfruimte is.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Pad naar map met gegevens van Windows Internal Database.</td>
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
<td style="border:1px solid black;">0=WSUS-server installeren, 1=alleen console installeren</td>
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
<td style="border:1px solid black;">0=logboekbestanden behouden, 1=logboekbestanden verwijderen (wordt gebruikt in combinatie met de schakeloptie /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=huidige database gebruiken, 1=database maken</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Vensteringang voor het retourneren van MSI-voortgangsberichten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=deelnemen aan het programma voor verbetering van de gebruikerservaring van Microsoft Update, 0=niet deelnemen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=de locatie van de inhoud niet naar de database wegschrijven, 0=de locatie van de inhoud naar de database wegschrijven (voor NLB)</td>
</tr>
</tbody>
</table>
  
#### Voorbeeld van gebruik
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708491.Important(WS.10).gif)Belangrijk                                                                                                                                                                      |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u WSUS 3.0 installeert in de stille modus (/q) en niet alle vereiste onderdelen op de computer zijn geïnstalleerd, genereert het installatieprogramma een bestand met de naam WSUSPreReqCheck.xml. Dit bestand wordt opgeslagen in de map %TEMP%. |
  
Installatieproblemen  
--------------------
  
#### IIS wordt opnieuw gestart tijdens WSUS 3.0 Setup
  
WSUS 3.0 Setup start IIS opnieuw zonder melding. Dit kan invloed hebben op bestaande websites binnen uw organisatie. Als IIS niet wordt uitgevoerd, wordt het tijdens de installatie van WSUS 3.0 gestart.
  
#### Als verbindingen met een bestaande WSUS-database geopend zijn, kan de installatie mislukken
  
Als u vanaf een bestaande installatie een upgrade naar WSUS 3.0 uitvoert terwijl verbindingen naar de bestaande WSUS-database geopend zijn (als bijvoorbeeld SQL Server Management Studio geopend is), kan de installatie mislukken. Verbreek alle verbindingen en installeer WSUS 3.0 opnieuw.
  
#### Tijdens de installatie van WSUS wordt de verkeerde map voor databasebestanden weergegeven
  
In het scherm **Gereed voor installatie** van het installatieprogramma van WSUS wordt ten onrechte vermeld dat de bovenliggende map de locatie van de database is. De standaardlocatie is bijvoorbeeld %systemdrive%\\WSUS\\UpdateServicesDbFiles, maar deze locatie wordt onjuist vermeld als %systemdrive%\\WSUS.
  
#### Als WSUS is geïnstalleerd op een computer die beschikt over Multilingual User Interface-taalpakketten met een andere standaardtaal dan Engels, wordt de Help weergegeven in de standaardtaal in plaats van het Engels.
  
Als u beschikt over een computer met Multilingual User Interface-taalpakketten met een andere standaardtaal dan Engels, kunt u WSUS wel installeren als de huidige gebruiker Engelse landinstellingen heeft. De gebruikersinterface wordt weergegeven in het Engels, maar u moet een speciale methode gebruiken om de Help weer te geven in het Engels. Kopieer het CHM-bestand voor de Engelstalige Help (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) naar de hoofdmap voor documentatie (*WSUSInstallDir*\\documentation\\WSUS30Help.chm). Hierna moet de Help op de juiste wijze worden weergegeven in alle talen.
  
Upgradeproblemen  
----------------
  
#### Bij een upgrade van WSUS 3.0 RC naar WSUS 3.0 RTM wordt het SSL-certificaat niet aan de WSUS-website toegewezen
  
De WSUS-website wordt verwijderd en opnieuw gemaakt tijdens een upgrade van WSUS 3.0 RC naar WSUS 3.0 RTM. Daardoor is het SSL-certificaat niet meer toegewezen aan de WSUS-website. U moet het certificaat na de upgrade opnieuw toewijzen.
  
#### Herstel na een mislukte upgrade
  
Als u een upgrade uitvoert van WSUS 2.0 naar WSUS 3.0 en de upgrade om welke reden dan ook mislukt, moet u WSUS 2.0 opnieuw installeren en de back-up van de bijbehorende database terugzetten.
  
#### Het is niet mogelijk om een upgrade van WSUS 2.0 naar WSUS 3.0 uit te voeren als er een WSUS 3.0-database uit een eerdere installatie aanwezig is
  
Als eerder een installatie van WSUS 3.0 hebt uitgevoerd en daarna WSUS 2.0 opnieuw hebt geïnstalleerd, moet u de WSUS 3.0-database van de computer verwijderen voordat u WSUS 3.0 opnieuw probeert te installeren.
  
#### Als de computernaam wordt gewijzigd voordat de upgrade naar WSUS 3.0 wordt uitgevoerd, kan de upgrade mislukken
  
Als u de computernaam wijzigt nadat u WSUS 2.0 hebt geïnstalleerd en voordat u een upgrade naar WSUS 3.0 uitvoert, kan de upgrade mislukken.
  
Gebruik het volgende script om de groepen ASPNET en WSUS Administrators te verwijderen en vervolgens opnieuw toe te voegen. Voer de upgrade vervolgens opnieuw uit.
  
U moet *&lt;DBLocation&gt;* vervangen door de map waarin de database is geïnstalleerd en *&lt;ContentDirectory&gt;* door de lokale opslagmap.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Tijdens de installatie kan een back-up van de oude database worden overschreven
  
De database wordt aan de map toegevoegd die tijdens de installatie van WSUS 3.0 is opgegeven. Dit is standaard *%systemdrive%*\\WSUS\\UpdateServicesDbFiles. Als er in deze map een back-up van de oude database aanwezig is, wordt deze door de nieuwe database overschreven. Beheerders moeten een back-up van databasebestanden maken voordat updates op de computer worden toegepast waarop de database zich bevindt.
  
#### Als u van MSDE bent gemigreerd naar SQL Server 2000 of SQL Server 2005 op WSUS 2.0, moet u mogelijk een registerwaarde wijzigen
  
Als u over een installatie van WSUS 2.0 beschikt en u een migratie vanaf SQL Server 2000 of SQL Server 2005 hebt uitgevoerd, moet u de waarde van **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** van 1 in 0 wijzigen. Als u dat niet doet voordat u een upgrade naar WSUS 3.0 uitvoert, mislukt de upgrade.
  
#### Als de installatie van WSUS 2.0 wordt gestart en geannuleerd, wordt de WSUS-registersleutel verwijderd
  
Als u de installatie van WSUS 2.0 start en vervolgens annuleert, wordt de WSUS-registersleutel verwijderd. Dit kan tot problemen leiden als u WSUS 3.0 al hebt geïnstalleerd. Hetzelfde probleem doet zich voor wanneer u WSUS 2.0 gaat verwijderen, het verwijderen annuleert en vervolgens een upgrade van WSUS 2.0 naar WSUS 3.0 uitvoert.
  
#### Als u WSUS 3.0 verwijdert en de logboekbestanden achterlaat, zijn daarvoor mogelijk niet de juiste machtigingen ingesteld wanneer ze opnieuw worden geïnstalleerd
  
Wanneer u WSUS 3.0 verwijdert, kunt u ervoor kiezen de logboekbestanden van de installatie te behouden. Wanneer u WSUS 3.0 opnieuw installeert, worden de machtigingen voor de oude logboekbestanden verwijderd (gewoonlijk alleen voor WSUS Administrators). U moet de machtigingen voor deze logboekbestanden terugzetten.
  
#### Wanneer Windows SharePoint Services na WSUS 3.0 RC is geïnstalleerd, kan er via een omweg een upgrade naar WSUS 3.0 RTM worden uitgevoerd
  
Als u eerst WSUS 3.0 RC en vervolgens Windows SharePoint Services op dezelfde computer hebt geïnstalleerd, kunt u alleen een upgrade naar WSUS 3.0 RTM uitvoeren door op de aangepaste poort (port 8530) te installeren. U voert deze installatie vanaf een opdrachtregel uit door een opdrachtshell te openen en de volgende opdracht in te voeren: **WSUSSetup /q / g/ DEFAULT\_WEBSITE=0**. (U voert deze installatie via de gebruikersinterface uit door **WSUSSetup /g DEFAULT\_WEBSITE=0** te typen.)
  
Als WSUS is geïnstalleerd op een computer waarop Multilingual User Interface-taalpakketten zijn geïnstalleerd, wordt de Help weergegeven in de standaardtaal in plaats van de huidige taal van de gebruiker.
  
#### Als WSUS 2.0-clients beschikken over updates met de status Niet van toepassing, worden de updates enige tijd als Onbekend weergegeven na de upgrade naar WSUS 3.0
  
Als een WSUS 2.0-server clients heeft die beschikken over updates met de status Niet van toepassing, worden deze updates enige tijd als Onbekend weergegeven na de upgrade van de server naar WSUS 3.0 De updatestatus wordt na de volgende scan van de client weer ingesteld op Niet van toepassing.
  
Bekende kwesties  
----------------
  
#### Het oplossen van problemen bij meerdere downloadfouten of herhaalde fouten bij clientsynchronisatie
  
Als WSUS 3.0-clients meerdere downloadfouten rapporteren of als clients gedurende langere tijd niet met de WSUS 3.0-server kunnen worden gesynchroniseerd, is mogelijk een clientdownloadcache beschadigd. U kunt deze fout herstellen door te proberen de clientdownloadcache uit het bestandssysteem te verwijderen.
  
De clientdownloadcache verwijderen:
  
1.  Verwijder alle bestanden en submappen op de volgende locatie op de clientcomputer: **%windir%\\SoftwareDistribution\\Download**  
2.  Probeer de update te installeren door de clientcomputer opnieuw te synchroniseren met WSUS 3.0. De installatiepoging moet mislukken en de volgende fout moet worden weergegeven: **WU\_E\_DM\_NOTDOWNLOADED, 'De update is niet gedownload."**  
3.  Na deze fout start de clientcomputer de download automatisch opnieuw en kan de installatie worden voortgezet.
  
#### Als het synchronisatieproces mislukt, moet een nieuwe synchronisatiepoging worden uitgevoerd
  
Als het synchronisatieproces mislukt, moet u eerst nogmaals proberen om de server te synchroniseren. Als alle volgende synchronisatiepogingen mislukken, gebruikt u de informatie over het oplossen van problemen in de [Windows Server Update Services 3.0 Operations Guide](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072).
  
#### De WSUS 3.0-configuratie kan niet rechtstreeks in de database worden gewijzigd
  
De configuratiegegevens van Windows Server Update Services worden in een SQL Server-database opgeslagen. U kunt de configuratiegegevens echter niet wijzigen door rechtstreeks in de database wijzigingen aan te brengen. Probeer de WSUS 3.0-configuratie niet te wijzigen door de database rechtstreeks te bewerken. U moet de WSUS 3.0-configuratie wijzigen met behulp van de WSUS 3.0-console of het aanroepen van WSUS 3.0 API's.
  
#### Fouten bij het downloaden worden niet tijdig gerapporteerd als schijfquota zijn ingeschakeld
  
Als schijfquota zijn ingeschakeld en het quotum wordt bereikt, worden fouten bij het downloaden op de WSUS-server mogelijk niet tijdig gerapporteerd. U kunt dit probleem voorkomen door schijfquota uit te schakelen of de quota te verhogen.
  
#### Als WSUS 3.0 wordt geïmplementeerd met behulp van SSL, kan op clientcomputers de foutcode 0x8024400a worden weergegeven
  
Op clientcomputers kan soms de foutcode '0x8024400a' worden weergegeven bij communicatie met een WSUS 3.0-server via SSL. Raadpleeg het artikel [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593) voor een update waarmee dit probleem wordt opgelost.
  
#### De WSUS-domeinbeheerdersaccount wordt niet verwijderd wanneer WSUS wordt verwijderd
  
De groep WSUS Administrators wordt gemaakt als een domeinaccount (en geen lokale account) op domeincontrollers. Alle installaties die deze domeinaccount gebruiken, zouden dus worden uitgeschakeld als de account werd verwijderd bij het verwijderen van WSUS. De WSUS-domeinbeheerdersaccount wordt daarom gehandhaafd wanneer WSUS wordt verwijderd.
  
#### Als een downstream-server wordt geconverteerd naar een upstream-server, moeten updates van de catalogussite opnieuw worden geïmporteerd
  
Wanneer u een downstream-server converteert naar een upstream-server, moet u ook alle updates van de catalogussite opnieuw importeren. Als u dit niet doet, worden de nieuwe revisies van catalogussite-updates niet gesynchroniseerd naar deze server.
  
#### Als u IIS gebruikt in combinatie met SSL, is niet-gecodeerde toegang nog steeds mogelijk, tenzij de optie 'Beveiligd kanaal vereisen' is ingeschakeld
  
Als u IIS instelt op het gebruik van SSL door een certificaat te installeren, is toegang tot de site via niet-gecodeerde HTTP nog steeds mogelijk, tenzij de optie 'Beveiligd kanaal vereisen' is ingeschakeld. Raadpleeg het artikel over [inschakelen van codering](http://go.microsoft.com/fwlink/?linkid=70601) (http://go.microsoft.com/fwlink/?LinkId=70601) voor meer informatie.
  
#### Het importeren van de catalogussite kan mislukken als er geen machtiging voor lezen en schrijven is voor de map %windir%\\TEMP
  
Wanneer een catalogussite wordt geïmporteerd en de Network Service-account geen machtiging voor lezen en schrijven heeft voor de map %windir%\\TEMP, kan het importeren mislukken en wordt een foutbericht van de volgende strekking weergegeven: 'Server kan de aanvraag niet uitvoeren. ---&gt; Kan bestand 'C:\\WINDOWS\\TEMP\\*tempFileName*.dll' niet vinden.'
  
#### De prestaties nemen af wanneer u synchroniseert tussen WSUS 3.0 en een downstream replica-server waarop WSUS 2.0 wordt uitgevoerd
  
Als u WSUS 3.0 installeert op een upstream-server en probeert te synchroniseren met een downstream replica-server waarop WSUS 2.0 wordt uitgevoerd, ondervindt u problemen met de prestaties. Raadpleeg het artikel [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669) voor een oplossing van dit probleem.
  
#### Als de e-mailserver niet actief is of niet kan worden bereikt, worden geen e-mailmeldingen verzonden
  
Als de e-mailserver van het netwerk offline is, verzendt WSUS 3.0 geen e-mailmeldingen en wordt daarover geen foutbericht weergegeven. Gebeurtenis 10052 (HealthCoreEmailNotificationRed) wordt echter wel naar het gebeurtenislogboek weggeschreven.
  
#### Gewijzigde instellingen op een upstream-server worden niet direct doorgevoerd op de downstream-server
  
Wanneer de configuratie van de upstream-server wordt gewijzigd, kan het enige tijd duren voordat deze configuratiewijzigingen van kracht worden. Als u bijvoorbeeld een instelling voor het selecteren van een nieuwe taal wijzigt op de upstream-server en direct een synchronisatiesessie met de downstream-server start, wordt de wijziging niet doorgevoerd op de downstream-server. Dit gebeurt pas tijdens de volgende geplande synchronisatie. De wachttijd neemt toe al naar gelang het aantal updates op de upstream-server.
  
#### Wanneer WSUS 3.0 wordt verwijderd, wordt de database-instantie niet verwijderd
  
Wanneer WSUS 3.0 wordt verwijderd, wordt de database-instantie niet verwijderd. De instantie kan door meerdere toepassingen worden gebruikt. Als die instantie wordt verwijderd, kan dat problemen voor de desbetreffende toepassingen geven.
  
Als u Windows Internal Database moet verwijderen, kunt u de volgende opdrachten gebruiken:
  
(op 32-bits platforms)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(op 64-bits platforms)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Als u Windows Internal Database Service Pack 2 van Windows Server 2008 wilt verwijderen, kunt u dat via Server Manager doen.
  
Door de toepassing te verwijderen worden echter niet de standaard MDB- en LBD-bestanden verwijderd. Daardoor zal een daaropvolgende installatie van WSUS 3.0 mislukken. U kunt deze bestanden verwijderen uit de map %windir%\\SYSMSI\\SSEE.
  
#### Als de upstream-server van een downstream-server wordt gewijzigd, worden updates met de status 'Onbekend' vermeld als 'Niet van toepassing'
  
Als een downstream-server de synchronisatie start vanaf een andere upstream-server, worden updates met de status 'Onbekend' op de nieuwe upstream-server vermeld als 'Niet van toepassing'. Deze status is tijdelijk en wordt gecorrigeerd wanneer de status van de downstream-server de volgende keer wordt gerapporteerd, nadat de bijbehorende clients met de downstream-server zijn gesynchroniseerd.
  
#### Als een replica-server met WSUS 3.0 meerdere computers met dezelfde naam beheert, mislukt het totaliseren van rapporten
  
Als een replica-server met WSUS 3.0 meerdere computers met dezelfde naam beheert, mislukt het totaliseren van rapporten. De rapporten die voor de basis-WSUS-server beschikbaar zijn, zijn dan onvolledig. U kunt dit probleem oplossen door op de replica-server alle dubbele computervermeldingen te verwijderen zodat u één unieke vermelding overhoudt.
  
#### Als de wizard Server opschonen vanaf een externe console op meerdere servers wordt uitgevoerd en op één server een time-out ondervindt, wordt de verbinding met alle servers verbroken
  
U kunt de wizard Server opschonen op meerdere servers uitvoeren vanaf één externe console. Als tijdens het opschonen echter een time-out optreedt op een van de servers, verliest de console de verbinding met alle servers. Er gaan een gegevens verloren, maar de beheerder moet de externe verbinding met elke server opnieuw instellen.
  
#### Bestanden worden door de wizard Server opschonen na dertig dagen verwijderd, niet na drie maanden
  
Sommige tekst in de wizard Server opschonen is onjuist. De melding luidt als volgt: 'Updates verwijderen die zijn verlopen en drie maanden lang niet zijn goedgekeurd, en oude revisies van updates verwijderen die drie maanden lang niet zijn goedgekeurd.' De juiste periode is dertig dagen, niet drie maanden.
  
#### Als de verbinding snel achter elkaar wordt gestart en verbroken, wordt het foutbericht 'Geen fouten' in de configuratiewizard weergegeven
  
Wanneer u WSUS gaat configureren, moet u verbinding maken met de upstream-server (Microsoft Update of de upstream-server van het intranet) om basisgegevens van de server over te dragen. Als u op **Verbinding maken** en meteen daarna op **Verbinding verbreken** klikt, ontvangt u het onjuiste foutbericht 'Er is geen synchronisatiefout opgetreden'.
  
#### WSUS-clients met Windows Vista RTM kunnen nu naar updates op Microsoft Update zoeken
  
In vorige versies van WSUS konden clients met Windows Vista RTM alleen updates van de WSUS-server ophalen. Met WSUS 3.0 RTM kunnen Vista-clients updates nu ook van Microsoft Updates ophalen. U kunt Vista-clients naar Microsoft Update omleiden door Windows Update vanuit het Configuratiescherm te starten en op de hyperlink **Online controleren op updates van Microsoft Update** te klikken. Als de groepsbeleidsoptie **Toegang tot alle functies van Windows Update verwijderen** is ingeschakeld, wordt de hyperlink niet door Windows Update weergegeven.
  
WSUS 3.0 op Windows Server 2008  
-------------------------------
  
#### Ondersteunde versies
  
WSUS 3.0 ondersteunt Windows Server 2008 zowel in 32-bits als in 64-bits versies.
  
#### Vereisten
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Vereist</th>
<th>Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">IIS (Microsoft Internet Information Services)</td>
<td style="border:1px solid black;">Moet worden geïnstalleerd vanuit het besturingssysteem. De volgende onderdelen moeten zijn ingeschakeld:
Windows-verificatie
Statische inhoud
ASP.NET
Compatibiliteit met 6.0-beheer
Compatibiliteit met IIS-metabase</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herdistribueerbaar pakket (x86) voor Microsoft .NET Framework versie 2.0</td>
<td style="border:1px solid black;">Niet nodig op Windows Server 2008, omdat dit al als onderdeel van het besturingssysteem is geïnstalleerd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">Niet nodig op Windows Server 2008, omdat dit al als onderdeel van het besturingssysteem is geïnstalleerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dit is een vereiste om de gebruikersinterface van WSUS te kunnen gebruiken. Raadpleeg het artikel met informatie over het herdistribueerbare pakket voor Microsoft Report Viewer 2005 in het <a href="http://go.microsoft.com/fwlink/?linkid=70410">Downloadcentrum van Microsoft</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### Kwestie 1: Het configuratiebestand van IIS 7.0 moet worden bijgewerkt voordat WSUS 3.0 wordt uitgevoerd
  
Voordat WSUS 3.0 op Windows Server 2008 wordt uitgevoerd, moet eerst het IIS-configuratiebestand worden bijgewerkt. U moet hiervoor het volgende doen:
  
1. Open het IIS-configuratiebestand: %WINDIR%\\system32\\inetsrv\\applicationhost.config
  
2. Verwijder &lt;add name="CustomErrorMode"&gt; uit de code &lt;System.webServer&gt;&lt;modules&gt;.
  
3. Voeg &lt;remove name="CustomErrorMode"&gt; aan de code &lt;System.webServer&gt;&lt;modules&gt; toe.
  
De code ziet er nu zo uit:
  
```  
 &lt;System.webServer&gt; &lt;modules&gt; &lt;remove name="CustomErrorMode"&gt; &lt;/modules&gt; &lt;/System.webServer&gt;  
```
  
#### Kwestie 2: Als u WSUS 3.0 op de aangepaste poort op Windows Server 2008 Beta 3 wilt installeren, moet u de website van tevoren maken
  
Als u WSUS 3.0 op Windows Server 2008 Beta 3 wilt installeren en u WSUS wilt instellen op het gebruik van de aangepaste poort 8530, moet u een website met de naam 'WSUS Administration' op poort 8530 maken voordat u het WSUS-installatieprogramma start.
  
WSUS 3.0 onder Windows Small Business Server 2003  
-------------------------------------------------
  
#### Kwestie 1: Als de virtuele hoofdmap voor IIS beperkt is tot bepaalde IP-adressen of domeinnamen, is de WSUS 3.0-server niet in staat om zichzelf bij te werken
  
Bij sommige installaties van Windows Small Business Server is de standaard IIS-website geconfigureerd voor 'IP-adres en domeinnaambeperkingen'. Als dat zo is, kan de Windows Update-client op de server zichzelf waarschijnlijk niet bijwerken.
  
#### Kwestie 2: Integratieproblemen bij het installeren van WSUS 3.0 onder Small Business Server
  
-   Als Windows Small Business Server 2003 een ISA-proxyserver gebruikt om toegang te krijgen tot internet, moeten de volgende instellingen handmatig bij **Instellingen** worden ingevoerd: de instellingen, naam en poort van de proxyserver.  
-   Als ISA Windows-verificatie gebruikt, moeten de proxyserver-referenties in de volgende vorm worden ingevoerd: 'DOMEIN\\gebruiker' (de gebruiker die behoort tot de groep Internetgebruikers).
  
#### Kwestie 3: Als u een subnet aan uw netwerk hebt toegevoegd zonder de Windows SBS-wizards te gebruiken, moet u deze procedure uitvoeren
  
Tijdens de installatieprocedure van de WSUS-server worden twee virtuele hoofdmappen voor IIS op de server geïnstalleerd: SelfUpdate en ClientWebService. Setup plaatst tevens enkele bestanden in de hoofdmap van de standaardwebsite (op poort 80) waarmee clientcomputers een zelf-update kunnen uitvoeren via de standaardwebsite. De standaardwebsite is echter standaard zodanig geconfigureerd, dat deze elk IP-adres of elke localhost de toegang weigert, behalve de localhost of specifieke subnets van de server. Clientcomputers die zich niet op de localhost of op de specifieke subnets bevinden, kunnen dus geen zelf-update uitvoeren. Als u een subnet aan uw netwerk hebt toegevoegd zonder de Windows SBS-wizards (Microsoft Windows Small Business Server 2003) te gebruiken, moet u deze procedure uitvoeren.
  
1.  Vouw in Serverbeheer achtereenvolgens **Geavanceerd beheer**, **Internet Information Services**, **Websites** en **Standaardwebsite** uit, klik met de rechtermuisknop op de virtuele map **Selfupdate** en klik op **Eigenschappen**.  
2.  Klik op **Mapbeveiliging**.  
3.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik op **Toegang verleend**.  
4.  Klik op **OK**, klik met de rechtermuisknop op de virtuele map **ClientWebService** en klik op **Eigenschappen**.  
5.  Klik op **Mapbeveiliging**.  
6.  Klik onder **IP-adres en domeinnaambeperkingen** op **Bewerken** en klik op **Toegang verleend**.
  
#### Copyright
  
Dit document biedt ondersteuning voor een voorlopige versie van een softwareproduct dat nog aanzienlijk kan worden gewijzigd voordat de eindversie beschikbaar komt. Dit document is vertrouwelijk en de informatie is eigendom van Microsoft Corporation. Deze informatie wordt openbaar gemaakt volgens een geheimhoudingsovereenkomst tussen de ontvanger van het document en Microsoft. Microsoft verstrekt dit document uitsluitend ter informatie en zonder enige impliciete of expliciete garantie. De informatie in dit document, URL's en andere verwijzingen naar websites op internet inbegrepen, is onderhevig aan wijziging zonder voorafgaande kennisgeving. Het risico van het gebruik of de resultaten van het gebruik van dit document berust geheel bij de gebruiker. Tenzij anders vermeld, zijn alle in de voorbeelden in dit document vermelde bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen fictief. Eventuele overeenkomsten met bestaande bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen berusten geheel op toeval. De gebruiker is verantwoordelijk voor naleving van alle geldende wetten inzake auteursrecht. Behoudens de in of krachtens de Auteurswet van 1912 gestelde uitzonderingen mag niets uit deze uitgave worden verveelvoudigd en/of openbaar gemaakt door middel van druk, fotokopie, microfilm of op welke andere wijze dan ook en evenmin in een gegevensopzoeksysteem worden opgeslagen zonder voorafgaande schriftelijke toestemming van Microsoft Corporation.
  
Microsoft is mogelijk in het bezit van octrooien, aanvragen voor octrooien, merken, auteursrechten of andere intellectuele eigendomsrechten met betrekking tot materiaal in dit document. De aanschaf van dit document geeft u geen licentie ten aanzien van deze octrooien, merken, auteursrechten of andere intellectuele eigendomsrechten, tenzij expliciet vermeld in een schriftelijke gebruiksrechtovereenkomst van Microsoft.
  
© 2007 Microsoft Corporation. Alle rechten voorbehouden.
  
Microsoft, SQL Server, Windows en Windows Server zijn merken of gedeponeerde merken van Microsoft Corporation.
  
Alle andere merken zijn eigendom van hun respectieve eigenaren.
