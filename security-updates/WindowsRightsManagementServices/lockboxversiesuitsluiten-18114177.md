---
TOCTitle: 'Lockbox-versies uitsluiten'
Title: 'Lockbox-versies uitsluiten'
ms:assetid: 'e287f026-aab2-43ab-93bc-48087da82f36'
ms:contentKeyID: 18114177
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747700(v=WS.10)'
---

Lockbox-versies uitsluiten
==========================

U kunt zorgen dat clients een bepaalde minimumversie van de RMS-clientsoftware gebruiken door de lockbox-versie van de client te gebruiken om eerdere versies van de RMS-clientsoftware uit te sluiten. Als u deze functie inschakelt, geeft u op welke minimumversie van de lockbox is ondertekend via de activeringsservice van Microsoft. Vervolgens schakelt u lockbox-uitsluiting in op de beheerwebsite van elk cluster waarvoor de uitsluiting moet gelden. Alle certificerings- en licentieaanvragen worden gecontroleerd. Zodoende weet u zeker dat de lockbox voldoet aan het criterium van de minimumversie.

Als u uitsluiting op basis van de lockbox-versie hebt ingeschakeld, kunnen met clients met een eerdere versie dan de opgegeven minimumversie van de lockbox geen rechtenaccountcertificaten of gebruikslicenties worden opgehaald, omdat aanvragen van deze clients worden geweigerd. Deze clients dienen een nieuwe versie van de RMS-clientsoftware te installeren om een nieuwe lockbox te krijgen met de huidige versie van de software.

De RMS-client voor Service Pack 1 (SP1) gebruikt een lockbox-versie die hoger dan of gelijk aan 5.0.0.0 is. Door de lockbox-uitsluiting op die minimumversie in te stellen, verplicht u de RMS-clients in uw organisatie om te upgraden naar de RMS-client voor SP1 als ze door RMS beveiligde inhoud willen gebruiken.

Als aan een gebruiker met een uitgesloten lockbox eerder licenties voor inhoud zijn uitgegeven, kan de gebruiker met deze inhoud blijven werken zonder een nieuwe lockbox.
