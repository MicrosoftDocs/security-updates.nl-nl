---
TOCTitle: 'Inschrijving van de RMS-client'
Title: 'Inschrijving van de RMS-client'
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18114074
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747613(v=WS.10)'
---

Inschrijving van de RMS-client
==============================

Clientcomputers kunnen met de uitgifteservice van RMS worden ingeschreven voor een RMS-clientlicentiecertificaat. Hiermee kunnen auteurs door RMS beveiligde inhoud uitgeven wanneer ze niet zijn aangesloten op het bedrijfsnetwerk. In dit geval worden de uitgiftelicenties met informatie over de gebruiksrechten voor de door RMS beveiligde inhoud die met deze computer is uitgegeven, niet door de uitgifteservice maar door de clientcomputer ondertekend en uitgegeven.

Met de uitgifteservice van RMS worden clientlicentieverleningscertificaten uitgegeven.

Clients worden als volgt ingeschreven:

1.  Vanaf de clientcomputer wordt het rechtenaccountcertificaat van de gebruiker in een inschrijvingsaanvraag verstuurd naar de uitgifteservice die op een basiscertificeringsserver of -cluster of een licentieserver of -cluster wordt uitgevoerd.
2.  Op de server wordt op basis van de netwerkbeheerinstellingen gecontroleerd of de clientinschrijving is toegestaan en of het rechtenaccountcertificaat niet is opgenomen in een uitsluitingslijst in de configuratiedatabase. Zie 'Uitsluitingsbeleid beheren' in 'Een RMS-server beheren' in deze documentatie voor informatie over het maken van uitsluitingslijsten.
3.  In de uitgifteservice wordt een sleutelpaar gemaakt voor de clientcomputer. Daarnaast wordt een clientlicentiecertificaat gemaakt waarin de openbare sleutel wordt opgenomen. De persoonlijke sleutel wordt gecodeerd met de persoonlijke sleutel van het rechtenaccountcertificaat en de gecodeerde sleutel wordt in het certificaat opgenomen.
4.  Met de uitgifteservice wordt een clientlicentiecertificaat verleend aan de clientcomputer.
