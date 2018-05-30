---
TOCTitle: Een sjabloon voor het rechtenbeleid bewerken
Title: Een sjabloon voor het rechtenbeleid bewerken
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18114081
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747684(v=WS.10)'
---

Een sjabloon voor het rechtenbeleid bewerken
============================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Sjablonen voor het rechtenbeleid bewerken
-----------------------------------------

#### Een sjabloon voor het rechtenbeleid bewerken

1.  Open de pagina **Algemeen beheer** en klik naast de website waarop u de sjabloon voor het rechtenbeleid wilt bewerken op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Sjablonen voor het rechtenbeleid**.

3.  Klik onder **Sjabloonnaam** op de naam van de sjabloon die u wilt bewerken.

4.  Breng in het gedeelte **Sjabloonidentificatie** de gewenste wijzigingen aan in de informatie bij **Sjabloonnaam**, **Sjabloonbeschrijving** en **URL voor het aanvragen van rechten**.

5.  Voer in het gedeelte **Gebruikers en groepen** een of meer van de volgende handelingen uit:

    -   Een gebruiker of groep toevoegen: typ bij **Gebruikers of groepen toevoegen** het geldige e-mailadres van een gebruiker of groep die u wilt toevoegen, klik op **Toevoegen** en selecteer de naam in **Huidige gebruikers of groepen**. Selecteer bij **Rechten** alle rechten die u aan de geselecteerde gebruiker of groep wilt toekennen.
    -   De rechten van een bestaande gebruiker of groep wijzigen: selecteer de naam in **Huidige gebruikers of groepen** en schakel de selectievakjes voor de rechten in of uit.
    -   Een gebruiker of groep verwijderen: selecteer de naam in **Huidige gebruikers of groepen** en klik op **Verwijderen**.

6.  Breng in het gedeelte **Verloopbeleid** zo nodig wijzigingen aan in de waarden voor het verstrijken en vernieuwen van inhoudlicenties.

7.  Bewerk de informatie in het gedeelte **Uitgebreid beleid** om de manier te wijzigen waarop inhoudlicenties moeten worden geïmplementeerd. Hierbij gaat het om de persistentie van auteursrechten, het al dan niet ondersteunen van vertrouwde browsers, de persistentie van licenties binnen de inhoud en het verplichte gebruik van toepassingsspecifieke gegevens.

8.  Geef in het gedeelte **Intrekkingsbeleid** op of een intrekkingslijst wordt vereist voor inhoud die wordt gemaakt op basis van deze sjabloon. Als u **Verlang intrekking** selecteert, geeft u de volgende instellingen op:

    -   Typ bij **URL of UNC** de URL van de intrekkingslijst. Als niet-verbonden gebruikers of externe gebruikers moeten worden ondersteund, moet deze URL toegankelijk zijn vanaf het bedrijfsnetwerk en vanaf internet. Zie '[Intrekking implementeren](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)' eerder in dit onderwerp voor meer informatie.
    -   Typ bij **Vernieuwingsinterval intrekkingslijst** het aantal dagen dat de intrekkingslijst geldig blijft. Als een gebruiker een kopie van de intrekkingslijst heeft die ouder is dan deze waarde, moet de gebruiker een bijgewerkte intrekkingslijst ontvangen om de inhoud te kunnen gebruiken.
    -   Typ bij **Openbare-sleutelbestand** het pad en de bestandsnaam van het bestand met de openbare sleutel voor de intrekkingslijst. Zie 'Een handtekening invoegen in een intrekkingslijst' eerder in dit onderwerp voor meer informatie over dit bestand.

    | ![](/security-updates/images/Cc747684.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ga voorzichtig om met de implementatie van intrekkingen. Op basis van het vernieuwingsinterval dat u opgeeft, moet u een intrekkingslijst regelmatig vernieuwen. Anders verloopt de lijst automatisch, waardoor gebruikers geen gebruik kunnen maken van inhoud waarvoor de lijst vereist is. Kies het interval dat u opgeeft voor vernieuwing van de intrekkingslijst zorgvuldig. Zo voorkomt u dat gebruikers onbedoeld geen gebruik kunnen maken van inhoud. Zie '[Intrekking beheren](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)' eerder in dit onderwerp voor meer informatie. |

9.  Klik op **Verzenden**.

Zie '[Sjablonen voor het rechtenbeleid maken en wijzigen](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)' eerder in dit onderwerp voor meer informatie over het uitvoeren van deze procedure.
