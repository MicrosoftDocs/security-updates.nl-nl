---
TOCTitle: 'Uw RMS-topologie bepalen'
Title: 'Uw RMS-topologie bepalen'
ms:assetid: 'bf516f7d-b3a1-4e7f-971f-bfab1db41812'
ms:contentKeyID: 18114120
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747651(v=WS.10)'
---

Uw RMS-topologie bepalen
========================

In de basistopologie voor RMS verschaft de basiscertificeringsserver of het basiscertificeringscluster van RMS in elk Active Directory-forest alle RMS-services voor een organisatie. Deze RMS-topologie werkt goed zowel in grote als in kleine organisaties. In een gedistribueerde RMS-topologie kunnen een of meer licentieservers (soms afdelingslicentieservers genoemd) enkele of alle licentieservices bieden aan bepaalde gebruikers en groepen binnen de organisatie. Hoewel de basiscertificeringsserver (of -cluster) de accountcertificering en de activeringproxyservices voor de gehele organisatie blijft verzorgen, is deze gedistribueerde RMS-topologie ontworpen voor organisaties die zeer specifieke icentiebehoeften hebben en het beheer van RMS binnen een bepaald segment van de organisatie willen houden.

Hoewel er slechts twee basistopologieën bestaan voor RMS, kunnen de onderdelen van de topologieën sterk verschillen. U definieert de onderdelen die geschikt zijn voor uw organisatie, en creëert de juiste topologie voor de implementatie van RMS als volgt:

-   Evalueer de vereisten en doelstellingen van de organisatie.
-   Definieer hoe rechtenbeheer (rights management) moet worden gebruikt
-   Analyseer de geprojecteerde verkeerspatronen en -belastingen voor het implementeren van een passend serviceniveau.

Het definiëren van de topologie en het nemen van beslissingen die nodig zijn om uw ontwerp te implementeren, is een iteratief proces dat in de implementatie van RMS doorgaat.

In dit onderwerp wordt het volgende besproken:

-   [Kernonderdelen identificeren](https://technet.microsoft.com/c9ec225b-0e51-42f5-aff6-0aecb62e3b27)
-   [Topologiedoelen vaststellen](https://technet.microsoft.com/8275a04d-3e5b-40b0-be9d-2f31b7aeca6b)
-   [De omvang van de RMS-implementatie plannen](https://technet.microsoft.com/4b5fe1be-643e-47c4-bf9b-50d1e97108fb)
-   [Schaalbaarheidsvereisten evalueren](https://technet.microsoft.com/89f0138c-946d-47d7-a286-041d4d9606a8)
-   [Redundantie en taakverdeling verzorgen](https://technet.microsoft.com/162d547c-78a7-4848-b43e-58e481832af2)
-   [Migratievereisten evalueren](https://technet.microsoft.com/cec07f45-dc52-4004-860b-5cc33e5fc209)
-   [De infrastructuur van de databaseserver plannen](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
-   [Implementatie naar verschillende forests plannen](https://technet.microsoft.com/2dfb40b7-95b1-4362-b32e-72867544b705)
-   [Plannen voor externe RMS-gebruikers](https://technet.microsoft.com/107e1338-4dcf-4ed5-a49d-e875cc883db1)
-   [Een RMS-basistopologie plannen](https://technet.microsoft.com/fec3201e-201f-4faf-910e-fa44132af83d)
-   [Een gedistribueerde RMS-topologie plannen](https://technet.microsoft.com/8773a1e0-6ac3-41f5-9866-5890cef08d04)
