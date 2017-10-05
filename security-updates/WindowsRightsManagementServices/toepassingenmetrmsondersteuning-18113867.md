---
TOCTitle: 'Toepassingen met RMS-ondersteuning'
Title: 'Toepassingen met RMS-ondersteuning'
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18113867
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720231(v=WS.10)'
---

Toepassingen met RMS-ondersteuning
==================================

Gebruikers die met door RMS beveiligde inhoud willen werken of dergelijke inhoud willen maken, moeten over een toepassing met RMS-ondersteuning beschikken, zoals wordt beschreven in dit onderwerp. Daarnaast moet de RMS-client worden geïnstalleerd en de computers die hier gebruik van maken, moeten worden geactiveerd. Zie '[RMS-client](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2)' en '[RMS-computeractivering](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)' verderop in dit onderwerp voor meer informatie.

Met toepassingen met RMS-ondersteuning kunnen auteurs gebruiksrechten in de vorm van uitgiftelicenties aan bestanden koppelen en zodoende bepalen op welke wijze met de inhoud wordt gewerkt. In deze toepassingen worden de gecodeerde bestandsgegevens verwerkt. Daarnaast kunnen gebruikers met deze toepassingen op basis van de opgegeven machtigingen in de uitgiftelicentie met de inhoud werken.

Met de SDK voor RMS-clients kunnen ontwikkelaars toepassingen met RMS-ondersteuning maken waarmee door RMS beveiligde inhoud kan worden gelicentieerd, uitgegeven en gebruikt. Toepassingen met RMS-ondersteuning kunnen worden ontwikkeld voor computers met Microsoft® Windows® 98 Second Edition of later.

Ontwikkelaars kunnen ook servertoepassingen met RMS-ondersteuning maken met de SDK voor RMS-clients. Met deze toepassingen kan inhoud wel worden uitgegeven, maar niet worden gebruikt.

Gebruikers die geen andere toepassing met RMS-ondersteuning hebben voor het werken met door RMS beveiligde inhoud in e-mailberichten en webpagina's, kunnen de Rights Management-invoegtoepassing voor Microsoft® Internet Explorer gebruiken. Zo kunnen OWA-gebruikers (Outlook Web Access) de Rights Management-invoegtoepassing voor Internet Explorer gebruiken als ze willen werken met door RMS beveiligde e-mailberichten.

U kunt deze invoegtoepassing voor Internet Explorer downloaden van de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450).

| ![](images/Cc720231.note(WS.10).gif)Opmerking                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u de Rights Management-invoegtoepassing voor Internet Explorer bij Windows XP Service Pack 2 gebruikt, kan de verbeterde beveiligingsconfiguratie voor problemen met de compatibiliteit van de toepassing zorgen. |

Als de URL van de extranetverbinding voor elk domein binnen uw organisatie niet is toegevoegd aan de lokale intranetsites in Internet Explorer, ontvangen gebruikers die de Rights Management-invoegtoepassing voor Internet Explorer gebruiken, steeds berichten met de vraag of zij verbinding met de sites willen maken. Door deze vraag verkeerd te beantwoorden kan de RMS-client een nieuw rechtenaccountcertificaat voor de gebruikersaccount krijgen.

U stelt deze sites op de juiste manier in de gehele organisatie in door een script te gebruiken waarmee de noodzakelijke URL's als onderdeel van de lokale intranetzone in het register worden weggeschreven. De lokale intranetzone biedt standaard voldoende beveiliging om de berichten tegen te houden.
