---
TOCTitle: De licentieservice opsporen
Title: De licentieservice opsporen
ms:assetid: '4eabbb76-b359-443a-b737-098c5659e9c6'
ms:contentKeyID: 18114036
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720269(v=WS.10)'
---

De licentieservice opsporen
===========================

Met de licentieservice van RMS worden gebruikslicenties uitgegeven waarmee geverifieerde gebruikers kunnen werken met beveiligde inhoud.

Deze service wordt uitgevoerd op de basiscertificerings- en licentieservers of clusters. Als met een client een gebruikslicentie moet worden aangevraagd, moet eerst de URL voor de virtuele map Licensing in het basiscertificeringscluster worden opgehaald uit Active Directory. De licentieservice is in deze map opgenomen. Vervolgens wordt het pad naar de licentieservice toegevoegd.

De URL voor de virtuele map Licensing in het basiscertificeringscluster, wordt in Active Directory met de volgende notatie opgeslagen:

http://*servernaam*/\_wmcs/Licensing

Wanneer met een server een gebruikslicentie wordt aangevraagd, wordt de bestandsnaam van de licentieservice als volgt toegevoegd aan de URL:

http://*servernaam*/\_wmcs/Licensing/Licensing.asmx

De servicelocatie is de RMS-server of de.NET Passport-account waarmee de uitgiftelicentie is uitgegeven. De URL is opgenomen in de uitgiftelicentie.

| ![](images/Cc720269.note(WS.10).gif)Opmerking                                     |
|----------------------------------------------------------------------------------------------------------------|
| Als u SSL hebt ingeschakeld op de RMS-server, wordt voor deze URL's het verbindingsprotocol https:// gebruikt. |
