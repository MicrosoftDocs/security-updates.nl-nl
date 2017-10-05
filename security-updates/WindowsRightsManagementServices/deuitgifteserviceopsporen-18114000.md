---
TOCTitle: De uitgifteservice opsporen
Title: De uitgifteservice opsporen
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18114000
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747580(v=WS.10)'
---

De uitgifteservice opsporen
===========================

Met de uitgifteservice van RMS worden uitgiftelicenties uitgegeven waarmee inhoud wordt beveiligd. Tevens worden hiermee clientlicentiecertificaten uitgegeven waarmee gebruikers inhoud kunnen uitgeven zonder te zijn aangesloten op het bedrijfsnetwerk.

De uitgifteservice is beschikbaar via het basiscertificeringscluster of via licentieservers. In een toepassing met RMS-ondersteuning wordt deze service aangevraagd als een auteur door RMS beveiligde inhoud uitgeeft. Als met een toepassing een uitgifteservice moet worden aangevraagd, moet eerst de URL voor de virtuele map Licensing op de server, waar de uitgifteservice zich bevindt, uit de Active Directory worden opgehaald. Vervolgens wordt het pad naar de uitgifteservice toegevoegd.

De URL voor de virtuele map Licensing van een server wordt in Active Directory in de volgende notatie opgeslagen:

http://*servernaam*/\_wmcs/Licensing

Wanneer met een server een uitgiftelicentie wordt aangevraagd, wordt de bestandsnaam van de uitgifteservice als volgt toegevoegd aan de URL:

http://*servernaam*/\_wmcs/Licensing/Publish.asmx

Als in RMS wordt ontdekt dat het rechtenaccountcertificaat is gebaseerd op Windows-gebruikersverificatie, wordt de locatie van de uitgifteservice bepaald op basis van het Active Directory-forest. Dit geldt zowel voor interne als externe gebruikers die via een VPN-netwerk zijn aangesloten op het bedrijfsnetwerk.

Als in RMS wordt ontdekt dat het rechtenaccountcertificaat is gebaseerd op Microsoft® .NET Passport, komt de locatie van de uitgifteservice overeen met de locatie van de .NET Passport-account die is opgegeven in de door RMS beveiligde inhoud.

| ![](images/Cc747580.note(WS.10).gif)Opmerking                                     |
|----------------------------------------------------------------------------------------------------------------|
| Als u SSL hebt ingeschakeld op de RMS-server, wordt voor deze URL's het verbindingsprotocol https:// gebruikt. |
