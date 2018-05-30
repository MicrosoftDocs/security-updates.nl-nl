---
TOCTitle: Inschrijving van RMS
Title: Inschrijving van RMS
ms:assetid: '999db3e1-e3ab-4513-87d9-d584ee334c00'
ms:contentKeyID: 18114099
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747698(v=WS.10)'
---

Inschrijving van RMS
====================

Met het serverinschrijvingsproces wordt een serverlicentieverleningscertificaat gemaakt en geleverd. Met serverlicentieverleningscertificaten wordt de identiteit van de servers in de implementatie gevalideerd en worden referenties gevalideerd als er met door RMS beveiligde inhoud wordt gewerkt. De eerste server in elk licentiecluster wordt als onderdeel van het inrichtingsproces bij het basiscertificeringscluster ingeschreven. Overige servers in het cluster worden niet apart ingeschreven.

De eerste server van een basiscertificeringscluster (de basiscertificeringsserver) moet worden ingeschreven bij de inschrijvingsservice van Microsoft. Deze inschrijving kan automatisch als onderdeel van de inrichting worden uitgevoerd als de basiscertificeringsserver een internetverbinding heeft. De server kan ook off line worden ingeschreven door een aanvraag daartoe naar een bestand te exporteren en vervolgens dat bestand vanaf een andere computer met een internetverbinding naar de inschrijvingsservice van Microsoft te versturen. Na de inschrijvingsaanvraag zult u voor de basiscertificeringsserver een serverlicentieverleningscertificaat ontvangen dat kan worden geïmporteerd met de beheerpagina's van RMS.

De inschrijvingsaanvraag bevat de volgende informatie:

-   Informatie over intrekking. De RMS-installatie gebruikt standaard of aangepaste (door derden uitgevoerde) intrekking. Als intrekking door derden wordt gebruikt, wordt de openbare sleutel van de intrekkingsautoriteit opgenomen in de intrekkingsinformatie.
-   Openbare sleutel van het certificaat. De openbare sleutel van het serverlicentieverleningscertificaat. Deze openbare sleutel wordt gegenereerd op de RMS-server en vervolgens verstuurd naar de inschrijvingsservice van Microsoft, zodat het serverlicentieverleningscertificaat kan worden verkregen.
-   SKU. De officiële RMS SKU.
-   Versie. Het versienummer van de RMS-assemblage.
-   URL. De basis-URL van het RMS-servercluster.

Als de Microsoft-inschrijvingsservice een antwoord geeft op de inschrijvingsaanvraag, geeft deze in XML-formaat de volgende informatie aan de RMS-server:

-   Serverlicentieverleningscertificaat.
-   Certificaatsketen van ondertekenende autoriteiten.

Dezelfde informatie wordt overgedragen, ongeacht of de RMS-basiscertificeringsserver on line of off line wordt ingeschreven. Bij beide methoden wordt er geen aanvullende informatie verzameld.

Zie 'Een basiscertificeringsserver off line of on line inschrijven' in 'Een RMS-server beheren' in deze documentatie voor het off line inschrijven van de server.

Tijdens het clientinschrijvingsproces wordt een clientlicentieverleningscertificaat gemaakt en aan de clientcomputer geleverd. Met dit clientlicentieverleningscertificaat kan een auteur door RMS beveiligde inhoud uitgeven vanaf een computer die niet is aangesloten op het bedrijfsnetwerk. Een auteur kan op elk moment een clientlicentieverleningscertificaat aanvragen. Clientinschrijving is niet vereist.

Alle inschrijvingsaanvragen worden vastgelegd.

Dit gedeelte bevat de volgende onderwerpen:

-   [Inschrijving van de basiscertificeringsserver](https://technet.microsoft.com/f08bc919-f090-4843-b2ce-b40d558012ce)
-   [Subinschrijving van de licentieserver](https://technet.microsoft.com/7bc63397-9186-464c-8824-867038adce9b)
-   [Inschrijving van de RMS-client](https://technet.microsoft.com/9c1d07bf-7235-4694-8291-ac2e5b221f4a)
-   [RMS-computeractivering](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)
-   [RMS-accountcertificering](https://technet.microsoft.com/c9a385c5-6dbb-47f5-a80f-69718e6f9deb)
