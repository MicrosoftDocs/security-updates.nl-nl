---
TOCTitle: RMS uit bedrijf nemen
Title: RMS uit bedrijf nemen
ms:assetid: 'dbcacce7-434d-48a7-a11d-ef9690d78b44'
ms:contentKeyID: 18114211
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747767(v=WS.10)'
---

RMS uit bedrijf nemen
=====================

Het uit bedrijf nemen van een RMS-server is het verwijderen van de server en de bijbehorende databases uit het computersysteem van een organisatie. Met dit proces kunt u RMS uit de infrastructuur verwijderen zonder dat u daarbij de toegang tot door RMS beveiligde gegevens verliest. Hieronder staan enkele redenen om een RMS-server uit de infrastructuur te verwijderen:

-   Migratie van een geteste RMS-server van een testomgeving naar de productieomgeving.
-   Vereenvoudiging van het architectuurontwerp door licentieservers te verwijderen en in het basiscluster van RMS te consolideren.
-   Samenvoegen van RMS-servers (bijvoorbeeld als gevolg van een fusie of acquisitie) door twee RMS-infrastructuren in één infrastructuur te integreren.
-   Het besluit om inhoud niet meer met RMS te beveiligen.

Omdat een actieve RMS-server wordt geïntegreerd met zowel een databaseserver als Active Directory en omdat er dan inhoud is die is beveiligd met een sleutel van de RMS-server, is het verwijderen van RMS uit de organisatie meer dan alleen het verwijderen van het programma van de server. In deze sectie worden de benodigde stappen uitgelegd, waarmee u indien nodig uw RMS-server uit bedrijf kunt nemen.

Dit gedeelte bevat de volgende onderwerpen:

-   [Uitleg over het uit bedrijf nemen](https://technet.microsoft.com/57bd9949-9433-437b-93ed-ffb2dff9992e)
-   [De service Uit bedrijf nemen inschakelen](https://technet.microsoft.com/45226e85-b50d-41cc-aca7-0f603f8509d5)
-   [Machtigingen voor virtuele mappen instellen](https://technet.microsoft.com/45112111-9608-45b1-9a86-7b313d0a1579)
-   [RMS-beveiliging van inhoud verwijderen](https://technet.microsoft.com/c30361e3-50d2-4474-a87d-d38de502cf9e)
-   [De webservice verwijderen (de inrichting van RMS ongedaan maken)](https://technet.microsoft.com/68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e)
-   [RMS-programmabestanden verwijderen](https://technet.microsoft.com/d1dc8a8b-f8de-487f-87b4-2174d449f0bc)
-   [Alternatieven voor het uit bedrijf nemen van RMS](https://technet.microsoft.com/4d32f35e-997d-4d10-ab66-efe217e853f7)
