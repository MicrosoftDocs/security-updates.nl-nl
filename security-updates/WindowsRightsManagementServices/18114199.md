---
TOCTitle: Inschrijving van de basiscertificeringsserver
Title: Inschrijving van de basiscertificeringsserver
ms:assetid: 'f08bc919-f090-4843-b2ce-b40d558012ce'
ms:contentKeyID: 18114199
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747734(v=WS.10)'
---

Inschrijving van de basiscertificeringsserver
=============================================

Inschrijving met de inschrijvingsservice van Microsoft is vereist voor de eerste server in een RMS-implementatie. Deze server, de basiscertificeringsserver, kan tijdens de inrichting automatisch worden ingeschreven als de server een internetverbinding heeft. Als de server in een gesloten netwerk staat, kan de server handmatig worden ingeschreven. Zie 'Handmatig een basiscertificeringsserver inschrijven' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over het handmatig inschrijven van servers.

De aanvraag voor inschrijving moet de volgende invoerparameters bevatten:

-   Een openbare sleutel van 1024 bits. Deze openbare sleutel is de openbare sleutel van RMS.
-   De versie, naam en URL van de RMS-server die moet worden ingeschreven.

In de inschrijvingsservice van Microsoft worden deze gegevens uitsluitend gebruikt voor het maken van het serverlicentiecertificaat en uitsluitend opgeslagen voor intrekkingsdoeleinden.

De inschrijvingsservice van Microsoft stuurt een certificaatketen terug waarin de licentiecertificaatketen van de inschrijvingsserver en een door de inschrijvingsserver ondertekend certificaat zijn opgenomen. Het certificaat bevat de openbare sleutel van de server die is ondertekend met de persoonlijke sleutel voor de inschrijving en de versie en URL van de ingeschreven server. Met dit certificaat wordt aan de basiscertificeringsserver het recht verleend serverlicentieverleningscertificaten uit te geven aan licentieservers. Daarnaast kunnen hiermee rechtenaccountcertificaten, clientlicentiecertificaten, uitgiftelicenties en gebruikslicenties worden uitgegeven.

Het serverlicentiecertificaat is geldig voor één jaar. Het certificaat is geldig vanaf het moment dat het wordt uitgegeven. De geldigheid van het certificaat kan worden verlengd. Certificaten en licenties die door de server worden uitgegeven, zijn zeven jaar geldig. Deze certificaten en licenties zijn geldig vanaf het moment dat ze worden uitgegeven.

Wanneer er informatie over de intrekking van het certificaat is opgegeven in de inschrijvingsaanvraag, wordt deze toegevoegd aan het serverlicentiecertificaat. De openbare sleutel van de intrekkingsservice van Microsoft wordt als een intrekkingssleutel toegevoegd aan het certificaat. Als een intrekkingssleutel van derden wordt opgegeven, wordt deze eveneens toegevoegd als een intrekkingssleutel.
