---
TOCTitle: 'RMS-accountcertificering'
Title: 'RMS-accountcertificering'
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18114172
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747750(v=WS.10)'
---

RMS-accountcertificering
========================

Tijdens het accountcertificeringsproces wordt een rechtenaccountcertificaat gemaakt waarmee een gebruikersaccount aan een bepaalde computer wordt gekoppeld, zodat de gebruiker op die computer met door RMS beveiligde inhoud kan werken. De eerste keer dat een gebruiker door RMS beveiligde inhoud uitgeeft of op een clientcomputer probeert te werken met door RMS beveiligde inhoud, wordt door de toepassing met RMS-ondersteuning een aanvraag voor een rechtenaccountcertificaat verstuurd naar de accountcertificeringsservice van RMS.

De certificeringsservice kan de gebruiker verifiëren via de verificatie van Windows of een x.509-certificaat dat is opgeslagen in een hardwarecoderingsapparaat, zoals een smartcard. Nadat de gebruiker is geverifieerd, wordt er op de RMS-server een rechtenaccountcertificaat voor de gebruiker gemaakt op basis van zijn of haar geverifieerde referenties. De persoonlijke sleutel van de gebruiker wordt gecodeerd met de openbare sleutel van het RMS-computercertificaat van de clientcomputer en de gecodeerde sleutel wordt opgenomen in het rechtenaccountcertificaat. Vervolgens wordt het rechtenaccountcertificaat verstuurd naar de toepassing waarmee het certificaat is aangevraagd en op de computer of het apparaat opgeslagen. Zodoende is het beschikbaar voor toekomstige aanvragen voor uitgifte- of gebruikslicenties. Het rechtenaccountcertificaat wordt ook opgeslagen in de configuratiedatabase.

Accountcertificering wordt na computeractivering uitgevoerd omdat het RMS-computercertificaat van de clientcomputer moet worden opgenomen in aanvragen voor het rechtenaccountcertificaat.

Gebruikers moeten voor elke computer een rechtenaccountcertificaat aanvragen. Als een gebruiker met meerdere computers werkt, wordt voor elke computer een uniek rechtenaccountcertificaat uitgegeven, maar op elke computer is hetzelfde sleutelpaar voor die gebruiker opgenomen.

Als met een toepassing met RMS-ondersteuning een gebruikslicentie wordt aangevraagd, wordt het rechtenaccountcertificaat opgenomen in de aanvraag. In de licentieservice wordt de persoonlijke sleutel van het rechtenaccountcertificaat gebruikt voor het coderen van de inhoudssleutel. Hierdoor kan de gebruikslicentie alleen worden gebruikt door de geverifieerde gebruiker.

Het proces voor accountcertificering omvat de volgende stappen:

1.  De eerste keer dat een gebruiker door RMS beveiligde inhoud uitgeeft of op een bepaalde computer probeert te werken met door RMS beveiligde inhoud, verstuurt de toepassing met RMS-ondersteuning een aanvraag voor een rechtenaccountcertificaat naar de accountcertificeringsservice die wordt uitgevoerd op de basiscertificeringsserver.
2.  In de accountcertificeringsservice wordt de gebruiker geverifieerd met Windows-verificatie.
3.  In de service voor accountcertificering wordt voor de gebruiker een rechtenaccountcertificaat gemaakt dat is gebaseerd op zijn of haar geverifieerde referenties. De persoonlijke sleutel van de gebruiker wordt gecodeerd met de openbare sleutel van het RMS-computercertificaat en de gecodeerde sleutel wordt opgenomen in het certificaat. Vervolgens wordt het rechtenaccountcertificaat verleend aan de toepassing waarmee de aanvraag is verstuurd.
4.  Het rechtenaccountcertificaat wordt op de computer of het apparaat opgeslagen zodat het beschikbaar is voor toekomstige aanvragen voor uitgifte- of gebruikslicenties.

Het type accountcertificeringsservice waarmee de client het rechtenaccountcertificaat aanvraagt, is afhankelijk van de computer waarop de RMS-client is geïnstalleerd. Standaarddesktopcomputers maken verbinding met de accountcertificeringsservice (certification.asmx). De serverservices die zijn ingeschakeld voor gebruik met RMS SP1, ontvangen de rechtenaccountcertificaten van de servercertificeringsservice (ServeCertfication.asmx). De mobiele apparaten die zijn ingeschakeld voor gebruik met RMS SP1, ontvangen de rechtenaccountcertificaten van de certificeringsservice voor mobiele apparaten (MobileDeviceCertfication.asmx). In een standaardinstallatie van RMS SP1 is alleen de accountcertificeringsservice ingeschakeld.

Zie 'Ondersteuning van RMS-server voor mobiele apparaten en serverservices mogelijk maken' in het gedeelte 'Een RMS-server beheren' in deze documentatie voor meer informatie over het gebruik van RMS SP1 bij mobiele apparaten en serverservices.
