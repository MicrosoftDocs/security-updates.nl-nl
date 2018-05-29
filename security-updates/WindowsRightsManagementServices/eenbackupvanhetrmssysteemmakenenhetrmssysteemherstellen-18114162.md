---
TOCTitle: 'Een back-up van het RMS-systeem maken en het RMS-systeem herstellen'
Title: 'Een back-up van het RMS-systeem maken en het RMS-systeem herstellen'
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18114162
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747745(v=WS.10)'
---

Een back-up van het RMS-systeem maken en het RMS-systeem herstellen
===================================================================

Bij het plannen van het systeemherstel moet u rekening houden met een storing aan de databaseserver en een RMS-server. Als er een systeemfout optreedt, kunt u de functionaliteit van een RMS-server of -cluster herstellen met een back-up van de configuratiedatabase. U hebt hiervoor geen nieuw serverlicentieverleningscertificaat of nieuwe persoonlijke sleutel voor de RMS-server nodig, omdat deze items zijn opgeslagen in de configuratiedatabase.

Een back-up van het RMS-systeem plannen
---------------------------------------

Naast de serversleutel worden in de configuratiedatabase gebruikersgegevens, waaronder openbare-sleutelgegevens, opgeslagen. Sla een back-up van de configuratiedatabase op een opslagmedium op en bewaar dit medium op een veilige plaats om de waardevolle sleutelgegevens te beveiligen. Omdat de configuratiedatabase voor het basiscertificeringscluster regelmatig wordt gewijzigd, kunt u het beste regelmatig back-ups maken. Hoe vaker er nieuwe gebruikers aan de organisaties worden toegevoegd, hoe vaker u back-ups moet maken. Als u een back-up van uw basiscertificeringsserver maakt, moet u ook de tabel **sysmessages** uit de hoofddatabase in de back-up opnemen. De basiscertificeringsserver werkt niet en geeft een fout als er in deze tabel geen RMS-specifieke berichten staan. Staat deze tabel niet in de back-up, dan kunt u deze tabel opnieuw maken door het inrichtingsproces opnieuw uit te voeren met behulp van een bestaande database.

De RMS-logboekdatabase bevat logboeken met probleemoplossingen en statistische gegevens, maar deze database is doorgaans niet van essentieel belang voor een RMS-systeem. De Directory Services-database is een lokale cache van de Active Directory-database. Deze cache wordt automatisch opnieuw gemaakt wanneer u een RMS-systeem herstelt. Raadpleeg uw SQL Server-beheerder als u een plan wilt opstellen voor het maken van back-ups van de RMS-databases.

Als u een hardwarebeveiligingsmodule gebruikt om de persoonlijke sleutels van RMS te beveiligen, moet u ook een back-up van de configuratie van de hardwarebeveiligingsmodule maken. Raadpleeg de documentatie voor de hardwarebeveiligingsmodule voor meer informatie over het maken van een back-up en het herstellen van de hardwarebeveiligingsmodule.

| ![](/security-updates/images/Cc747745.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u andere software dan de standaardsoftware als cryptografieprovider voor het coderen van de persoonlijke sleutels van RMS hebt gebruikt, moet u in uw organisatie procedures voor sleutelbeheer, zoals back-up- en herstelprocedures, voor de cryptografieprovider implementeren voordat u deze gebruikt met RMS. |

Het herstellen van een RMS-systeem plannen
------------------------------------------

Als u een databaseserver vanaf een back-up herstelt, moet de versie van de huidige RMS dezelfde versie zijn als toen de back-up werd gemaakt. Laat gebruikers van het RMS-systeem weten dat als zij na het maken van de back-up het RMS-systeem gaan gebruiken, zij een nieuw rechtenaccountcertificaat nodig hebben. Er gaat geen beveiligde inhoud verloren.

U herstelt een RMS-server vanuit een cluster door de server opnieuw te maken, RMS opnieuw te installeren en vervolgens met behulp van de bestaande database de server met het cluster samen te voegen. Deze activiteit heeft geen merkbare gevolgen voor de gebruikers van het RMS-systeem, omdat de servers in het cluster als één geheel werken.
