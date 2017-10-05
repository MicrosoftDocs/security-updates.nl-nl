---
TOCTitle: De proxyinstellingen voor RMS wijzigen
Title: De proxyinstellingen voor RMS wijzigen
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18114054
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747594(v=WS.10)'
---

De proxyinstellingen voor RMS wijzigen
======================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Zie Help van Internet Information Services voor meer informatie over verificatiemethoden voor proxyservers en hoe deze in Windows Server 2003 werken.

De proxyinstellingen voor RMS wijzigen
--------------------------------------

#### De proxyinstellingen voor RMS wijzigen

1.  Open de pagina **Algemeen beheer** en klik op **RMS op deze website beheren**.

2.  Klik bij **Clusterbeheer** op **Beveiligingsinstellingen**.

3.  Als u niet eerder een proxyserver met RMS hebt gebruikt, schakelt u het selectievakje **Deze computer maakt via een proxyserver verbinding met het Internet** in. Vervolgens worden er extra instellingen weergegeven die u kunt configureren.

4.  Typ in het vak **Adres** het IP-adres of de DNS-naam van de proxyserver die u wilt gebruiken.

5.  Typ in het vak **Poort** het poortnummer dat door de proxyserver wordt gebruikt om verbinding te maken met internet.

6.  Als u de proxyserver niet gebruikt om verbinding met lokale bronnen te maken, schakelt u het selectievakje **Proxyserver niet gebruiken voor lokale adressen** in.

7.  Schakel desgewenst het selectievakje **Deze proxyserver vereist verificatie** in.

    -   Selecteer het verificatietype **Basisverificatie**, **Verificatiesamenvatting** of **Geïntegreerde Windows-verificatie** in de lijst.
    -   Typ bij **Gebruikersnaam** de gebruikersnaam die moet worden opgegeven wanneer hierom wordt verzocht door de proxyserver.
    -   Typ bij **Wachtwoord** het wachtwoord dat moet worden opgegeven wanneer hierom wordt verzocht door de proxyserver.
    -   Typ bij **Wachtwoord bevestigen** hetzelfde wachtwoord zodat kan worden gecontroleerd of u het wachtwoord eerder correct hebt getypt.
    -   Als voor de proxyserver Geïntegreerde Windows-verificatie is ingesteld, typt u bij **Domein** het domein van de gebruiker.

8.  Klik op **Verzenden**.
