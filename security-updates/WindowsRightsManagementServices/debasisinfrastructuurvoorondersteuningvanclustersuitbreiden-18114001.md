---
TOCTitle: De basisinfrastructuur voor ondersteuning van clusters uitbreiden
Title: De basisinfrastructuur voor ondersteuning van clusters uitbreiden
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18114001
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747567(v=WS.10)'
---

De basisinfrastructuur voor ondersteuning van clusters uitbreiden
=================================================================

Als u clusters wilt implementeren voor grotere distributies, moet u de infrastructuur zo instellen dat deze de clustervereisten ondersteunt. De volgende items moeten in uw implementatieplanning worden opgenomen.

DNS-registratie
---------------

Zorg dat eventuele DNS-registraties die worden uitgevoerd om het virtuele IP-adres zichtbaar te maken in het extranet, ook worden uitgevoerd om het adres zichtbaar te maken in het intranet.

Wordt voor het intranet geen DNS-registratie uitgevoerd, dan mislukken interne aanvragen voor clientlicenties. Als u de DNS-instellingen niet kunt veranderen, wijzigt u de hosts-tabel van elke server in het cluster om de cluster-URL toe te wijzen aan het virtuele IP-adres van het cluster. DNS-registratie moet worden uitgevoerd voordat de service wordt ingericht. Als u de service al hebt ingericht, moet u RMS van de server verwijderen en de inrichtingsprocedure herhalen.

Taakverdeling
-------------

Stel de vereiste hardware en software in voor de implementatie van taakverdelingsservers, de Network Load Balancing-service of hardwaretaakverdeling om de aanvragen in het cluster te verdelen.
