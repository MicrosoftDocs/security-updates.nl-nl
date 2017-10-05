---
TOCTitle: 'RMS-logboekdatabase'
Title: 'RMS-logboekdatabase'
ms:assetid: '8ba147f3-16e4-4d9a-ac8f-f05ba2ba11bb'
ms:contentKeyID: 18114072
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747669(v=WS.10)'
---

RMS-logboekdatabase
===================

In het installatieprogramma van RMS wordt voor alle basiscertificeringsservers en -clusters een logboekdatabase geïnstalleerd in dezelfde versie van de databaseserver waarin de configuratiedatabase is opgenomen. Daarnaast wordt een wachtrij voor persoonlijke berichten gemaakt voor logboekregistratie in Message Queuing. Met de service van de logboekregistratie-listener worden de gegevens uit deze berichtenwachtrij doorgestuurd naar de logboekdatabase.

Aan de RMS-servicegroep zijn uitvoeringsmachtigingen toegewezen voor de opgeslagen procedures in de logboekdatabase.

Omdat met de service van de logboekregistratie-listener grote hoeveelheden gegevens naar de logboekdatabase worden verstuurd, kunnen beheerders het beste filters maken waarmee alleen de gewenste gegevens worden opgeslagen in de logboekdatabase.
