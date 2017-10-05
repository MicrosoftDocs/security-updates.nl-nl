---
TOCTitle: 'De webservice verwijderen (de inrichting van RMS ongedaan maken)'
Title: 'De webservice verwijderen (de inrichting van RMS ongedaan maken)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18114164
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747602(v=WS.10)'
---

De webservice verwijderen (de inrichting van RMS ongedaan maken)
================================================================

Nadat de inrichting van de RMS-server ongedaan is gemaakt en alle RMS-beveiliging is verwijderd, kan de webservice als volgt worden verwijderd:

-   Klik op de pagina **Algemeen beheer** op **RMS van deze website verwijderen**.

De volgende stap hangt af van het type server dat wordt verwijderd, alhoewel in alle gevallen RMS uit IIS wordt verwijderd.

-   Als de server onderdeel is van een cluster (maar niet de laatste server in het cluster), hoeven er geen extra stappen te worden uitgevoerd.
-   Is de server alleen een licentieserver, dan verwijdert u de database met adreslijstservices maar niet de configuratiedatabase en de registratiedatabase (deze worden door de certificeringsserver gebruikt die nog in bedrijf is).
-   Als de server de laatste RMS-server binnen de organisatie is, verwijdert u niet de configuratiedatabase en de registratiedatabase maar wel het serviceverbindingspunt in Active Directory.
