---
TOCTitle: 'Stap 7: Updates goedkeuren en implementeren'
Title: 'Stap 7: Updates goedkeuren en implementeren'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18126768
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720504(v=WS.10)'
---

Stap 7: Updates goedkeuren en implementeren
===========================================

In deze stap keurt u een update goed voor alle testclientcomputers in de groep Test. Computers in de groep zullen zich in de komende 24 uur melden bij de WSUS-server. Na deze periode kunt u de rapportfunctie van WSUS gebruiken om na te gaan of de update op de computers is geïnstalleerd. Als uit de test blijkt dat de update geen problemen oplevert, kunt u dezelfde update voor installatie goedkeuren voor de rest van de computers in uw organisatie.

Stap 7 omvat de volgende procedures:

-   Een update goedkeuren en implementeren
-   Het rapport Status van updates bekijken

**Een update goedkeuren en implementeren**
1.  Klik op **Updates** op de werkbalk van de WSUS-console. De lijst met updates is standaard zodanig gefilterd dat alleen de essentiële updates en beveiligingsupdates die voor detectie op clientcomputers zijn goedgekeurd, worden weergegeven. Gebruik het standaardfilter voor deze procedure.

2.  Selecteer in de lijst met updates de updates die u voor installatie wilt goedkeuren. Op het tabblad **Details** is informatie over een geselecteerde update beschikbaar. Als u in de lijst meerdere aangrenzende updates wilt selecteren, houdt u SHIFT ingedrukt terwijl u de updates selecteert. Als u meerdere updates wilt selecteren die niet aan elkaar grenzen, houdt u CTRL ingedrukt terwijl u updates selecteert.

3.  Klik onder **Taken voor updates** op **Goedkeuringsstatus wijzigen**. Het dialoogvenster **Updates goedkeuren** wordt weergegeven.

4.  Klik in de lijst **Groepsinstellingen voor goedkeuring voor de geselecteerde updates** op **Installeren** in de kolom **Goedkeuring** voor de groep Test en klik vervolgens op **OK**.

| ![](images/Cc720504.note(WS.10).gif)Opmerking                                                                                                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voor het goedkeuren van updates kunt u vele opties instellen. U kunt bijvoorbeeld deadlines instellen of de installatie van updates ongedaan maken. Deze opties worden besproken in het Engelstalige document 'Microsoft Windows Server Update Services Operations Guide'. |

Na een periode van 24 uur kunt u de rapportfunctie van WSUS gebruiken om na te gaan of de updates op de computers zijn geïnstalleerd.

**Het rapport Status van updates bekijken**
1.  Klik op **Rapporten** op de werkbalk van de WSUS-console.

2.  Klik op de pagina **Rapporten** op **Status van updates**.

3.  Als u de lijst met updates wilt filteren, selecteert u onder **Weergeven** de criteria die u wilt gebruiken om de lijst te filteren, en klikt u vervolgens op **Toepassen**.

4.  Als u de status van een update per computergroep en vervolgens per computer wilt weergeven, vouwt u de weergave van de update waar nodig uit.

5.  Als u het rapport Status van updates wilt afdrukken, klikt u onder **Taken** op **Rapport afdrukken**.

Als de updates zonder problemen op de computers uit de groep Test zijn geïnstalleerd, kunt u dezelfde updates goedkeuren voor installatie voor de rest van de computers in uw organisatie.
