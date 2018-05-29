---
TOCTitle: Snelimplementatiegids
Title: Snelimplementatiegids
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18114153
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747735(v=WS.10)'
---

Snelimplementatiegids
=====================

Deze gids is bedoeld om u te helpen bij het snel opzetten van een RMS-server met Service Pack 1, zodat u dit product kunt evalueren en kunt beslissen of u een brede implementatie in uw organisatie wilt doorvoeren.

**Stap 1 - Voorbereiden op RMS**

RMS steunt op andere onderdelen die u moet installeren en configureren voordat u de service kunt gebruiken. Als u de volgende stappen hebt voltooid, voldoet uw infrastructuur aan de basisvereisten voor RMS:

1.  Configureer een computer waarop Windows Server 2003 wordt uitgevoerd en voeg die vervolgens toe aan een Active Directory-domein. (Bij kleinere organisaties die over slechts één server beschikken, kan dit de domeincontroller voor Active Directory zijn. In dat geval moet Windows Server 2003, Standard Edition, Windows Server 2003, Enterprise Edition of Windows Server 2003, Datacenter Edition op de computer worden uitgevoerd. Een computer waarop Windows Server 2003, Web Edition, wordt uitgevoerd kan geen domeincontroller zijn.)
2.  Configureer de server voor de rol van **toepassingsserver**. Klik hiervoor op **Start** en dubbelklik achtereenvolgens op **Configuratiescherm** en het pictogram **Software**. Klik in **Software** op **Windows-onderdelen toevoegen of verwijderen** en zorg dat onder **Toepassingsserver** de volgende services zijn ingeschakeld:
    -   **ASP.NET**
    -   **Internet Information Services (IIS)**
    -   **Message Queuing**

    Accepteer bij elk van de services de standaardopties. Verdere configuratie is niet nodig.
