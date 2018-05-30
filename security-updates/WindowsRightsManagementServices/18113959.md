---
TOCTitle: De grootte van het logboekbestand beheren
Title: De grootte van het logboekbestand beheren
ms:assetid: '431b32b3-02f0-4666-b52c-183eb65154fd'
ms:contentKeyID: 18113959
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720271(v=WS.10)'
---

De grootte van het logboekbestand beheren
=========================================

Door de logboekregistratieservice worden grote hoeveelheden gegevens naar de SQL Server-database verstuurd. Controleer de logboekdatabase regelmatig om er zeker van te zijn dat er voldoende schijfcapaciteit aanwezig is voor de gegevens. Als er te veel en overbodige gegevens worden opgenomen in de logboekdatabase, kunt u SQL Server-filters dusdanig instellen dat alleen de benodigde gegevens worden vastgelegd. Raadpleeg de Help van SQL Server Enterprise Manager voor instructies voor het filteren van logboekregistratiegegevens.

Als er te weinig beschikbare schijfruimte aanwezig is voor de logboekdatabase, kunt u deze verplaatsen naar een andere server, zoals wordt beschreven in '[De logboekdatabase verplaatsen](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)' verderop in dit onderwerp.

| ![](/security-updates/images/Cc720271.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Met Systeemmonitor moet u regelmatig de grootte van de wachtrij voor uitgaande logboekregistratieberichten controleren. Als de grootte van de wachtrij aanzienlijk toeneemt, controleert u of de service van de logboekregistratie-listener correct werkt. Raadpleeg Help en ondersteuning van Windows Server 2003 voor meer informatie over het gebruik van Systeemmonitor. |
