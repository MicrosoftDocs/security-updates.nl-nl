---
TOCTitle: 'RMS-computeractivering'
Title: 'RMS-computeractivering'
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18113837
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720182(v=WS.10)'
---

RMS-computeractivering
======================

Computeractivering is een vereiste voor het uitgeven of gebruiken van door RMS beveiligde inhoud op een clientcomputer. Computeractivering is het proces waarbij voor een clientcomputer een unieke lockbox en een bijbehorend RMS-computercertificaat worden uitgegeven. De lockbox bevat de persoonlijke sleutel van de computer. Het bijbehorende computercertificaat bevat de openbare sleutel van de computer. Omdat de lockbox de persoonlijke sleutel van de computer bevat, is een lockbox de belangrijkste beveiligings-principal voor codering en decodering. Iedere gebruiker van de computer heeft een uniek computercertificaat dat tijdens het proces voor computeractivering is gemaakt.

Het proces voor computeractivering dat wordt gebruikt voor de RMS-client voor Service Pack 1, verschilt aanzienlijk van het proces voor computeractivering in versie 1. De RMS-client voor Service Pack 1 is een zelfactiverende client. Wanneer de RMS-client door een aangemelde gebruiker wordt geïnstalleerd of een RMS-functie voor het eerst door een aangemelde gebruiker wordt gebruikt, start de client het activeringsproces dat met de cryptografische API van Windows diverse sets sleutels genereert. Met deze sleutels worden een aantal coderingen uitgevoerd die een computercertificaat genereren waarmee de gebruiker, de computer en de RMS-client met elkaar worden verbonden in de RMS-vertrouwenshiërarchie.
