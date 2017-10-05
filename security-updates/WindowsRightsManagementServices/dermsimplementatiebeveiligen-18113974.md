---
TOCTitle: 'De RMS-implementatie beveiligen'
Title: 'De RMS-implementatie beveiligen'
ms:assetid: '6de8b636-a824-4844-aefc-f26347abfc14'
ms:contentKeyID: 18113974
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720291(v=WS.10)'
---

De RMS-implementatie beveiligen
===============================

Een RMS-implementatie is van groot belang voor elke organisatie die dezelfde beveiligingsmaatregelen ten aanzien van locatie en netwerk nodig heeft als voor andere cruciale servers in de netwerkomgeving. Onderdeel van de implementatie van de RMS-server is het in kaart brengen van de specifieke dreigingen voor deze servers en de te nemen tegenmaatregelen.

RMS wordt geïmplementeerd als een webservice, dus kunt u met behulp van toegangsbeheerlijsten en Secure Sockets Layer (SSL) de toegang tot RMS op dezelfde manier regelen als bij andere webservices.

**Toegang tot RMS-webservices met behulp van toegangslijsten beperken**

Met behulp van toegangslijsten kunt u de toegang tot RMS-services beperken. Elke virtuele hoofdmap die is gemaakt toen RMS werd ingericht op een website, heeft een overeenkomende mappenstructuur die kan worden beveiligd. De mappenstructuur staat standaard in &lt;systeemstation&gt;:\\&lt;*webhoofdmap*&gt;\\\_wmcs, waarbij *webhoofdmap* de naam is van de map die is toegewezen aan de website waarop u RMS hebt ingericht. Sommige webservices zoals de inschrijvingsservice, de certificeringsservice voor mobiele apparaten en de certificeringsservice voor serverservices zijn standaard beperkt. De gebruikers en groepen die de service mogen gebruiken, moeten daarvoor eerst aan de toegangslijst worden toegevoegd.

De certificeringsservice voor serverservices levert rechtenaccountcertificaten (RAC) waarmee services die door RMS worden beveiligd (waaronder websites voor samenwerking, e-mailservers en servers voor documentbeheer), kunnen worden benaderd, ter ondersteuning van de aanvullende componenten van een RMS-systeem, zoals:

-   Een server voor samenwerking aan documenten waar gebruikers onbeveiligde documenten kunnen uploaden. Gedownloade documenten worden echter automatisch door RMS beveiligd conform het rechtenbeleid voor het type inhoud. Een voorbeeld hiervan is Microsoft Office SharePoint Server 2007.
-   Een documentbeheersysteem dat als een algemene opslag en algemeen archief voor documenten fungeert (beveiligd en niet-beveiligd). Het systeem kan met rechten beveiligde documenten voor zoekopdrachten indexeren, zonder dat het rechtenbeleid dat door de maker van de inhoud is gedefinieerd, daarbij verloren gaat.
-   De e-mailserver met rechten beveiligde inhoud laten openen voor controle op virussen en spam of als onderdeel van een juridische bepaling of van een beleid binnen het bedrijf ten aanzien van e-mailberichten.

Omdat voor deze scenario's licenties namens de gebruikers zijn vereist, moet u ervoor zorgen dat de mogelijkheid om rechtenaccountcertificaten voor de service te verkrijgen alleen is voorbehouden aan de servers binnen uw organisatie die daarvoor zijn goedgekeurd en afdoende zijn beveiligd.

**Toegang tot RMS-webservices met behulp van SSL beperken**

U wordt aangeraden SSL (Secure Sockets Layer) in te schakelen en bij elk van de bestanden van de RMS-webservices 128-bits codering te gebruiken. Dit zijn de ASMX-bestanden die in de virtuele mappen Licensing, Certification en Admin zijn opgenomen. Voor SSL is het nodig dat er op uw server een geldig SSL-certificaat voor de website is geïnstalleerd. Als u SSL op de map \_wmcs van de RMS-installatie toepast, nemen de submappen en bestanden deze instelling over. Zie 'Internet Information Services' in de sectie 'Technische referentie van RMS' van deze documentatie voor meer informatie over webservicebestanden en virtuele mappen.

| ![](images/Cc720291.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u de webpagina's voor Windows RMS-beheer wilt openen in een browser op een externe computer, moet u SSL inschakelen. Zelfs als SSL is ingeschakeld, dan nog kunt u de pagina **Algemeen beheer** niet op een externe computer openen. Zie 'De introductiepagina van de beheerwebsite gebruiken' in 'RMS beheren' in deze documentatie voor meer informatie over het externe beheer van RMS. |

**Een sterk wachtwoord instellen voor de persoonlijke sleutel**

Het wachtwoord voor de persoonlijke sleutel wordt gebruikt om de persoonlijke sleutel te maken en veilig op te slaan in de RMS-configuratiedatabase. Er sterk wachtwoord is aan te bevelen voor een maximale beveiliging. Als u het wachtwoord moet noteren, zorgt u er dan voor dat dit wachtwoord in een fysiek beveiligde omgeving wordt bewaard.

| ![](images/Cc720291.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u het wachtwoord voor de persoonlijke sleutel kwijtraakt of niet meer weet en de RMS-server raakt onverwacht offline, moet u alle RMS-documenten decoderen, uw RMS-omgeving opnieuw opbouwen en alles vervolgens opnieuw coderen met de nieuwe persoonlijke sleutel. |
