---
TOCTitle: Gebruikersaccounts verwijderen
Title: Gebruikersaccounts verwijderen
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18114121
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747653(v=WS.10)'
---

Gebruikersaccounts verwijderen
==============================

Als u een gebruikersaccount uit Active Directory verwijdert, wordt de vermelding van het rechtenaccountcertificaat van de gebruiker, die zich in de tabel met gebruikerssleutels van de configuratiedatabase voor het basisconfiguratiecluster bevindt, niet automatisch verwijderd. Als gevolg daarvan is de grootte van de tabel met gebruikerssleutels niet aan beperkingen gebonden omdat nieuwe gebruikerssleutels wel worden toegevoegd, maar oude gebruikerssleutels niet worden verwijderd.

Als u de configuratiedatabase wilt onderhouden, kunt u een opgeslagen procedure uitvoeren waarmee een gebruikerssleutel op basis van de beveiligings-id (SID) wordt verwijderd als de bijbehorende gebruikersaccount uit Active Directory wordt verwijderd. U kunt ook regelmatig een script uitvoeren waarmee gebruikerssleutels uit de configuratiedatabase worden verwijderd als de bijbehorende SID's niet meer aanwezig zijn in Active Directory. Bij deze methode worden zowel SQL Server als Active Directory zwaar belast.
