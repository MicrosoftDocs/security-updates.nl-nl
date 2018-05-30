---
TOCTitle: 'Active Directory-cache van RMS'
Title: 'Active Directory-cache van RMS'
ms:assetid: 'c721a2eb-2fe9-4346-b426-3cc169b97265'
ms:contentKeyID: 18114129
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747662(v=WS.10)'
---

Active Directory-cache van RMS
==============================

Alle RMS-basiscertificeringsservers, RMS-basiscertificeringsclusters en licentieservers hebben een lokale Active Directory-cache waarin de resultaten worden opgeslagen van query's over groepslidmaatschappen in de globale catalogus van Active Directory. Elk cluster maakt naast deze cache gebruik van een gedeelde cache die in de database met adreslijstservices wordt opgeslagen. Het doel van deze caches is dat er minder query's naar de globale catalogus worden verstuurd en dat de reactietijd voor licentieaanvragen wordt verbeterd.

Wanneer een gebruiker een gebruikslicentie aanvraagt, wordt op de betreffende server bepaald of de benodigde rechten zijn opgenomen in de uitgiftelicentie van de gebruiker. In het eenvoudigste geval wordt de naam van de gebruiker die een licentie aanvraagt expliciet genoemd in de uitgiftelicentie. In veel gevallen wijst de auteur de rechten echter aan een groep toe in plaats van aan afzonderlijke gebruikers.

Als de naam van de aanvrager niet expliciet voorkomt in de uitgiftelicentie, maar er in plaats daarvan rechten zijn toegewezen aan een groep, moet op basis van de groepslidmaatschappen van de gebruiker worden bepaald of de gebruiker deel uitmaakt van een groep waaraan rechten zijn toegewezen. In dat geval wordt er een LDAP-query uitgevoerd in de globale catalogus.

Op RMS-servers worden alle resultaten van query's over groepslidmaatschappen zowel in de lokale Active Directory-cache als in de cache van de clusterdatabase met adreslijstservices opgeslagen. Servers kunnen vervolgens informatie over groepslidmaatschappen ophalen uit deze caches waardoor er minder query's naar de globale catalogus worden verstuurd. Standaard wordt de query naar de dichtstbijzijnde server verstuurd. U kunt de registersleutel GC echter zo configureren dat u de query naar de gewenste globale-catalogusservers kunt versturen. Zie 'Registerinstellingen voor de verbindingengroep wijzigen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over deze instelling.

Bij het beoordelen van de groepslidmaatschappen van een gebruiker wordt eerst in de cache van de server gecontroleerd of hierin al informatie is opgeslagen over de groepslidmaatschappen van deze gebruiker. Als dit niet het geval is, wordt de database met adreslijstservices voor het cluster gecontroleerd. Is ook hierin geen informatie over groepslidmaatschappen van de gebruiker opgeslagen, dan wordt de globale catalogus gecontroleerd.

Voor gebruikers en groepen worden de volgende Active Directory-kenmerken opgeslagen in de cache:

-   mail
-   ProxyAddresses (alleen SMTP-e-mailadressen)
-   objectSID
-   sidHistory
-   memberOf (GUID's van groepen waarvan de gebruiker of groep deel uitmaakt)

De vermeldingen in de lokale Active Directory-cache worden voorzien van een tijdstempel. In de registerinstellingen worden de geldigheidsduur voor vermeldingen in de cache en het totale aantal vermeldingen dat in de cache kan worden opgenomen, opgegeven. Deze instellingen kunnen van invloed zijn op de prestaties van de servers. Zie 'Cache-instellingen voor Active Directory wijzigen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.
