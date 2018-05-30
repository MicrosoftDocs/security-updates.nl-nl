---
TOCTitle: On line uitgifte
Title: On line uitgifte
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18114087
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747694(v=WS.10)'
---

On line uitgifte
================

In het volgende schema wordt het proces van on line uitgifte beschreven.

![alt text](/security-updates/images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif "Onlinepublicatieproces")

Het proces voor on line uitgifte omvat de volgende stappen:

1.  De auteur maakt een document en gebruikt de toepassing met RMS-ondersteuning om gebruikers op te geven en rechten en voorwaarden toe te passen op de inhoud.
2.  De toepassing met RMS-ondersteuning genereert een symmetrische inhoudssleutel en vraagt een uitgiftelicentie aan bij de certificaatserver of een licentieserver. In deze aanvraag zijn de inhoudsleutel en de gebruiksinstellingen opgenomen.
3.  De licentieserver genereert de uitgiftelicentie, codeert de inhoudssleutel met de openbare sleutel van de server en stuurt vervolgens de uitgiftelicentie terug naar de toepassing met RMS-ondersteuning.
4.  In de toepassing wordt het bestand gecodeerd met de inhoudsleutel en wordt de uitgiftelicentie gekoppeld aan het bestand.
5.  Vanuit de toepassing met RMS-ondersteuning op de computer van de gebruiker wordt een aanvraag met het rechtenaccountcertificaat van de gebruiker naar de RMS-server (waarmee de uitgiftelicentie is uitgegeven) verstuurd voor een gebruikslicentie voor het document.
6.  De referenties van de gebruiker worden op de RMS-server gecontroleerd. Als de referenties van de gebruiker aan de voorwaarden voldoen, wordt er een gebruikslicentie gegenereerd en naar de toepassing met RMS-ondersteuning op de computer van de gebruiker verstuurd.
7.  Het document wordt geopend in de toepassing met RMS-ondersteuning en wijst de gebruikersrechten toe op basis van de opgegeven parameters in de gebruikslicentie.
