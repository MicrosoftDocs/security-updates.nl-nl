---
TOCTitle: De infrastructuur van de databaseserver plannen
Title: De infrastructuur van de databaseserver plannen
ms:assetid: 'b12354bd-3143-4d1f-b5aa-450c4550653c'
ms:contentKeyID: 18114149
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747731(v=WS.10)'
---

De infrastructuur van de databaseserver plannen
===============================================

Omdat RMS bij bewerkingen databases en opgeslagen procedures gebruikt, is er een database-infrastructuur nodig om RMS in uw organisatie te kunnen gebruiken. Uw databaseserver kan op dezelfde server als RMS of op een andere server staan. Als er binnen uw infrastructuur geen databaseserver voor ondersteuning van RMS is, kunt u om RMS te testen Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) versie A gebruiken als databaseserver.

U wordt aangeraden Microsoft SQL Server Desktop Engine alleen in testomgevingen te gebruiken voor ondersteuning van RMS-databases, omdat Microsoft SQL Server Desktop Engine niet over de noodzakelijke hulpprogramma's beschikt om een database in het gehele bedrijf te kunnen uitvoeren en ondersteunen. Aangezien MSDE externe netwerken niet ondersteunt, moet u MSDE op dezelfde server als RMS installeren en kunt u geen extra RMS-servers aan het RMS-cluster toevoegen. In de gebruiksvoorwaarden voor Microsoft SQL Server Desktop Engine wordt aangegeven dat u hulpprogramma's voor SQL Server-clients niet kunt gebruiken voor het bewerken van een Microsoft SQL Server Desktop Engine-database. Door deze beperking kunt u geen back-up maken van de RMS-configuratiedatabase en deze herstellen en geen logboekgegevens weergeven of gegevens wijzigen die in de configuratiedatabase zijn opgeslagen.

Als u van plan bent de databases op een andere server onder te brengen dan de RMS-installatie, hebt u een compleet databaseserverproduct zoals SQL Server nodig ter ondersteuning van de databases. Zorg dat de RMS-serviceaccount over voldoende machtigingen beschikt voor het lezen, schrijven en maken van databases op de databaseserver die voor de ondersteuning van RMS wordt gebruikt.

RMS is ontworpen voor en getest met databaseservers waarop SQL Server 2000 en MSDE wordt uitgevoerd. Microsoft ondersteunt het gebruik van RMS in combinatie met een andere databaseprovider dan SQL Server 2000 of MSDE niet. Toch kan RMS worden uitgevoerd op andere databaseservers waarop ADO.NET-interfaces worden uitgevoerd die zijn verstrekt door Microsoft .NET Framework. Daarom is het mogelijk dat andere leveranciers databases hebben ontwikkeld die compatibel zijn met RMS. Elke willekeurige databaseprovider kan in combinatie met RMS worden gebruikt, mits de bijbehorende databaseserver aan de volgende criteria voldoet:

-   De databaseserver moet voldoen aan de eisen van Transact-SQL omdat initialisatiescripts en opgeslagen procedures van RMS gebruikmaken van Transact-SQL.
-   De databaseserver moet voor Microsoft SQL Server specifieke extensies ondersteunen.

De databaseprovider moet kunnen:

-   Reageren op methodeaanroepen van de System.Data.SqlClient-naamruimte van .NET Framework.
-   De bijbehorende functionaliteit van de System.Data.SqlClient-naamruimte verstrekken.
-   Geïntegreerde Windows-verificatie gebruiken in plaats van SQL-verificatie.

Gebruikt u RMS in een andere configuratie, neem dan contact op met de relevante databaseleverancier of het bedrijf waarvan u de databaseprovider gebruikt in uw aangepaste implementatie.

| ![](/security-updates/images/Cc747731.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS-databases worden standaard gemaakt met Volledig herstel ingeschakeld, maar er worden geen back-uptaken voor het transactielogboek gemaakt. Hierdoor kan de vaste schijf van de server vol raken, waardoor er zich een fout op de databaseserver kan voordoen. Volledig herstel wordt aangeraden voor de database DRMS\_configuration. De andere DRMS-databases kunnen worden ingesteld voor een ander herstelmodel dat is afgestemd op de situatie binnen uw organisatie. |

Dit gedeelte bevat de volgende onderwerpen:

-   [De grootte van de database inschatten](https://technet.microsoft.com/87652cc2-b886-4797-8d40-356669768089)
-   [De database met directoryservices onderhouden](https://technet.microsoft.com/911a62f2-c1d6-4091-99b0-b53211be27a7)
-   [De logboekdatabase onderhouden](https://technet.microsoft.com/de55058b-0d1a-4997-8a45-e14678ddd13f)
