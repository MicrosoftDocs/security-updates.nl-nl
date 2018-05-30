---
TOCTitle: Een vertrouwd gebruikersdomein toevoegen
Title: Een vertrouwd gebruikersdomein toevoegen
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18114231
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747793(v=WS.10)'
---

Een vertrouwd gebruikersdomein toevoegen
========================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Een vertrouwd gebruikersdomein toevoegen
----------------------------------------

#### Een vertrouwd gebruikersdomein toevoegen

1.  Open de pagina **Algemeen beheer** en klik naast de website waarop u een vertrouwd gebruikersdomein wilt toevoegen op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Vertrouwensbeleid**.

3.  Klik in het gedeelte **Vertrouwde gebruikersdomeinen** op **Bladeren**. Zoek en dubbelklik op het serverlicentieverleningscertificaat van het gebruikersdomein dat u wilt importeren om de vertrouwensrelatie tot stand te brengen en klik op **Toevoegen**.

    De naam van het domein verschijnt in de lijst **Vertrouwde gebruikersdomeinen**.

4.  Als u wilt aangeven welke e-maildomeinen in het vertrouwde gebruikersdomein worden vertrouwd, klikt u in de lijst naast de certificaatnaam op **Vertrouwde domeinen** om het venster **Vertrouwde e-maildomeinen** te openen.

5.  Kies een van de volgende opties:

    -   Selecteer de optie **Alle e-maildomeinen vertrouwen** als u alle gebruikersaccounts wilt vertrouwen die lid zijn van dat domein.
        - of -
    -   Selecteer de optie **Alleen opgegeven e-maildomeinen vertrouwen** en geef vervolgens de domeinnaam op die u wilt vertrouwen, zoals voorbeeld.com. Klik vervolgens op **Toevoegen**. Het domein wordt aan de lijst Vertrouwde e-maildomeinen toegevoegd. Als u een naam uit de lijst wilt verwijderen, selecteert u de naam en klikt u op **Verwijderen**. Als u een domein aan de lijst toevoegt, worden ook de subdomeinen toegevoegd.

6.  Als u RMS gebruikt in een omgeving waarin u het groepslidmaatschap moet uitbreiden naar forests, schakelt u het selectievakje **RM-licentieverlening aan beveiligings-id's (SID's) voor dit gebruikersdomein vertrouwen** in.

7.  Klik op **Sluit het venster en ga terug naar Vertrouwensbeleid** als u klaar bent.

Zie '[Vertrouwde gebruikersdomeinen toevoegen en verwijderen](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)' eerder in dit onderwerp voor meer informatie over het uitvoeren van deze procedure.
