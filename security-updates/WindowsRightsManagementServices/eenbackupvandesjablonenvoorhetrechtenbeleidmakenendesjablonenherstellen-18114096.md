---
TOCTitle: 'Een back-up van de sjablonen voor het rechtenbeleid maken en de sjablonen herstellen'
Title: 'Een back-up van de sjablonen voor het rechtenbeleid maken en de sjablonen herstellen'
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18114096
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747625(v=WS.10)'
---

Een back-up van de sjablonen voor het rechtenbeleid maken en de sjablonen herstellen
====================================================================================

Maak regelmatig een back-up van de sjabloongegevens in de configuratiedatabase en sla deze op een veilige plaats op om de waardevolle sjablonen voor het rechtenbeleid te beveiligen. Als er een systeemfout optreedt, kunt u de sjablonen voor het rechtenbeleid herstellen met de back-up.

Voer een van de volgende handelingen uit:

-   Maak een back-up van de hele configuratiedatabase waarin de sjabloongegevens voor het rechtenbeleid zijn opgenomen. Raadpleeg de documentatie voor SQL Server voor meer informatie over het maken van een back-up van een SQL Server-database.
    - of -
-   Maak alleen een back-up van de sjabloongegevens voor het rechtenbeleid. U kunt dit doen door de GUID- en TemplateData-gegevens vanuit de tabel DRMS\_RightsTemplate in de configuratiedatabase naar een nieuw tekstbestand te exporteren. Raadpleeg de documentatie van SQL Server voor meer informatie over het exporteren van gegevens vanuit een SQL Server-database.

Als u de sjabloongegevens voor het rechtenbeleid in de configuratiedatabase moet herstellen, kunt u de GUID- en TemplateData-gegevens ophalen uit de tabel DRMS\_RightsTemplate in de back-up van de configuratiedatabase. Als u alleen een back-up van de sjabloongegevens hebt gemaakt, hoeft u alleen maar de gegevens uit het tekstbestand te importeren. Raadpleeg de documentatie voor SQL Server voor meer informatie over het uitvoeren van deze taken.

| ![](/security-updates/images/Cc747625.note(WS.10).gif)Opmerking                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------|
| Raadpleeg uw SQL Server-beheerder als u een plan wilt opstellen voor het maken van back-ups van sjablonen voor het rechtenbeleid. |
