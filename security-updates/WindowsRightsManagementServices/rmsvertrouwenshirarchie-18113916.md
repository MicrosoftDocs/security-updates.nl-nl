---
TOCTitle: 'RMS-vertrouwenshiërarchie'
Title: 'RMS-vertrouwenshiërarchie'
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18113916
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720232(v=WS.10)'
---

RMS-vertrouwenshiërarchie
=========================

Een RMS-systeem bestaat uit de inschrijvingsservice van Microsoft, de RMS-organisatieservers, clientcomputers en gebruikers van het systeem. Aan elk onderdeel wordt een certificaat uitgegeven waarmee de identiteit van het onderdeel in het systeem wordt vastgesteld. Met een vertrouwenshiërarchie wordt de vertrouwensrelatie tussen deze certificaten, en dus ook de entiteiten waarvoor deze gelden, gedefinieerd. Tevens wordt hiermee de vertrouwensrelatie gedefinieerd tussen vertrouwde entiteiten en de licenties die hiermee worden verleend aan andere vertrouwde entiteiten.

De vertrouwenshiërarchie verbindt certificaten en licenties in een vertrouwensketen, waardoor in RMS een bepaald certificaat of een bepaalde licentie altijd kan worden herleid tot een vertrouwd sleutelpaar. De vertrouwensketen bevat het huidige certificaat, het certificaat van de entiteit waarmee het is uitgegeven, het certificaat van de entiteit waarmee het certificaat van deze entiteit is uitgegeven en alle overige gebruikte certificaten en licenties tot en met de basis van de vertrouwensketen.

Voor RMS bestaat de basis van de vertrouwensketen, het 'vertrouwensanker', uit een Microsoft-sleutelpaar. Met deze gemeenschappelijke vertrouwensbasis als uitgangspunt kan een organisatie een ecosysteem van vertrouwen opbouwen om de vertrouwde entiteiten, zoals interne en externe gebruikers en partners, in op te nemen.

In het volgende schema wordt de vertrouwenshiërarchie in een organisatie weergegeven. De vertrouwensketen kan worden herleid tot de Microsoft-services waarmee de basiscertificaten zijn uitgegeven.

![alt text](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif "Vertrouwensrelatiehiërarchie")
1.  Aan elke clientcomputer wordt een unieke lockbox uitgegeven waarin de openbare hoofdsleutel van Microsoft is opgenomen.
2.  Wanneer een licentie wordt aangevraagd, worden de principals gevalideerd in RMS. Hierbij wordt in de vertrouwenshiërarchie het pad naar de basis van de vertrouwensketen gecontroleerd.
3.  In RMS wordt de authenticiteit gecontroleerd van de vertrouwde entiteit in de licentie.
4.  In RMS wordt gecontroleerd of het certificaat van de vertrouwde entiteit is uitgegeven door een server die is opgenomen in de vertrouwenshiërarchie.

De licentie of het certificaat wordt op elk niveau van de certificaatketen gevalideerd. Vervolgens wordt gecontroleerd of de licentie of het certificaat via een vertrouwensketen is verbonden met een bekende vertrouwensbasis. Alle licenties en certificaten in de keten worden in RMS gecontroleerd op de volgende punten:

-   De XrML is geldig.
-   De handtekening van de uitgever is geldig.
-   De semantiek van de licentie is geschikt voor het bestemde gebruik.
-   Aan de voorwaarden, zoals de geldigheidsdatums, is voldaan.
-   De licentie is niet ingetrokken.
-   De handtekeningsleutel van de licentie komt overeen met de sleutel van de gecertificeerde uitgever.
