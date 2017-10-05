---
TOCTitle: 'RMS-serversleutels'
Title: 'RMS-serversleutels'
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18113941
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720280(v=WS.10)'
---

RMS-serversleutels
==================

Een RMS-server heeft een sleutelpaar met RSA-sleutels van 1024 bits.

Met de openbare sleutel van de server wordt de inhoudssleutel in een uitgiftelicentie gecodeerd, zodat de inhoudssleutel alleen met de RMS-server kan worden opgehaald en gebruikslicenties alleen met de RMS-server kunnen worden uitgegeven op basis van deze uitgiftelicentie. Het serverlicentiecertificaat bevat de openbare sleutel van de server.

Met de persoonlijke sleutel van de server worden de certificaten en licenties ondertekend die door de server worden uitgegeven.

Beveiliging van de persoonlijke sleutel van de server
-----------------------------------------------------

Standaard wordt de persoonlijke sleutel van de server tijdens het inrichten gemaakt en gecodeerd opgeslagen in de RMS-database. U kunt tijdens het inrichten ook een CSP (cryptografieprovider) opgeven die al op de server is geïnstalleerd.

U kunt een CSP op twee manieren gebruiken:

-   Kies uit de software-CSP's die standaard op de server zijn geïnstalleerd.
    - of -
-   Gebruik een software-CSP van derden die u op de server hebt geïnstalleerd.

| ![](images/Cc720280.note(WS.10).gif)Opmerking                                   |
|--------------------------------------------------------------------------------------------------------------|
| Als u een hardwarebeveiligingsmodule wilt gebruiken, moet u een CSP selecteren die deze modules ondersteunt. |

Als u de persoonlijke sleutel van de server beveiligt met een CSP, worden in RMS de namen opgeslagen van de provider en van de sleutelcontainer die is opgenomen in de configuratiedatabase.
