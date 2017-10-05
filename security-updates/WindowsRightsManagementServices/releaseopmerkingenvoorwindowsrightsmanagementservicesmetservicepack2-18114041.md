---
TOCTitle: Releaseopmerkingen voor Windows Rights Management Services met Service Pack 2
Title: Releaseopmerkingen voor Windows Rights Management Services met Service Pack 2
ms:assetid: '78067886-681f-49a6-b43d-bfd08a369b69'
ms:contentKeyID: 18114041
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747637(v=WS.10)'
---

Releaseopmerkingen voor Windows Rights Management Services met Service Pack 2
=============================================================================

*Releasedatum: December 2006*

Voordat u begint
----------------

Neem kennis van de volgende informatie voordat u Microsoft® Windows® Rights Management Services (RMS) met Service Pack 2 (SP2) installeert. De informatie in deze releaseopmerkingen is van toepassing op de RMS met SP2-server en niet op de RMS-client. Zie Rights Management Services ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) voor informatie over RMS-clients.

#### Systeemvereisten

De volgende tabel bevat de hardwarevereisten voor het uitvoeren van RMS met SP2.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Vereist</th>
<th style="border:1px solid black;" >Aanbevolen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Computer met één Pentium III-processor (800 MHz of hoger)</td>
<td style="border:1px solid black;">Computer met twee Pentium 4-processors (1500 MHz of hoger)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">256 MB RAM</td>
<td style="border:1px solid black;">512 MB RAM</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">20 GB vrije ruimte op de vaste schijf</td>
<td style="border:1px solid black;">40 GB vrije ruimte op de vaste schijf</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                      |  
|-------------------------------------------------------------------------------------------------------------------------------------------------|  
| RMS met SP2-server is ontworpen voor een 32-bits computer. Bij installatie op een 64-bits computer wordt de server uitgevoerd in emulatiemodus. |
  
De volgende tabel bevat de softwarevereisten voor het uitvoeren van RMS met SP2.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Onderdeel</th>
<th style="border:1px solid black;" >Vereist</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Besturingssysteem</td>
<td style="border:1px solid black;">Microsoft Windows Server® 2003, uitgezonderd Web Edition, voor RMS met SP2.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rights Management Services met SP2</td>
<td style="border:1px solid black;">RMS met Service Pack 1 (SP1) moet zijn geïnstalleerd voordat u een upgrade kunt uitvoeren naar RMS met SP2. Dit vereiste geldt niet voor de RMS met SP2-client.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bestandssysteem</td>
<td style="border:1px solid black;">Het NTFS-bestandssysteem wordt aanbevolen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Onderdelen die aanwezig moeten zijn</td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (ofwel MSMQ) met Active Directory® Directory Service-integratie ingeschakeld.<br />
<br />
</li>
<li>Internet Information Services (IIS) met ASP.NET ingeschakeld.<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U kunt RMS met SP2 zo configureren dat beheer op afstand mogelijk is. De computer die verbinding maakt met de RMS met SP2-beheerservice moet gebruikmaken van Internet Explorer 6.0 of later. |

De volgende tabel bevat de infrastructuurvereisten voor servers waarop RMS met SP2 wordt uitgevoerd.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Onderdeel</th>
<th style="border:1px solid black;" >Vereisten</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Directory-services</td>
<td style="border:1px solid black;">Active Directory uitgevoerd op domeincontrollers met Windows Server 2000 met Service Pack 3 (SP3) of later, in hetzelfde domein waarin RMS is geïnstalleerd. Alle gebruikers en groepen die met RMS licenties verkrijgen en inhoud publiceren, moeten over een e-mailadres beschikken dat in Active Directory is geconfigureerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Databaseserver</td>
<td style="border:1px solid black;">RMS met SP2 vereist een database en opgeslagen procedures om bewerkingen te kunnen uitvoeren. U kunt Microsoft SQL Server™ 2000 met SP3a of later gebruiken, of Microsoft SQL Server 2005. Voor testdoeleinden of andere toepassingen voor één computer, kan Microsoft SQL Server Desktop Engine (MSDE 2000) Release A of Microsoft SQL Server 2005 Express Edition worden gebruikt.</td>
</tr>
</tbody>
</table>
  
