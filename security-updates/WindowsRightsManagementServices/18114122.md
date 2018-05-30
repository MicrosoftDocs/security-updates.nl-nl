---
TOCTitle: Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken
Title: Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18114122
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747655(v=WS.10)'
---

Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken
=========================================================================

Microsoft voorziet in een accountcertificeringsservice die op basis van Microsoft .NET Passport-referenties het rechtenaccountcertificaat voor de gebruiker regelt. Als u wilt dat gebruikers met rechtenaccountcertificaten die voortkomen uit die service kunnen beschikken over gebruikslicenties uit uw RMS-cluster, moet u een vertrouwd gebruikersdomein instellen dat gebruikersreferenties van de accountcertificeringsservice van Microsoft accepteert.

Om deze functie te kunnen gebruiken, configureert u Internet Information Services zodanig dat anonieme toegang tot de licentieservice van RMS is toegestaan. Deze stap is voor externe gebruikers van groot belang omdat de licentieservice standaard is geconfigureerd voor gebruik van Geïntegreerde Windows-verificatie. Als anonieme toegang niet wordt ingesteld, kunnen externe gebruikers met Passport-RAC's (Rights Account Certificates) geen licenties ontvangen.

Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken
-------------------------------------------------------------------------

#### Anonieme toegang tot de RMS-licentieservice instellen

1.  Open de module **Beheer van Internet Information Services (IIS)** en vouw de server uit die als host optreedt voor RMS.

2.  Vouw **Websites** uit in de consolestructuur en vouw vervolgens de specifieke website uit waarop u RMS hebt geconfigureerd. Dit is standaard de **Standaardwebsite**.

3.  Vouw de website **\_wmcs** uit in de consolestructuur en selecteer vervolgens de virtuele map **Licentieverlening**.

4.  Klik met de rechtermuisknop op de virtuele map **Licentieverlening** en selecteer vervolgens **Eigenschappen**.

5.  Klik in het dialoogvenster **Eigenschappen voor Licentieverlening** op het tabblad **Mapbeveiliging**.

6.  Klik op **Bewerken** in het gebied **Verificatie en toegang beheren**.

7.  Schakel het selectievakje **Anonieme toegang inschakelen** in.

#### Op Passport gebaseerde rechtenaccountcertificaten als vertrouwd aanmerken

1.  Open de pagina **Algemeen beheer** en klik op **RMS op deze website beheren** naast de website waarop u rechtenaccountcertificaten die op Passport zijn gebaseerd, als vertrouwd wilt aanmerken.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Vertrouwensbeleid**.

3.  Klik in het gedeelte **Vertrouwde gebruikersdomeinen** op **RAC's van Passport vertrouwen**. De RM-certificeringsservice van Microsoft verschijnt in de lijst **Vertrouwde gebruikersdomeinen**.

4.  Eventueel kunt u gebruikers uitsluiten op basis van e-mailadressen. Klik hiertoe op **Uitgesloten identiteiten** en typ het e-mailadres van de gebruiker die u niet vertrouwt.
