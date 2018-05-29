---
TOCTitle: Een sjabloon voor het rechtenbeleid toevoegen
Title: Een sjabloon voor het rechtenbeleid toevoegen
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18113847
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720206(v=WS.10)'
---

Een sjabloon voor het rechtenbeleid toevoegen
=============================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Een sjabloon voor het rechtenbeleid toevoegen
---------------------------------------------

#### Een sjabloon voor het rechtenbeleid toevoegen

1.  Open de pagina **Algemeen beheer** en klik naast de website waarop u een sjabloon voor het rechtenbeleid wilt toevoegen op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Sjablonen voor het rechtenbeleid**.

3.  Klik bij **Taal** op de taal voor de sjabloon.

4.  Klik op **Een sjabloon voor rechtenbeleid toevoegen**.

5.  Geef in het gedeelte **Sjabloonidentificatie** een naam, een beschrijving en een URL voor het aanvragen van rechten op voor de sjabloon.

6.  Typ in het gedeelte **Gebruikers en groepen** bij **Gebruikers of groepen toevoegen** het geldige e-mailadres van een gebruiker of groep die u wilt toevoegen en klik op **Toevoegen**. Herhaal deze stap om alle gewenste gebruikers en/of groepen toe te voegen.

7.  Selecteer bij **Huidige gebruikers of groepen** het e-mailadres van een gebruiker of groep waaraan u rechten wilt toekennen.

8.  Schakel de selectievakjes in van alle rechten die u aan de geselecteerde gebruiker of groep wilt toekennen. Herhaal deze stap om rechten toe te kennen aan de overige gebruikers en groepen.

9.  Selecteer in het gedeelte **Verloopbeleid** een van de drie verloopopties en geef vervolgens al naar gelang de situatie een verloopdatum of verlooptijd op. Selecteer indien nodig **Gebruikslicenties voor inhoud moeten worden vernieuwd elke:** en geef het aantal dagen tussen de vernieuwingen op.

10. Selecteer in het gedeelte **Uitgebreid beleid** een of meer van de vier opties. Als u **Verplicht gebruik van toepassingsspecifieke gegevens** selecteert, geeft u een naam en waarde op voor de gegevens die verplicht moeten worden gebruikt en klikt u op **Toevoegen**.

11. U kunt intrekking implementeren door in het gedeelte **Intrekkingsbeleid** het selectievakje **Verlang intrekking** in te schakelen en vervolgens de volgende stappen uit te voeren:

    1.  Typ bij **URL of UNC** de URL van de intrekkingslijst. Als niet-verbonden gebruikers of externe gebruikers moeten worden ondersteund, moet deze URL toegankelijk zijn vanaf het bedrijfsnetwerk en vanaf internet.
    2.  Typ bij **Vernieuwingsinterval intrekkingslijst** het aantal dagen dat de intrekkingslijst geldig blijft. Als een gebruiker een kopie van de intrekkingslijst heeft die ouder is dan deze waarde, moet de gebruiker een bijgewerkte intrekkingslijst ontvangen om de inhoud te kunnen gebruiken.
    3.  Typ bij **Bestand met de openbare sleutel** het pad en de bestandsnaam of klik op **Bladeren** om naar het bestand met de openbare sleutel voor de intrekkingslijst te zoeken. Zie 'Een handtekening invoegen in een intrekkingslijst' voor meer informatie over dit bestand.

    | ![](/security-updates/images/Cc720206.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ga voorzichtig om met de implementatie van intrekkingen. Op basis van het vernieuwingsinterval dat u opgeeft, moet u een intrekkingslijst regelmatig vernieuwen. Anders verloopt de lijst automatisch, waardoor gebruikers geen gebruik kunnen maken van inhoud waarvoor de lijst vereist is. Kies het interval dat u opgeeft voor vernieuwing van de intrekkingslijst zorgvuldig. Zo voorkomt u dat gebruikers onbedoeld geen gebruik kunnen maken van inhoud. Zie '[Intrekking beheren](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)' eerder in dit onderwerp voor meer informatie. |

12. Klik op **Verzenden**.

Zie '[Intrekking beheren](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)' eerder in dit onderwerp voor meer informatie over intrekken.

Zie '[Intrekkingsbeleid definiëren](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)' eerder in dit onderwerp voor aandachtspunten bij het opgeven van intrekkingsopties.

Zie '[Sjablonen voor het rechtenbeleid maken en wijzigen](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)' eerder in dit onderwerp voor meer informatie over het uitvoeren van deze procedure.
