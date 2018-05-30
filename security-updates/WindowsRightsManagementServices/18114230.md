---
TOCTitle: Rechtenaccountcertificaten uitsluiten
Title: Rechtenaccountcertificaten uitsluiten
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18114230
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747785(v=WS.10)'
---

Rechtenaccountcertificaten uitsluiten
=====================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Deze voorwaarden worden afgedwongen door de client op het moment dat de gebruikslicentie aan de beveiligde inhoud wordt gebonden.

Rechtenaccountcertificaten uitsluiten
-------------------------------------

#### Rechtenaccountcertificaten uitsluiten

1.  Open de pagina **Algemeen beheer** en klik naast de website waarop u rechtenaccountcertificaten wilt uitsluiten op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Uitsluitingsbeleid**.

3.  Klik in het gedeelte rechtenaccountcertificaatuitsluiting op **Inschakelen** om het rechtenaccountcertificaat van een gebruiker uit te sluiten.

4.  Selecteer de methode waarmee het uit te sluiten accountcertificaat moet worden opgegeven:

    -   Als u het accountcertificaat wilt uitsluiten op basis van de gebruikersnaam, klikt u op **Gebruikersnaam** voor het uit te sluiten rechtenaccountcertificaat. Typ de naam van de uit te sluiten gebruiker (met de indeling *gebruikersnaam*@*domeinnaam.com*) en klik op **Toevoegen**. Deze optie is bestemd voor het uitsluiten van accountcertificaten van interne gebruikers met Active Directory-gebruikersaccounts.
    -   Als u een accountcertificaat wilt uitsluiten op basis van de openbare sleutel, klikt u op **Openbare-sleuteltekenreeks** voor het uit te sluiten rechtenaccountcertificaat. Typ de openbare-sleuteltekenreeks van het betreffende rechtenaccountcertificaat en klik op **Toevoegen**. Deze optie is bestemd voor het uitsluiten van accountcertificaten van externe gebruikers zonder Active Directory-gebruikersaccounts.

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                     |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Als u een accountcertificaat wilt verwijderen uit de uitsluitingslijst, selecteert u het uitgesloten rechtenaccountcertificaat in de lijst en klikt u op **Geselecteerde openbare sleutels van de uitsluitingslijst verwijderen**. De gebruiker met het betreffende accountcertificaat kan nu een licentie krijgen voor RMS-beveiligde inhoud van deze server. |

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Opmerking                                     |
    |----------------------------------------------------------------------------------------------------------------|
    | Als u de uitsluiting van rechtenaccountcertificaten wilt uitschakelen, dient u op **Uitschakelen** te klikken. |

Zie '[Rechtenaccountcertificaten uitsluiten](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)' eerder in dit onderwerp voor meer informatie over de uitvoering van deze procedure.
