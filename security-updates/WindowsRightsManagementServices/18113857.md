---
TOCTitle: Clientlicentiesleutels
Title: Clientlicentiesleutels
ms:assetid: '28781125-2692-4ff9-99b1-e09227d72966'
ms:contentKeyID: 18113857
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720221(v=WS.10)'
---

Clientlicentiesleutels
======================

Met clientlicentieverleningscertificaten kunnen auteurs door RMS beveiligde inhoud uitgeven zonder te zijn aangesloten op het netwerk met RMS-ondersteuning. Een clientlicentiecertificaat heeft een sleutelpaar met RSA-sleutels van 1024 bits.

Het clientonderdeel van RMS gebruikt de openbare sleutel van het clientlicentieverleningscertificaat wanneer er een uitgiftelicentie wordt uitgegeven, zodat de volgende taken kunnen worden uitgevoerd:

-   Het coderen van de symmetrische inhoudsleutel.
-   Het ondertekenen van uitgiftelicenties die lokaal worden uitgegeven als de gebruiker niet is aangesloten op het netwerk.
