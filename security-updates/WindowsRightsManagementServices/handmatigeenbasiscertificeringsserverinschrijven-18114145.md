---
TOCTitle: Handmatig een basiscertificeringsserver inschrijven
Title: Handmatig een basiscertificeringsserver inschrijven
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18114145
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747727(v=WS.10)'
---

Handmatig een basiscertificeringsserver inschrijven
===================================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste Uitvoeren als gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Maakt u gebruik van het off line inschrijvingsproces, dan dient u ervoor te zorgen dat RMS-clients niet voordat de inschrijving is voltooid proberen voor licenties verbinding te maken met de RMS-server. Als een client probeert verbinding te maken met een RMS-server die niet is ingeschreven, doet er zich een fout voor met de webservices waardoor clients deze niet kunnen gebruiken. Weet u niet zeker of clients niet zullen proberen verbinding te maken met de RMS-server, dan kunt u het beste IIS na de inschrijvingsprocedure opnieuw instellen, zodat eventueel ontstane fouten worden gecorrigeerd.

Als u de basiscertificeringsserver off line wilt inschrijven en u gebruikt een computer met een sterk beveiligde browserconfiguratie (zoals een computer met Windows Server 2003 of Windows Service Pack 2) om een verbinding te maken met internet en een serverlicentieverleningscertificaat aan te vragen, moet u ervoor zorgen dat de URL van de website van de inschrijvingsservice is toegevoegd aan de zone Vertrouwde websites, zodat u het serverlicentieverleningscertificaat kunt downloaden. Deze URL is https://activation.drm.microsoft.com.

Als u het off line inschrijvingsproces volgt, dient u ervoor te zorgen dat op de computer waarmee u het inschrijvingsverzoek bij de inschrijvingsservice van Microsoft indient de GTE Cyber Trust Root CA als certificeringsinstantie in het certificatenarchief is geïnstalleerd. Deze certificeringsinstantie wordt standaard op Windows Server 2003-computers vertrouwd. Als op de computer een andere Windows-versie actief is, kunt u deze certificeringsinstantie vertrouwen door de nieuwste update van het certificaat via de website Windows Update te downloaden.

Handmatig een basiscertificeringsserver inschrijven
---------------------------------------------------

#### Handmatig een basiscertificeringsserver inschrijven

1.  Na installatie van RMS op een server waarvan u de basiscertificeringsserver wilt maken, dient u de pagina **Algemeen beheer** te openen naast de website waarop u een basisserverlicentieverleningscertificaat wilt installeren. Klik vervolgens op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Clusterbronnen** op **Inschrijven**. Het dialoogvenster **Inschrijven** wordt weergegeven.

3.  Selecteer **Off line** en klik op de knop **Exporteren**. Het dialoogvenster **Bestand downloaden** wordt weergegeven.

4.  Klik op **Opslaan**. Het dialoogvenster **Opslaan als** wordt weergegeven.

    | ![](images/Cc747727.note(WS.10).gif)Opmerking                                                                                                                     |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Klik in het dialoogvenster **Bestand downloaden** NIET op **Openen**. Als u op **Openen** zou klikken, wordt er een foutbericht weergegeven en wordt het inschrijvingsverzoek niet opgeslagen. |

5.  Klik op **Opslaan** om het verzoek naar een bestand te exporteren. Standaard wordt het bestand op het bureaublad opgeslagen onder de naam *Servernaam*EnrollRequest.xml, waarbij de *servernaam* door de naam van uw RMS-server wordt vervangen. U kunt het bestand op een andere locatie opslaan door de gewenste locatie in de vervolgkeuzelijst **Opslaan in** te kiezen. U kunt ook de bestandsnaam wijzigen door een andere naam te typen in het vak **Bestandsnaam**.

6.  Nadat u het verzoek tot inschrijving hebt opgeslagen, wordt het venster **Downloaden voltooid** weergegeven. Als u op **Openen** klikt, wordt de XML-code in het bestand weergegeven, maar maak geen wijzigingen in het bestand. Klik op **Map openen** om de map te openen waarin het bestand wordt opgeslagen. Klik op **Sluiten** als u klaar bent met het bestand en dit op de juiste locatie staat.

7.  Verplaats het aanvraagbestand voor de inschrijving van uw server naar een computer die verbinding met internet kan maken, en ga naar de [website van de inschrijvingsservice]().

8.  Volg de instructies op de website om een serverlicentieverleningscertificaat te verkrijgen.

9.  Verplaats het serverlicentieverleningscertificaat terug naar deze basiscertificeringsserver.

10. Klik in het gedeelte **Clusterbronnen** op **Inschrijven**. Het dialoogvenster **Inschrijven** wordt weergegeven.

11. Klik in het dialoogvenster **Inschrijven** op de knop **Bladeren** en ga naar het serverlicentieverleningscertificaat dat u hebt gedownload. Klik vervolgens op de knop **Importeren**.

12. Klik op **Ja** om te bevestigen dat u dit certificaat wilt importeren.

13. Het gedeelte **Clusterbronnen** wordt bijgewerkt en geeft het serverlicentieverleningscertificaat weer.
