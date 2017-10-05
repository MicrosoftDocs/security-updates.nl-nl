---
TOCTitle: Vertrouwde uitgiftedomeinen toevoegen en verwijderen
Title: Vertrouwde uitgiftedomeinen toevoegen en verwijderen
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18114151
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747687(v=WS.10)'
---

Vertrouwde uitgiftedomeinen toevoegen en verwijderen
====================================================

Standaard kunnen met een RMS-server alleen gebruikslicenties worden uitgegeven die zijn gebaseerd op uitgiftelicenties die met deze of een andere server in het cluster zijn uitgegeven. Als u inhoud hebt die is gepubliceerd met een andere basiscertificeringsserver in uw organisatie (bijvoorbeeld met een server van een vestiging in een ander forest) of in een andere afzonderlijke organisatie, kan uw RMS-server gebruikslicenties verlenen aan gebruikers van deze inhoud als u een vertrouwd uitgiftedomein configureert op uw RMS-server. Als u een vertrouwd uitgiftedomein toevoegt realiseert u een vertrouwensrelatie tussen uw RMS-server en de andere basiscertificeringsserver door het serverlicentieverleningscertificaat van de andere server te importeren. Er is geen maximaal aantal vertrouwde uitgiftedomeinen dat u kunt configureren voor uw RMS-server.

U kunt een vertrouwd uitgiftedomein dat u hebt toegevoegd op elk moment verwijderen door het bijbehorende certificaat te verwijderen uit de lijst met certificaten voor vertrouwde uitgiftedomeinen.

Als u een vertrouwd uitgiftedomein wilt toevoegen, moet u het serverlicentieverleningscertificaat, de persoonlijke sleutel (als deze is opgeslagen in de software en niet in een hardwarebeveiligingsmodule) en alle sjablonen voor het rechtenbeleid importeren voor de RMS-server of het RMS-cluster dat u wilt toevoegen. De beheerder moet deze items eerst van deze server of vanuit dit cluster naar een bestand exporteren dat met een wachtwoord is beveiligd en vervolgens het vereiste wachtwoord voor het decoderen van het bestand opgeven. Vervolgens moet de beheerder het bestand in een gedeelde map opslaan en u op de hoogte stellen van het wachtwoord. Vervolgens kunt u het bestand importeren door de bestandslocatie en het wachtwoord op te geven. Als u het bestand wilt opslaan, moet de account waarmee de **beheertoepassingengroep** wordt uitgevoerd, over machtigingen voor de gedeelde map beschikken.

Zie '[Een vertrouwd uitgiftedomein toevoegen](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c)' verderop in dit onderwerp voor stapsgewijze instructies voor het instellen van een vertrouwd uitgiftedomein.

Als de persoonlijke sleutel is opgeslagen in een hardwarebeveiligingsmodule, moet u de sleutel verplaatsen naar de hardwarebeveiligingsmodule op de vertrouwde server. Volg hierbij de instructies in de documentatie voor de hardwarebeveiligingsmodule. Afhankelijk van het type hardwarebeveiligingsmodule op elke server en de configuratie van de hardwarebeveiligingsmodule-apparaten, kunt u de persoonlijke sleutel mogelijk niet van de ene naar de andere hardwarebeveiligingsmodule verplaatsen. Raadpleeg de documentatie voor de hardwarebeveiligingsmodule om te bepalen of u de persoonlijke sleutel naar een andere hardwarebeveiligingsmodule kunt verplaatsen zonder dat hierbij gegevens verloren gaan. Als u de persoonlijke sleutel niet kunt verplaatsen, kunt u geen vertrouwd uitgiftedomein tot stand brengen tussen de twee servers.

| ![](images/Cc747687.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u de persoonlijke sleutel van RMS beveiligt met een hardwarebeveiligingsmodule en een serverlicentieverleningscertificaat wilt importeren vanuit een RMS-installatie waarin gebruik wordt gemaakt van softwarebeveiliging voor persoonlijke sleutels, moet u op de pagina Beveiligingsinstellingen van elke RMS-server in het cluster een wachtwoord voor persoonlijke sleutels opgeven voordat u het certificaat importeert. |
