---
TOCTitle: 'RMS: Implementatie'
Title: 'RMS: Implementatie'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18113926
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720274(v=WS.10)'
---

RMS: Implementatie
==================

Implementatie van RMS
---------------------

-   [Is er enige afhankelijkheid met de versie van Exchange als de beveiligingsprincipals die voor RMS worden gebruikt, lid van de algemene adreslijst (GAL) zijn?](#bkmk_20)
-   [Welke rol heeft SQL Server in RMS?](#bkmk_21)
-   [Moet de computer van een gebruiker aan hetzelfde domein als dat van de RMS-basiscluster worden toegevoegd om RMS te kunnen gebruiken?](#bkmk_22)
-   [Als een klant de RMS-server in een perimeternetwerk wil plaatsen, welke poorten in de firewall richting internet en de firewall richting het intranet moeten er zijn geopend om met RMS te kunnen communiceren?](#bkmk_23)
-   [Hoe worden onderliggende servers in een cluster exclusief voor licentieverlening ingeschreven en moet ik iets doen met de clients om die bewust te maken van deze cluster?](#bkmk_24)
-   [Wat is het voordeel van het gebruik van een cluster exclusief voor licentieverlening?](#bkmk_25)
-   [Wat moet ik doen om een RMS-installatie helemaal ongedaan te maken?](#bkmk_26)
-   [Moet ik nog bestanden verwijderen als ik via Software in het Configuratiescherm de installatie van RMS ongedaan heb gemaakt?](#bkmk_27)
-   [Werkt RMS in het FAT-bestandssysteem?](#bkmk_28)
-   [Welke hardwareconfiguratie is het beste voor de databaseserver die door RMS wordt gebruikt?](#bkmk_29)
-   [Wat is het effect van het gebruik in RMS van de globale catalogus voor groepsuitbreiding op de prestaties van de server met de globale catalogus?](#bkmk_30)
-   [Moeten er voor RMS wijzigingen in het schema van Active Directory worden aangebracht?](#bkmk_31)
-   [Wordt het serviceverbindingspunt automatisch gerepliceerd tussen de diverse domeincontrollers in het domein waar de RMS-cluster is geïnstalleerd?](#bkmk_32)
-   [Hoe kan de RMS-client worden geïnstalleerd en geconfigureerd als gebruikers geen beheerrechten op hun computers hebben?](#bkmk_33)
-   [Wat is de schaalbaarheid van RMS?](#bkmk_35)
-   [Kunnen in RMS hardwarebeveiligingsmodules worden gebruikt voor het beveiligen van RMS-sleutels in de hardware?](#bkmk_36)

<span id="BKMK_20"></span>
#### Is er enige afhankelijkheid met de versie van Exchange als de beveiligingsprincipals die voor RMS worden gebruikt, lid van de algemene adreslijst (GAL) zijn?

RMS is afhankelijk van Active Directory en niet van Exchange. In Exchange 5.5 wordt echter een eigen adreslijst en niet Active Directory gebruikt. Alle gebruikers en groepen in Active Directory moeten een geldig e-mailadreskenmerk hebben dat de volledig gekwalificeerde domeinnaam bevat. Dit gebeurt automatisch bij Exchange 2000 of hoger.

<span id="BKMK_21"></span>
#### Welke rol heeft SQL Server in RMS?

In RMS wordt een database gebruikt om alle configuratiegegevens van de services, informatie over principals in het systeem en alle logboekgegevens op te slaan en worden alle zoekopdrachten die in Active Directory en tijdens de uitbreiding van de distributielijst worden uitgevoerd, in de cache opgeslagen. RMS is volledig getest met SQL Server 2000 en SQL Server 2005.

<span id="BKMK_22"></span>
#### Moet de computer van een gebruiker aan hetzelfde domein als dat van de RMS-server worden toegevoegd om RMS te kunnen gebruiken?

De computer van de gebruiker hoeft geen lid te zijn van het domein waarvan de RMS-cluster lid is, maar de computer moet wel de RMS-cluster kunnen vinden. De gemakkelijkste manier voor clientcomputers om de RMS-cluster te vinden is via een zoekopdracht van Active Directory middels het serviceverbindingspunt. De RMS-cluster kan echter ook zonder een zoekopdracht van Active Directory worden opgezocht door registerinstellingen op de client in te stellen. Het ligt aan de toepassing met RMS-ondersteuning welke instellingen er in het register moeten worden ingesteld.

<span id="BKMK_23"></span>
#### Als een klant de RMS-server in een perimeternetwerk wil plaatsen, welke poorten in de firewall richting internet en de firewall richting het intranet moeten er zijn geopend om met RMS te kunnen communiceren?

De interne gebruikers moeten toegang hebben tot de RMS-servers die rechtenaccountcertificaten en gebruikslicenties uitgeven. De RMS-server luistert standaard op HTTP (TCP-poort 80) of HTTPS (TCP-poort 443), afhankelijk van het feit of de server voor het gebruik van SSL is ingesteld. Deze poorten moeten zijn geopend op de firewall richting internet. Hierbij zult u op de firewall richting internet extra poorten moeten openen die door lidservers in een domein worden gebruikt.

<span id="BKMK_24"></span>
#### Hoe worden onderliggende servers in een cluster exclusief voor licentieverlening ingeschreven en moet ik iets doen met de clients om die bewust te maken van deze cluster?

Wanneer in een bedrijf de eerste RMS-server in de basiscluster wordt gemaakt, ontvangt deze server een serverlicentieverleningscertificaat van de inschrijvingsservice van Microsoft. Wanneer een volgende RMS-server wordt geïnstalleerd en ingericht, kunt u die toevoegen aan de basiscluster of die als server inschrijven bij een onderliggende cluster exclusief voor licentieverlening. Als u besluit de server in te schrijven bij een onderliggende cluster exclusief voor licentieverlening, verzendt de server een inschrijvingsaanvraag naar de RMS-basiscluster. Toepassingen met RMS-ondersteuning geven aan waar een clienttoepassing moet zoeken naar de cluster exclusief voor licentieverlening. Office 2003 is een voorbeeld van een toepassing met RMS-ondersteuning die standaard contact maakt met de basiscluster. Dit gedrag kan worden omzeild via registerinstellingen, zodat de toepassing de nieuwe, onderliggende cluster exclusief voor licentieverlening opzoekt.

<span id="BKMK_25"></span>
#### Wat is het voordeel van het gebruik van een onderliggende cluster exclusief voor licentieverlening?

Het voordeel is, dat hiermee de afdelingen binnen een organisatie van elkaar kunnen worden gescheiden. Als er tussen RMS-clusters geen vertrouwd uitgiftedomein is ingesteld, kan de inhoud alleen worden gebruikt door gebruikers die toegang tot de licentieserver hebben. Op deze manier kan de juridische afdeling ervoor zorgen dat behalve de eigen medewerkers niemand anders door RMS gecodeerde e-mail kan lezen. Daarnaast kunnen er diverse opties worden ingesteld op de cluster exclusief voor licentieverlening, zoals sjablonen voor het rechtenbeleid, logboekregistratie, het lidmaatschap van de groep Supergebruikers en het uitsluitingsbeleid.

<span id="BKMK_26"></span>
#### Wat moet ik doen om een RMS-installatie helemaal ongedaan te maken?

Met de volgende procedure kunt u de installatie van RMS volledig ongedaan maken.

**De installatie van RMS ongedaan maken**
1.  Verwijder het serviceverbindingspunt voor de RMS-cluster via de beheerwebsite van RMS.

2.  Klik op **RMS van deze website verwijderen** op de pagina **Algemeen beheer** om de inrichting van RMS op de server ongedaan te maken. U moet eerst de inrichting van onderliggende ingeschreven licentieservers in clusters exclusief voor licentieverlening ongedaan maken en vervolgens de inrichting van de servers in de basiscluster ongedaan maken.

3.  Klik in het **Configuratiescherm** op **Software** en verwijder **Rights Management Services**.

4.  Verwijder de overige RMS-databases van de databaseserver.

5.  Verwijder de RMS-serviceaccount uit de lijst met geautoriseerde aanmeldingen van de databaseservers en verwijder vervolgens de account uit Active Directory.

6.  Als op de RMS-clients Windows XP of Windows 2000 wordt uitgevoerd, verwijdert u de RMS-client van de clientcomputers.

| ![](/security-updates/images/Cc720274.Important(WS.10).gif)Belangrijk                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u dit hebt gedaan, kunt u niet langer met rechten beveiligde inhoud openen. Als RMS wordt gebruikt voor het beveiligen van gegevens, moet u eerst RMS uit bedrijf nemen voordat u een RMS-installatie ongedaan gaat maken. |

<span id="BKMK_27"></span>
#### Moet ik nog bestanden verwijderen als ik via Software in het Configuratiescherm de installatie van RMS ongedaan heb gemaakt?

U kunt de lockbox uit %systemroot%\\system32 verwijderen, maar dit is niet strikt noodzakelijk.

<span id="BKMK_28"></span>
#### Werkt RMS in het FAT-bestandssysteem?

Ja, RMS werkt op een computer met het FAT-bestandssysteem, maar u wordt aangeraden het NTFS-bestandssysteem te gebruiken.

<span id="BKMK_29"></span>
#### Welke hardwareconfiguratie is het beste voor de databaseserver die door RMS wordt gebruikt?

De logboekdatabase wordt snel groter, vooral in omgevingen waar RMS veelvuldig wordt gebruikt. Als u van plan bent SQL Server als databaseserver te gebruiken, is de beste keuze SQL Server 2000 Enterprise Edition of SQL Server 2005 Enterprise Edition op Windows 2000 Advanced Server of Windows Server 2003, Enterprise Edition, geconfigureerd in een cluster in een actieve/stand-by configuratie. In dat geval is de aanbevolen configuratie RAID-1-logboekschijven en RAID-5-gegevensschijven met minstens 512 MB RAM. De minimum aanbevolen CPU voor deze configuratie is een Pentium III van 1,4 GHz. Op toegewijde databaseservers is één CPU voldoende.

<span id="BKMK_30"></span>
#### Wat is het effect van het gebruik in RMS van de globale catalogus voor groepsuitbreiding op de prestaties van de server met de globale catalogus?

Op de RMS-server worden de groepsuitbreidingslijsten opgeslagen, waardoor de server met de globale catalogus wordt ontlast. Door het groepslidmaatschap regelmatig bij te werken wordt de server met de globale catalogus betrouwbaarder. De time-out voor het aanvragen van nieuwe groepsoverzichten kan in het register worden ingesteld. Het veelvuldig uitbreiden van grote groepen heeft een nadelig effect op de prestaties. Zie voor meer informatie "Cache-instellingen wijzigen van Active Directory Cache" in "RMS: Operations" in deze documentatie.

<span id="BKMK_31"></span>
#### Moeten er voor RMS wijzigingen in het schema van Active Directory worden aangebracht?

In RMS kan het groepslidmaatschap dat in de uitgiftelicentie is opgegeven, alleen naar andere forests worden uitgebreid als in het lokale Active Directory-forest een contactobject is opgenomen dat de groep in het externe forest vertegenwoordigt. In RMS kan naar de kenmerken van het contactobject worden gezocht en worden ontdekt dat dit object een groep uit een ander forest vertegenwoordigt.

Hiervoor is voor Active Directory het schemakenmerk msExchOriginatingForest van Exchange Server 2003 of hoger nodig. Dit kenmerk wordt standaard in het Active Directory-schema geïnstalleerd als er in het forest één server met Exchange Server 2003 is. Dit kenmerk moet aanwezig zijn in het forest van elk Active Directory-schema dat wordt gebruikt in RMS. Als u Exchange Server 2003 niet gebruikt, kunt u het schema apart installeren in de Active Directory-structuur met de RMS Administration Toolkit.

<span id="BKMK_32"></span>
#### Wordt het serviceverbindingspunt automatisch gerepliceerd tussen de diverse domeincontrollers in het domein waar de RMS-server is geïnstalleerd?

Nadat de eerste RMS-server in een forest is ingericht, moet deze server in Active Directory worden geregistreerd met behulp van een domeinaccount. Deze account moet voldoende rechten voor het maken van een containerobject onder de Services-container in de Configuratie-container in Active Directory hebben. De ingebouwde beveiligingsgroep Ondernemingsadministrators is een voorbeeld van een account met de vereiste rechten. Het serviceverbindingspunt wordt gemaakt. Omdat dit punt zich in de Services-container bevindt, repliceert Active Directory de gegevens naar alle domeincontrollers in het forest.

<span id="BKMK_33"></span>
#### Hoe kan de RMS-client worden geïnstalleerd en geconfigureerd als gebruikers geen beheerrechten op hun computers hebben?

De RMS-client is een Windows Installer-bestand dat kan worden verspreid door middel van een systeem voor het verspreiden van software, zoals Systems Management Server 2003. De RMS-client kan ook worden verspreid met behulp van een groepsbeleidsobject waarbij een serviceaccount met beheerrechten wordt gebruikt. Als op de RMS-client Windows Vista wordt uitgevoerd, is een afzonderlijke installatie van een RMS-client niet langer nodig omdat die is geïntegreerd in het besturingssysteem.

<span id="BKMK_35"></span>
#### Wat is de schaalbaarheid van RMS?

RMS is een webservice zonder status. Deze service kan net als elke andere website of webservice in een cluster worden geplaatst en de taakverdeling kan ervoor worden ingesteld. De prestaties van RMS hangen voor het overgrote deel af van de beschikbaarheid van de processor en kunnen worden verbeterd door extra processors toe te voegen.

<span id="BKMK_36"></span>
#### Kunnen in RMS hardwarebeveiligingsmodules worden gebruikt voor het beveiligen van RMS-sleutels in de hardware?

Ja, RMS werkt met CAPI compatibele hardwarebeveiligingsmodules, zoals die van nCipher.
