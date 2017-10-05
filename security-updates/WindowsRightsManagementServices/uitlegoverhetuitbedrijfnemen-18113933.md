---
TOCTitle: Uitleg over het uit bedrijf nemen
Title: Uitleg over het uit bedrijf nemen
ms:assetid: '57bd9949-9433-437b-93ed-ffb2dff9992e'
ms:contentKeyID: 18113933
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720276(v=WS.10)'
---

Uitleg over het uit bedrijf nemen
=================================

Door Internet Information Services (IIS) te gebruiken kan RMS de eigen beschikbare services weergeven. De certificeringsservice bijvoorbeeld schrijft gebruikers en hun computers in en de licentieservice publiceert inhoud en geeft toegang tot door RMS beveiligde gegevens. Er moet een extra service, de zogenaamde service voor uit bedrijf nemen, op de RMS-server worden ingeschakeld om het proces voor het uit bedrijf nemen te starten. Wanneer deze service is ingeschakeld, worden alle andere RMS-services van de server uitgeschakeld.

Als de RMS-server is ingeschakeld voor uit bedrijf nemen, kunnen toepassingen een inhoudssleutel ophalen bij de service Uit bedrijf nemen, waarmee de toepassing de door RMS beveiligde inhoud kan decoderen.

Wanneer de RMS-server in de modus Uit bedrijf nemen wordt gebruikt, kan iedere gebruiker met of zonder de rechten voor de originele door RMS beveiligde inhoud, een inhoudssleutel ophalen en de volledige rechten voor de inhoud verkrijgen.

Nadat de inhoud is gedecodeerd, moet de inhoud zonder RMS-beveiliging worden opgeslagen. Houd er rekening mee dat de gebruiker in de RMS-infrastructuur moet zijn ingeschreven om de service Uit bedrijf nemen te kunnen gebruiken. Een gebruiker zonder een geactiveerde RMS-client kan de service Uit bedrijf nemen niet gebruiken voor toegang tot door RMS beveiligde inhoud.
