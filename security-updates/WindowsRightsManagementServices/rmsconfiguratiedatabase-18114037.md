---
TOCTitle: 'RMS-configuratiedatabase'
Title: 'RMS-configuratiedatabase'
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18114037
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747634(v=WS.10)'
---

RMS-configuratiedatabase
========================

Voor het opslaan van de configuratie- en beleidsgegevens van RMS wordt een databaseserver gebruikt, zoals Microsoft® SQL Server of Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) versie A. Er is één configuratiedatabase beschikbaar voor elke RMS-server of elk RMS-cluster. Deze database wordt gebruikt voor het opslaan, delen en ophalen van configuratiegegevens en andere gegevens.

De configuratiedatabase voor een basiscertificeringsserver of -cluster bevat een lijst met Windows-gebruikersidentiteiten en bijbehorende rechtenaccountcertificaten. Voordat het sleutelpaar van een certificaat in de database wordt opgeslagen, wordt het sleutelpaar gecodeerd als de openbare sleutel van de RMS-server. Configuratiedatabases voor licentieservers bevatten deze gegevens niet.

Aan de RMS-servicegroep zijn uitvoeringsmachtigingen toegewezen voor de opgeslagen procedures in de database.

**Belangrijk** Het wordt aangeraden MSDE 2000 alleen in testomgevingen te gebruiken ter ondersteuning van RMS-databases omdat MSDE 2000 geen ondersteuning biedt voor netwerkinterfaces. Bovendien bepalen de voorwaarden voor het gebruik van MSDE 2000 dat u geen SQL Server-clienthulpprogramma's mag gebruiken om MSDE 2000-databases te bewerken. Door deze beperking kunt u geen logboekgegevens weergeven of opgeslagen gegevens in de configuratiedatabase wijzigen.
