---
TOCTitle: Off line uitgifte
Title: Off line uitgifte
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18114207
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747741(v=WS.10)'
---

Off line uitgifte
=================

Bij off line uitgifte wordt de uitgiftelicentie voor de toepassing met RMS-ondersteuning op andere wijze verkregen dan bij on line uitgifte.

Voordat een auteur inhoud off line kan uitgeven, moet de auteur een clientlicentiecertificaat ophalen terwijl deze netwerktoegang tot de basiscertificeringsserver heeft.

Het proces voor off line uitgifte omvat de volgende stappen:

1.  De auteur maakt het document met een toepassing met RMS-ondersteuning en geeft de rechten en voorwaarden voor de inhoud op.
2.  Als de auteur het bestand opslaat, kan met de lokale computer of het lokale apparaat een uitgiftelicentie worden uitgegeven en ondertekend op basis van het clientlicentiecertificaat.
    De uitgiftelicentie bevat twee exemplaren van de inhoudsleutel: een sleutel die is gecodeerd met de openbare sleutel van het clientlicentiecertificaat en een sleutel die is gecodeerd met de openbare sleutel van de server waarmee het clientlicentiecertificaat is uitgegeven. De licentie bevat tevens de URL van de server. De twee openbare sleutels en de URL zijn afkomstig uit het clientlicentiecertificaat.
3.  De computer gebruikt het clientlicentieverleningscertificaat voor het maken van een eigenaarslicentie, een speciale gebruikslicentie die de auteur het recht verleent off line met door RMS beveiligde inhoud te werken. Met de persoonlijke sleutel van het clientlicentiecertificaat wordt de symmetrische inhoudsleutel van de uitgiftelicentie gedecodeerd en vervolgens opnieuw gecodeerd als de eigenaarslicentie.
4.  In de toepassing wordt het bestand gecodeerd met de inhoudsleutel en wordt de uitgiftelicentie gekoppeld aan het bestand. Licenties voor het decoderen van dit bestand kunnen alleen worden uitgegeven met de RMS-server waarmee de uitgiftelicentie is uitgegeven of met een server die deel uitmaakt van een vertrouwd uitgiftedomein.
