---
TOCTitle: 'RMS-beveiligingsgroepen'
Title: 'RMS-beveiligingsgroepen'
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18113852
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720215(v=WS.10)'
---

RMS-beveiligingsgroepen
=======================

Het installatieprogramma van RMS maakt twee groepen: de RMS-servicegroep en de groep Supergebruikers.

De RMS-servicegroep is een lokale beveiligingsgroep waaraan voldoende machtigingen zijn toegewezen voor toegang tot alle bronnen die vereist zijn voor RMS-bewerkingen. Tijdens de installatie geeft de beheerder een gebruikersaccount op die moet worden gebruikt als de RMS-serviceaccount. Deze gebruikersaccount wordt doorgaans automatisch aangemeld als lid van de RMS-servicegroep en beschikt dus over de bijbehorende rechten. Tijdens de meeste bewerkingen wordt RMS uitgevoerd als deze gebruikersaccount.

Een andere belangrijke RMS-groep is de groep Supergebruikers. Deze groep heeft volledig beheer over alle inhoud. Dit betekent dat een lid van deze groep alle door RMS beveiligde inhoudsbestanden kan decoderen en alle RMS-beveiligingen kan verwijderen. Standaard bevat de groep Supergebruikers geen leden en worden RMS-beheerders niet automatisch opgenomen in deze groep. Het beheer van het lidmaatschap van deze groep is essentieel voor de beveiliging van uw door RMS beveiligde inhoud. Zie 'De groep Supergebruikers gebruiken' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.