3.  Configureer een databaseserver door een van de volgende databasetoepassingen te gebruiken:
    -   Microsoft® SQL Server 2000 met SP3a. Dit mag een lokale installatie van SQL Server 2000 zijn of een installatie op afstand die zich in hetzelfde domein bevindt.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A. Dit dient een lokale installatie te zijn. U kunt MSDE 2000 downloaden vanaf de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=17799%20(http://www.microsoft.com/)).

    U wordt aangeraden Microsoft SQL Server Desktop Engine alleen in testomgevingen te gebruiken voor ondersteuning van RMS-databases, omdat Microsoft SQL Server Desktop Engine niet over de noodzakelijke hulpprogramma's beschikt om een database in het gehele bedrijf te kunnen uitvoeren en ondersteunen. Aangezien MSDE externe netwerken niet ondersteunt, moet u MSDE op dezelfde server als RMS installeren en kunt u geen extra RMS-servers aan het RMS-cluster toevoegen. In de gebruiksvoorwaarden voor Microsoft SQL Server Desktop Engine wordt aangegeven dat u hulpprogramma's voor SQL Server-clients niet kunt gebruiken voor het bewerken van een Microsoft SQL Server Desktop Engine-database. Door deze beperking kunt u geen back-up maken van de RMS-configuratiedatabase en deze herstellen en geen logboekgegevens weergeven of gegevens wijzigen die in de configuratiedatabase zijn opgeslagen.
4.  Bepaal de naam van de service zodat gebruikers via het intranet verbinding kunnen maken (bijvoorbeeld http://certificering.contoso.com). Configureer het DNS (Domain Name System) zodat die URL wordt herleid naar het IP-adres van de RMS-computer. U moet een volledig gekwalificeerde DNS-domeinnaam voor de URL van het cluster gebruiken, zodat servers in andere DNS-zones het IP-adres van de RMS-servers of de servers kan herleiden.
5.  Maak een beheerdersaccount voor gebruik met RMS.
6.  U bent nu gereed om RMS SP1 te installeren. Zie 'RMS met Service Pack 1 installeren' in 'Een RMS-server beheren' in deze documentatie voor verdere instructies over deze stap.

**Veel gebruikte optionele functies**

De volgende functies zijn optioneel. Als u ze wilt gebruiken, moet u eerst de noodzakelijke voorbereidingen treffen voordat u RMS gaat installeren en inrichten:

-   U kunt RMS configureren voor het gebruik van een hardwarebeveiligingsmodule voor het opslaan van persoonlijke sleutels. Als u een hardwarebeveiligingsmodule wilt gebruiken, controleert u of de stuurprogramma's juist zijn geconfigureerd en of de beveiligingsomgeving is gedefinieerd.
-   U kunt tijdens het inrichtingsproces automatisch een serverlicentieverleningscertificaat downloaden als uw RMS-computer verbinding met internet heeft. Als uw organisatie via een proxyserver verbinding maakt met internet, controleert u de proxyinstellingen in Internet Explorer, inclusief eventuele verificatievereisten, en noteert u die voor later gebruik.
-   Als u RMS uitvoert op een domeincontroller en u een gebruikersaccount wilt gebruiken voor het uitvoeren van de RMS-services, moet u het Beveiligingsbeleid voor domeincontroller zo configureren dat de gebruikersaccount toestemming heeft voor lokaal aanmelden. Zie Windows Server 2003 Help en ondersteuning voor meer informatie over hoe u het beveiligingsbeleid voor domeincontrollers configureert.

**Stap 2 - De eerste RMS-server inrichten**

Het inrichten bestaat uit het configureren van een website voor RMS, zodat gebruikers de service kunnen gebruiken. Voer de volgende stappen uit om de basiscertificeringsserver voor uw organisatie in te richten:

1.  Meld u bij de computer aan als domeingebruiker met lokale beheerdersbevoegdheden. Als u RMS op een domeincontroller installeert, meldt u zich aan als domeinbeheerder.
2.  Klik op **Start**, wijs **Alle programma's** en **Windows RMS** aan en klik op **Windows RMS-beheer** om de pagina **Algemeen beheer** te openen. Deze pagina bevat een lijst met websites die op de server beschikbaar zijn.
3.  Klik op de website die u wilt inrichten met RMS en klik vervolgens op **RMS op deze website inrichten**. Boven aan de pagina die wordt geopend, wordt de tekst **De RMS-basiscertificeringsserver inrichten** weergegeven.
4.  Geef de informatie op voor uw organisatie.
    -   Typ in het vak **Cluster-URL** de naam van de service (bijvoorbeeld certificering.contoso.com) die u in stap 4 van de vorige procedure hebt geconfigureerd. Als u SSL met uw installatie wilt gebruiken, klikt u in de lijst met protocollen op het protocol HTTPS. In dat geval wordt SSL ingeschakeld. Dit betekent echter niet dat SSL vereist is voor RMS-webservices. Dat moet u afzonderlijk configureren via IIS.
    -   Als de server via een proxyserver met internet is verbonden, vult u in het gebied **RMS-proxyinstellingen** het gedeelte in met de informatie uit Internet Explorer, zoals wordt beschreven in het gedeelte over de optionele functies van de vorige procedure.
    -   In het gedeelte over **serverconnectiviteit met internet** dient u **On line** te selecteren als u wilt dat de server via internet verbinding met de inschrijvingsservice van Microsoft maakt om tijdens het inrichtproces automatisch een serverlicentieverleningscertificaat op te halen. Selecteer **Off line** als u handmatig verbinding met de inschrijvingsservice van Microsoft wilt maken, het serverlicentieverleniningscertificaat wilt downloaden en dit na inrichting in RMS wilt importeren.
5.  Klik op **Verzenden**.
    Het duurt ongeveer 60 tot 90 seconden voordat het inrichten is voltooid. U kunt dan terugkeren naar de pagina **Algemeen beheer**, waar u de zojuist ingerichte website kunt beheren.
6.  Ga naar de pagina **Algemeen beheer** en selecteer **RMS op deze website beheren** om de introductiepagina van de **beheerwebsite** voor de RMS-server te openen.
    Als u in stap 4 Off line hebt geselecteerd voor serverconnectiviteit met internet, dient u de procedure 'Handmatig een basiscertificeringsserver inschrijven' te voltooien alvorens door te gaan.
7.  Klik op de introductiepagina van de beheerwebsite op de koppeling **Serviceverbindingspunt voor RMS**.

| ![](/security-updates/images/Cc747735.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bij de volgende stap van deze procedure, het registreren van een serviceverbindingspunt, moet een domeinaccount met voldoende rechten worden gebruikt om een containerobject te maken onder de servicescontainer in de configuratiecontainer van het Active Directory-forest. De vooraf gedefinieerde beveiligingsgroep, **Ondernemingsadministrators**, is een voorbeeld van een account met de vereiste rechten. |

1.  Klik op de pagina **Serviceverbindingspunt voor RMS** op de knop **URL registreren**. Hiermee wordt het serviceverbindingspunt van RMS in Active Directory geregistreerd zodat met RMS compatibele toepassingen RMS-licentieservices, activeringsproxyservices en certificeringsservices kunnen opsporen.

**Stap 3 - RMS testen**

Voordat u RMS volledig kunt gebruiken, moet u de Microsoft Windows Rights Management-client en een toepassing met RMS-ondersteuning op de clientcomputers installeren. De gebruikers moeten lid zijn van het Active Directory-domein en de clientcomputers moeten aan het domein zijn toegevoegd. Bovendien moeten de gebruikers over e-mailadressen beschikken die zijn gedefinieerd in Active Directory. RMS testen:

1.  Meld u aan bij de clientcomputer als een geldige domeingebruiker.
2.  Installeer de RMS-client voor Service Pack 1.
3.  Installeer een toepassing met RMS-ondersteuning.
4.  Maak een door RMS beveiligd bestand, geef iedereen voor dat bestand rechten voor Alleen-lezen en sla het bestand vervolgens op in een gedeelde map met volledige toegang voor gebruikers.
5.  Meld u als andere gebruiker bij de computer aan. Open het bestand en probeer wijzigingen aan te brengen. Als RMS goed is geïnstalleerd, kunt u het bestand niet wijzigen.