RMS is ontworpen voor en getest met databaseservers waarop Microsoft SQL Server 2000 en Microsoft SQL Server 2005 worden uitgevoerd. RMS kan op andere databaseservers worden uitgevoerd als die voldoen aan de volgende criteria:
  
-   Ondersteuning bieden aan ADO.NET-interfaces die onderdeel zijn van Microsoft .NET Framework 1.1.  
-   Compatibel zijn met Transact-SQL, de gestructureerde querytaal waar Microsoft SQL Server gebruik van maakt, omdat RMS-initialisatiescripts en opgeslagen procedures van RMS gebruikmaken van Transact-SQL.  
-   Ondersteuning bieden voor alle Microsoft SQL Server-specifieke extensies.  
-   Reageren op methodeaanroepen van de System.Data.SqlClient-naamruimte van .NET Framework.  
-   De bijbehorende functionaliteit van de System.Data.SqlClient-naamruimte verstrekken.  
-   Windows-verificatiemodus gebruiken.
  
Om vast te stellen of de databaseserver voldoet aan de bovenstaande criteria neemt u contact op met de leverancier van de desbetreffende database.
  
De volgende tabel bevat de gebruikersrechten en -machtigingen die nodig zijn voor het uitvoeren van verschillende activiteiten met RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Activiteit</th>
<th style="border:1px solid black;" >Accountvereisten</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS installeren</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Een RMS-basiscluster inrichten</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden en Zoekopdrachten uitvoeren en schrijven in Active Directory</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Een cluster inrichten uitsluitend voor RMS-licentieverlening</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden en Zoekopdrachten uitvoeren in Active Directory</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Inrichten met gebruikmaking van een nieuwe configuratiedatabase</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden en machtigingen voor lezen, schrijven en maken op een computer waarop SQL Server wordt uitgevoerd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Inrichten met gebruikmaking van een bestaande configuratiedatabase</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden en machtigingen voor lezen en schrijven op de computer waarop de databaseserver wordt uitgevoerd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS beheren</td>
<td style="border:1px solid black;">Domeingebruiker met lokale beheerdersbevoegdheden</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                                                                                                                                                               |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Raadpleeg Help en ondersteuning van Windows Server 2003 Techcenter [http://go.microsoft.com/fwlink/?LinkId=7813](http://go.microsoft.com/fwlink/?linkid=78135) voor meer informatie over de configuratie van Windows Server, Active Directory, Message Queuing, IIS en bestandssystemen. |
  
Als u RMS in een clusterinstallatie gebruikt, moet u de problemen hebben verholpen die in de volgende tabel worden opgesomd.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Voorwaarde</th>
<th style="border:1px solid black;" >Aanbevolen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Een groot aantal computers maakt gebruik van RMS</td>
<td style="border:1px solid black;">Gebruik Systems Management Server (SMS) of Groepsbeleid om de RMS met SP2-client te installeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Een groot aantal clientaanvragen</td>
<td style="border:1px solid black;">Gebruik een taakverdelingsserver, de Network Load Balancing-service van Windows Server of hardwaretaakverdeling om de aanvragen te distribueren over de cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Twee netwerkinterfacekaarten die gebruikmaken van virtuele IP-adressering om aan de aanvragen van het extranet en het intranet te voldoen</td>
<td style="border:1px solid black;">Zorg ervoor dat een DNS-registratie (Domain Name System) die het virtuele IP-adres zichtbaar maakt op het extranet dat adres tevens zichtbaar maakt op het intranet.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                                                                                                                                |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als voor het intranet geen DNS-toewijzing wordt uitgevoerd, dan mislukken interne aanvragen voor clientlicenties. Als u de DNS-instellingen niet kunt veranderen, wijzigt u de hosts-tabel van elke server in de cluster om de cluster-URL toe te wijzen aan het virtuele IP-adres van de cluster. DNS-toewijzing moet worden gedaan voordat RMS wordt ingericht. Als u de service al hebt ingericht, moet u RMS van de server verwijderen en de inrichtingsprocedure herhalen. |
  
#### Ondersteunde clients voor deze versie
  
De RMS-client zonder servicepack, de RMS-client met SP1 of de RMS-client met SP2 kan worden geïnstalleerd op elke computer waarop Microsoft Windows 2000, Windows XP of Windows Server 2003 wordt uitgevoerd. Eerdere versies van het Windows-besturingssysteem worden niet ondersteund door deze versie.
  
| ![](images/Cc747637.Caution(WS.10).gif)Waarschuwing                                                                   |  
|----------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u werkt met de RMS-client zonder servicepack, is de client niet in staat online publicatie te gebruiken tegen een RMS-server met SP1 of later. |
  
Wijzigingen in functionaliteit  
------------------------------
  
RMS met SP2 bevat verschillende nieuwe functies:
  
-   [Verbeterde groepsuitbreiding naar andere forests](#bkmk_cif1)  
-   [Wijzigingen in databaselogboekregistratie](#bkmk_cif2)  
-   [Grotere omvang van serverbatches](#bkmk_cif3)  
-   [Compatibiliteit met Microsoft SQL Server 2005](#bkmk_cif4)
  
<span id="BKMK_CIF1"></span>
#### Verbeterde groepsuitbreiding naar andere forests
  
#### Wat is het effect van deze functie?
  
In RMS vergemakkelijkt de groepsuitbreiding in forests de mogelijkheid voor RMS om het groepslidmaatschap voor Active Directory Universal uit te breiden in een andere forest, waar groepslidmaatschappen niet tussen twee forests worden gerepliceerd. Wanneer een gebruiker in het ene forest met rechten beveiligde inhoud naar een gebruiker in een ander forest verstuurd, gaat RMS door een ontdekkingsfase waarbij wordt gecontroleerd of de gebruiker toegang heeft tot de inhoud. Dit controleproces wordt gedaan met behulp van een LDAP-query van het ene forest naar het andere om het RMS-serviceverbindingspunt (SCP) van het externe forest te vinden. Wanneer het serviceverbindingspunt (SCP) voor het externe forest is gevonden, verzendt de RMS-service een aanvraag naar de pipeline van de groepsuitbreiding. De aanvraag bij het externe forest dient om vast te stellen of een gebruiker lid is van een groep.
  
#### Voor wie is deze voorziening van belang?
  
Deze nieuwe functie is van belang voor RMS-klanten in een Active Directory-omgeving met meerdere forests waarvan de Universal-groepslidmaatschappen niet tussen de verschillende forests worden gerepliceerd.
  
#### Waarom is deze wijziging belangrijk?
  
Het nieuwe forest-vertrouwensuitbreidingsprotocol verbetert de betrouwbaarheid voor klanten die een Active Directory-omgeving met meerdere forests implementeren.
  
#### Wat werkt er anders?
  
Voor RMS met SP2 werd groepsuitbreiding over meerdere forests bereikt met externe .NET-aanroepen. In deze release is het protocol voor groepsuitbreiding over meerdere forests gewijzigd in een ASP.NET-webservice met SOAP/HTTP-aanvragen naar de pipeline van de groepsuitbreiding voor de forest-vertrouwensrelatie.
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                                                                                                                                                                     |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Ten behoeve van de achterwaartse compatibiliteit worden externe .NET-aanroepen nog steeds ondersteund in RMS met SP2. Om echter volledig te kunnen profiteren van het nieuwe protocol voor groepsuitbreiding over meerdere forests, moeten alle RMS-clusters ten minste RMS met SP2 uitvoeren. |
  
#### Welke instellingen zijn toegevoegd aan of gewijzigd in RMS met SP2?
  
In RMS met SP2 wordt de nieuwe pipeline voor RMS-groepsuitbreiding standaard geconfigureerd met de allerhoogste beveiligingsinstellingen. Alleen de lokale RMS-service- en Administrators-groepen hebben toegang tot die instellingen. Als u een account toegang wilt verlenen, moet u de toegangscontrolelijst wijzigen voor de pipeline van de groepsuitbreiding op wwwroot\\\_wmcs\\GroupExpansion\\GroupExpansion.asmx.
  
| ![](images/Cc747637.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Zorg ervoor dat de RMS-serviceaccount van elk Active Directory-forest toegang heeft tot de pipeline voor de groepsuitbreiding op elke RMS-server in de cluster. Als de accounts geen toegang hebben, mislukt de groepsuitbreiding. U kunt eventueel ook in elk forest dezelfde account aanmaken en hetzelfde wachtwoord toewijzen aan elke account. In dat geval hoeft u slechts die ene account toe te voegen aan de pipeline van de groepsuitbreiding. |
  
Er zijn nieuwe gebeurtenissen toegevoegd aan RMS met SP2 om u te informeren over probleemberichten die niet werden opgenomen in de Message Queuing-service. Deze nieuwe gebeurtenisregistraties omvatten gebeurtenissen waarmee u wordt gemeld dat een bericht niet digitaal kan worden ondertekend of dat het bericht niet kan worden gevalideerd. Enkele voorbeelden van validatieproblemen zijn een beschadigd bericht, een ontbrekende hash of handtekening of een ongeldige hash of handtekening.
  
<span id="BKMK_CIF2"></span>
#### Wijzigingen in databaselogboekregistratie
  
#### Wat is het effect van deze functie?
  
RMS gebruikt de service van een logboekregistratie-listener die alle RMS-communicatie middels Message Queuing naar de logboekdatabase verzendt. De RMS-cluster verzendt berichten naar de Message Queuing-service, de service van de logboekregistratie-listener haalt deze berichten op uit de Message Queuing-wachtrij en schrijft ze naar de logboekdatabase.
  
#### Voor wie is deze voorziening van belang?
  
Deze functie is van belang voor de huidige gebruikers van RMS die de RMS-service van de logboekregistratie-listener gebruiken en voor nieuwe gebruikers van RMS met SP2 die overwegen de RMS-service van de logboekregistratie-listener te gebruiken.
  
#### Waarom is deze wijziging belangrijk?
  
In vorige releases van RMS werd de wachtrij voor RMS-logboekregistratie beveiligd met toegangscontrolelijsten, maar was verificatie niet ingeschakeld. Zonder verificatie heeft een kwaadwillende gebruiker de mogelijkheid foutieve berichten naar de wachtrij voor RMS-logboekregistratie te schrijven.
  
#### Wat werkt er anders?
  
In RMS met SP2 is voorzien in aanvullende verificatie van de berichten die door de RMS-cluster worden verzonden met Message Queuing. Naast toegangscontrolelijsten die onbevoegde toegang tot de berichtenwachtrij voorkomen, wordt de Message Queuing-wachtrij tevens beveiligd door een verificatiemechanisme voor de authenticiteit van berichten. Wanneer een bericht naar de Message Queuing-service wordt verzonden, genereren de RMS-pipelines een hash van het bericht en voegen ze een digitale handtekening toe met de persoonlijke sleutel van de RMS-cluster. De service van de logboekregistratie-listener berekent eerst een eigen hash van het bericht en vergelijkt die met de hash die bij het bericht is gevoegd. Als de hashes overeenkomen, controleert de service van de logboekregistratie-listener de handtekening aan de hand van de openbare sleutel van de cluster en de hash in het bericht. Pas als de hashes overeenkomen en de handtekening is geverifieerd, wordt het bericht naar de logboekdatabase verzonden. Als de validatiestappen geen succes hebben, wordt het bericht permanent verwijderd uit de Message Queuing-wachtrij en wordt een gebeurteniswaarschuwing geschreven naar het gebeurtenislogboek voor toepassingen in Logboeken.
  
#### Welke instellingen zijn toegevoegd aan of gewijzigd in RMS met SP2?
  
Er zijn nieuwe gebeurtenissen toegevoegd aan RMS met SP2 die er op zijn gericht aan te geven wanneer probleemberichten niet werden opgenomen in de Message Queuing-wachtrij. Deze nieuwe gebeurtenissen worden naar het gebeurtenislogboek voor toepassingen geschreven en bevatten berichten die niet digitaal kunnen worden ondertekend of waarvan de digitale handtekeningen in het bericht niet kunnen worden gevalideerd. Enkele voorbeelden van validatieproblemen zijn een beschadigd bericht, een ontbrekende hash of handtekening of een ongeldige hash of handtekening.
  
<span id="BKMK_CIF3"></span>
#### Grotere omvang van serverbatches
  
#### Wat is het effect van deze functie?
  
Batchverwerking in RMS verbetert de prestaties omdat het daarmee mogelijk is meerdere licentieaanvragen als één aanvraag te verzenden naar de RMS-cluster in plaats van elke licentieaanvraag afzonderlijk.
  
#### Voor wie is deze functie van belang?
  
De ondersteuning voor een grotere omvang van serverbatches is van belang voor toepassingen met RMS-ondersteuning die in één keer verschillende licenties voor met rechten beveiligde inhoud moeten aanvragen.
  
#### Waarom is deze wijziging belangrijk?
  
Batchverwerking in RMS maakt het mogelijk dat één aanvraag kan worden ingediend bij de AcquireLicense RMS-pipeline om gebruikslicenties te verkrijgen voor meerdere rechtenaccountcertificaten (RAC's) tegen een of meerdere publicatielicenties. Zonder batchomvang groter dan 1 zou de toepassing met RMS-ondersteuning voor elke gebruiker afzonderlijk een aanvraag voor een gebruikslicentie moeten indienen.
  
#### Wat werkt er anders?
  
In RMS-versies ouder dan RMS met SP2 ondersteunt de RMS-cluster een maximale batchgrootte van 1. Als de maximumgrootte zou worden ingesteld op een getal hoger dan 1, zou de cluster dat negeren. In RMS met SP2 bedraagt de maximale batchomvang 100.
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                      |  
|-------------------------------------------------------------------------------------------------|  
| Alleen de AcquireLicense RMS-pipeline biedt ondersteuning voor in batches aangeboden aanvragen. |
  
Foutrapportage in RMS met SP2 is uitgebreid ten behoeve van in batches aangeboden aanvragen. Als u bijvoorbeeld een batch van tien aanvragen verstuurt, en de tweede en derde aanvraag mislukken, wordt een gebeurtenis geschreven naar het gebeurtenislogboek voor elke mislukte aanvraag.
  
<span id="BKMK_CIF4"></span>
#### Compatibiliteit met Microsoft SQL Server 2005
  
#### Wat is het effect van deze functie?
  
In RMS met SP2 kunt u Microsoft SQL Server 2005 gebruiken als databaseserver ter ondersteuning van de RMS-configuratie en -logboekdatabases zonder een extra configuratie uit te voeren.
  
#### Voor wie is deze functie van belang?
  
De ondersteuning voor Microsoft SQL Server 2005 met RMS met SP2 is van belang voor RMS-klanten die Microsoft SQL Server 2005 willen gebruiken als hun RMS-database.
  
#### Waarom is deze wijziging belangrijk?
  
In eerdere versies van RMS waren de gegevenstypen van een aantal parameters in de tabel sysmessages niet compatibel met de Microsoft SQL Server 2005-indeling. Zie voor meer informatie artikel 913372 de [Microsoft Knowledge Base](http://go.microsoft.com/fwlink/?linkid=68638) (http://go.microsoft.com/fwlink/?LinkID=68638).
  
#### Wat werkt er anders?
  
In RMS-versies ouder dan RMS met SP2 werden SQL RAISERROR-instructies gebruikt om de RMS-gebruiker te informeren dat er een fout was opgetreden. Via de RAISERROR-instructie wordt een query uitgevoerd op de sysmessages-tabel om de RMS-foutberichten op te halen die in deze tabel zijn opgeslagen. RMS met SP2 gebruikt nu een andere techniek om SQL-fouten door te geven, waarbij niet langer een afhankelijkheid bestaat van de sysmessages-tabel.
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                     |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u een upgrade uitvoert van RMS met SP1 naar RMS met SP2, wordt voor foutberichten geen query meer uitgevoerd op de sysmessages-tabel, maar blijven de foutberichten zelf aanwezig in de sysmessages-tabel. Met een schone installatie van RMS met SP2 worden geen nieuwe vermeldingen aan de sysmessages-tabel toegevoegd. |
  
Bekende problemen  
-----------------
  
In de volgende gedeelten worden de bekende problemen voor deze versie van RMS beschreven.
  
#### Help-bestand verwijst nog steeds naar RMS met Service Pack 1
  
Het Help-bestand dat onderdeel is van de installatie van RMS met SP2 verwijst nog naar RMS met SP1. Zie Rights Management Services ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) voor informatie over RMS met SP2.
  
#### Windows Update slaagt er niet in RMS met SP2-client te installeren op x64- of Itanium-computers
  
Als de RMS-client of de RMS met SP1-client op een x64-computer is geïnstalleerd en u probeert met behulp van Windows Update een upgrade van de client uit te voeren naar RMS met SP2-client (x64), mislukt de installatie. Hoewel de voorgaande RMS-clients, die werden gemaakt voor 32-bits systemen, werkten op x64-computers, kunnen die niet worden bijgewerkt naar RMS met SP2-client (x64). U moet eerst de installatie van de vorige RMS-client ongedaan maken en vervolgens de update opnieuw starten. Windows Update detecteert de versie van het besturingssysteem en stelt de juiste RMS met SP2-client voor. Hetzelfde geldt voor Itanium-computers.
  
#### Na opnieuw inrichten start de service van de logboekregistratie-listener niet meer
  
Bij het ongedaan maken van de inrichting van de cluster, wordt de service van de logboekregistratie-listener niet achtergelaten in de toestand Gestopt. Om de service volledig te stoppen, moet u de computer opnieuw opstarten.
  
#### Kan een niet op software gebaseerd vertrouwd uitgiftedomein niet verwijderen
  
Na het importeren van een vertrouwd uitgiftedomein met een niet op software gebaseerde persoonlijke sleutel, kan dit niet meer worden verwijderd. Het importeren van een niet op software gebaseerde persoonlijke sleutel moet niet worden uitgevoerd vanuit de beheerconsole van Windows Rights Management Services. Neem contact op met de desbetreffende hardwareleverancier voor instructies over het exporteren en importeren van de persoonlijke sleutel.
  
#### Microsoft .NET Framework 2.0 wijzigt de virtuele hoofdmappen van IIS bij een installatie op de RMS-server
  
RMS met SP2 gebruikt de ASP.NET-scripttoewijzing die is opgenomen in .NET Framework versie 1.1. De toewijzing die in latere versies is opgenomen is niet compatibel met RMS met SP2. Beide versies kunnen echter tegelijkertijd zijn geïnstalleerd zonder dat andere afhankelijke toepassingen hierdoor worden gehinderd. Nadat de installatie en inrichting van RMS met SP2 lijkt te zijn geslaagd, werkt de RMS-server mogelijk toch niet goed als .NET Framework 1.1 en .NET Framework 2.0 zijn geïnstalleerd op de server. De reden is dat de virtuele hoofdmappen van RMS moeten worden geregistreerd bij ASP .NET-scripttoewijzingsversie 1.1 in plaats van versie 2.0. Voer de volgende opdracht uit op een opdrachtregel om de virtuele mappen van RMS te registreren bij ASP .NET-scripttoewijzingsversie 1.1:
  
**%windir%\\Microsoft.NET\\Framework\\v1.1.4322&gt;aspnet\_regiis.exe -s W3SVC/1/ROOT/\_wmcs**
  
Met deze opdracht worden de virtuele mappen van RMS correct geregistreerd en kan RMS met SP2 worden uitgevoerd op de server.
  
#### Groepslidmaatschap kan ontbreken bij gebruik van het native functieniveau van Active Directory Windows 2000
  
Wanneer u RMS implementeert in een omgeving waarin de Active Directory-infrastructuurniveaus zijn verhoogd tot het native-functieniveau van Windows 2000, is RMS mogelijk niet in staat het kenmerk memberOf van Active Directory-objecten te lezen bij een poging het groepslidmaatschap uit te breiden van verborgen distributielijsten. RMS kan het kenmerk memberOf alleen lezen wanneer de RMS-serviceaccount een domeinaccount gebruikt die lid is van de groep Pre-Windows 2000-compatibele toegang. Zie voor meer informatie artikel 812841 in de Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=78152](http://go.microsoft.com/fwlink/?linkid=78152)).
  
#### De service van de logboekregistratie-listener verzendt Message Queuing-berichten naar de wachtrij voor onbestelbare berichten wanneer de database niet toegankelijk is
  
Er kunnen zich omstandigheden voordoen (bijvoorbeeld, database niet actief, netwerkproblemen, enzovoort) waarbij de service van de logboekregistratie-listener de database niet kan bereiken. In dat geval worden de berichten verstuurd naar een wachtrij voor onbestelbare berichten. De enige manier om deze berichten te herstellen (dat wil zeggen, te verzenden naar de logboekdatabase) is door gebruik te maken van het hulpprogramma voor RMS-wachtrijherstel dat bij de hulpprogramma's voor het beheer van RMS wordt geleverd. Ga naar [http://go.microsoft.com/fwlink/?LinkId=33841](http://go.microsoft.com/fwlink/?linkid=33841) om de hulpprogramma's voor het beheer van RMS te downloaden.
  
| ![](images/Cc747637.note(WS.10).gif)Opmerking                                                                                                                                                 |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Recover en RecoverandPurge zijn verwijderd uit LogRecoveryCmd. Hierdoor worden alle berichten terug gerouteerd via de Message Queuing-service en geverifieerd voordat het bericht naar de logboekdatabase wordt verzonden. |
  
#### U moet een upgrade uitvoeren naar RMS met SP2 voordat u een upgrade uitvoert naar Microsoft SQL Server 2005
  
Wanneer u een upgrade uitvoert naar RMS met SP2 en een upgrade van Microsoft SQL Server 2000 naar Microsoft SQL Server 2005, voert u eerst de RMS-upgrade uit. Daarmee worden mogelijke compatibiliteitsproblemen vorkomen met de Microsoft SQL Server-upgrade.
  
#### RMS met SP2 kan niet worden ingericht op websites met een apostrof (') in de naam
  
Wanneer u RMS met SP2 probeert in te richten op een website met een apostrof (') in de naam, mislukt het inrichtingsproces en wordt een foutbericht weergegeven waarin een **ongeldige parameter** wordt gemeld. Om RMS met SP2 op de website te kunnen inrichten, verwijdert u de apostrof uit de naam van de website.
  
#### ASP.NET versie 1.1 inschakelen op servers met de 64-bits versie van Windows Server 2003
  
In het onderwerp Systeemvereisten in RMS Help kunt u lezen hoe u .NET Framework 1.1 kunt installeren en ASP.NET 1.1 kunt inschakelen nadat u Internet Information Services (IIS) hebt geïnstalleerd. Als u echter .NET Framework 1.1 installeert voordat u IIS installeert, wordt ASP.NET 1.1 niet vermeld als webservice-extensie en kan de beschreven procedure niet worden gebruikt. Als IIS is geïnstalleerd na de installatie van .NET Framework 1.1, voert u de volgende opdracht uit om ASP.NET in te schakelen :
  
**%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis.exe -i –enable**
  
Wanneer u een latere versie van .NET Framework gebruikt dan versie 1.1, vervangt u **-i** door **-ir** in deze opdracht, om te voorkomen dat bestaande IIS-scripttoewijzingen opnieuw worden ingesteld.
  
#### RMS-serviceaccounts voor externe forests moeten worden toegevoegd aan de pipeline voor lokale groepsuitbreiding
  
Er is een beveiligingsprobleem opgelost waarbij BUILTIN\\users werd verwijderd uit de ACL in de pipeline van de groepsuitbreiding. Hierdoor kunnen scenario's voor groepsuitbreiding naar andere forests onwerkzaam worden. Voer de volgende stappen uit om dit probleem op te lossen:
  
**RMS-serviceaccount toevoegen aan externe forest**  
1.  Ga op Forest1 naar inetpub\\wwwroot\\\_wmcs, waarbij Forest1 de RMS-basiscluster is in het eerste forest.
  
2.  Klik met de rechtermuisknop op de map **GroupExpansion** en selecteer vervolgens **Eigenschappen**.
  
3.  Klik in het venster **Eigenschappen van GroupExpansion** op het tabblad **Beveiliging** en voeg de vermelding toe voor *Forest2\\RmsServiceAccount* (bijvoorbeeld rmil31\\rmsvc), waarbij Forest2 de RMS-basiscluster in het tweede forest is.
  
4.  Klik op **OK**.
  
5.  Klik op **Uitvoeren**, typ **iisreset** en klik vervolgens op**OK**.
  
#### Het uitvoeren van een upgrade van het .NET Framework kan gegevensverlies tot gevolg hebben
  
Als een upgrade van .NET Framework (CLR)-versie 1.1 wordt uitgevoerd nadat RMS is geïnstalleerd en ingericht, worden de virtuele hoofdmappen ingesteld op gebruik van .NET Framework versie 2.0. Als dat het geval is, wordt geen informatie vastgelegd in de logboekdatabase. Dit heeft gegevensverlies tot gevolg. Neem een van de volgende maatregelen:
  
-   Voer de upgrade van .NET Framework uit voordat u RMS installeert en inricht.  
-   Stel de virtuele hoofdmappen in voor het gebruik van 1.1 nadat de upgrade van .NET Framework is uitgevoerd.
  
Documentatiewijzigingen in deze release  
---------------------------------------
  
Hier volgt een lijst van onderwerpen die in deze release zijn gewijzigd:
  
-   Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken ([http://go.microsoft.com/fwlink/?LinkId=70369](http://go.microsoft.com/fwlink/?linkid=70369))  
-   Softwarevereisten voor RMS ([http://go.microsoft.com/fwlink/?LinkId=70371](http://go.microsoft.com/fwlink/?linkid=70371))  
-   Procedures voor het implementeren van de RMS-client ([http://go.microsoft.com/fwlink/?LinkId=70373](http://go.microsoft.com/fwlink/?linkid=70373))  
-   RMS installeren vanaf de opdrachtregel ([http://go.microsoft.com/fwlink/?LinkId=70374](http://go.microsoft.com/fwlink/?linkid=70374))  
-   Tabellen voor basisconfiguratiedatabase van RMS ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70375))  
-   Certificeringstabellen voor configuratiedatabase van RMS ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70376))  
-   Registratiedatabasetabellen van RMS ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70377))  
-   Vereisten voor het aanpassen van de schaal evalueren [http://go.microsoft.com/fwlink/?LinkId=70378](http://go.microsoft.com/fwlink/?linkid=70378))  
-   De RMS-implementatie beveiligen ([http://go.microsoft.com/fwlink/?LinkId=70379](http://go.microsoft.com/fwlink/?linkid=70379))  
-   De service Uit bedrijf nemen inschakelen ([http://go.microsoft.com/fwlink/?LinkId=70380](http://go.microsoft.com/fwlink/?linkid=70380))  
-   Plannen voor externe RMS-gebruikers [http://go.microsoft.com/fwlink/?LinkId=70381](http://go.microsoft.com/fwlink/?linkid=70381))  
-   Ondersteuning van RMS-server voor mobiele apparaten en serverservices inschakelen ([http://go.microsoft.com/fwlink/?LinkId=70382](http://go.microsoft.com/fwlink/?linkid=70382))
  
#### Copyright
  
*De informatie in dit document weerspiegelt de huidige zienswijze van Microsoft Corporation over de onderwerpen die vanaf de publicatiedatum zijn besproken. Aangezien Microsoft moet reageren op een veranderende marktsituatie, vormt dit document geen garantie van de zijde van Microsoft en kan Microsoft de juistheid van deze informatie die na de publicatiedatum wordt gepresenteerd, niet garanderen.*
  
*Dit document is alleen bedoeld ter informatie. MICROSOFT BIEDT GEEN GARANTIES MET BETREKKING TOT DE INFORMATIE IN DIT DOCUMENT, ONGEACHT OF DEZE GARANTIES EXPLICIET, IMPLICIET OF WETTELIJK ZIJN.*
  
*Het is de verantwoordelijkheid van de gebruiker zich te houden aan alle relevante copyrightwetgeving. Met inachtneming van de geldende auteursrechten, mag niets uit dit document worden gereproduceerd, opgeslagen in of toegevoegd aan gegevensbestanden, of openbaar gemaakt in enige vorm of op enige wijze, hetzij elektronisch, mechanisch, door opnamen of anderszins, of voor andere doeleinden worden gebruikt, zonder schriftelijke toestemming van Microsoft Corporation.*
  
*Microsoft heeft mogelijk patenten, patentaanvragen, merken, auteursrechten of andere intellectuele eigendomsrechten die van toepassing zijn op de inhoud in dit document. Tenzij uitdrukkelijk anders vermeld in de schriftelijke gebruiksrechtovereenkomst van Microsoft, geeft dit document u geen recht op deze patenten, merken, auteursrechten of andere intellectuele eigendommen.*
  
*Tenzij anders vermeld, zijn alle namen van bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen fictief. Elke overeenkomst met bestaande bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen berust op toeval.*
  
*© 2006 Microsoft Corporation. Alle rechten voorbehouden.*
  
*Active Directory, Microsoft, MS-DOS, Visual Studio, Windows, Windows Server, SQL Server en Windows NT zijn merken of gedeponeerde merken van Microsoft Corporation.*
  
*De namen van bestaande bedrijven en producten die in dit document worden vermeld, kunnen merken zijn van de desbetreffende eigenaren.*
