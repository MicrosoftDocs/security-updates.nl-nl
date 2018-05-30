---
TOCTitle: Gebruikerssleutels
Title: Gebruikerssleutels
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18113892
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720202(v=WS.10)'
---

Gebruikerssleutels
==================

Een RMS-gebruiker heeft een sleutelpaar met RSA-sleutels van 1024 bits. Het sleutelpaar van de gebruiker wordt in de configuratiedatabase van RMS opgeslagen zodat een gebruiker altijd hetzelfde sleutelpaar gebruikt in het RMS-systeem.

Een rechtenaccountcertificaat bevat de openbare sleutel van de gebruiker. Met deze sleutel wordt de inhoudssleutel in een gebruikslicentie gecodeerd, zodat alleen een bepaalde gebruiker met deze licentie kan werken met door RMS beveiligde inhoud.

Hetzelfde rechtenaccountcertificaat bevat tevens de persoonlijke sleutel van de gebruiker. Deze sleutel wordt gecodeerd met de openbare sleutel van een clientcomputer. Als gevolg hiervan kan een rechtenaccountcertificaat alleen worden gebruikt op de computer waarvoor dit certificaat is uitgegeven. Elk rechtenaccountcertificaat voor een bepaalde gebruiker bevat hetzelfde sleutelpaar. De persoonlijke sleutel van de gebruiker is nodig om met de inhoud te kunnen werken die is beveiligd met RMS.
