---
TOCTitle: Uitgiftelicenties
Title: Uitgiftelicenties
ms:assetid: '187228fc-370b-4e23-a53a-21bb296b84a1'
ms:contentKeyID: 18113905
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720211(v=WS.10)'
---

Uitgiftelicenties
=================

Gebruikers van toepassingen met RMS-ondersteuning kunnen aan digitale bestanden en gegevens specifieke gebruiksrechten toewijzen die consistent zijn met het bedrijfsbeleid. Deze gebruiksrechten zijn opgenomen in uitgiftelicenties waarin wordt aangegeven welke gebruikers de inhoud kunnen weergeven en op welke wijze de inhoud kan worden bewerkt en gedistribueerd.

Een uitgiftelicentie kan worden uitgegeven door een clienttoepassing met RMS-ondersteuning, de basiscertificeringsserver of een RMS-licentieserver. Wanneer een uitgiftelicentie wordt uitgegeven door een clienttoepassing met RMS-ondersteuning, wordt er door de RMS-server een clientlicentieverleningscertificaat aan de toepassing verstrekt. Dit wordt ook wel off line uitgifte genoemd. Dit is een algemene manier van uitgeven, omdat gebruikers van toepassingen met RMS-ondersteuning zonder verbinding met de RMS-server beveiligde inhoud kunnen maken. Als de clienttoepassing met RMS-ondersteuning geen gebruikmaakt van het clientlicentieverleningscertificaat, moet de gebruiker verbinding kunnen maken met een RMS-server om een uitgiftelicentie voor de beveiligde inhoud te kunnen ontvangen.

Een uitgiftelicentie bevat de symmetrische inhoudssleutel voor het decoderen van de inhoud die is gecodeerd met de openbare sleutel van de RMS-server. Het gevolg hiervan is dat alleen met de server inhoud kan worden gecodeerd en gebruikslicenties kunnen worden uitgegeven.

Een uitgiftelicentie wordt ondertekend met de persoonlijke sleutel van de uitgifteserver of de persoonlijke sleutel van het clientlicentiecertificaat.
