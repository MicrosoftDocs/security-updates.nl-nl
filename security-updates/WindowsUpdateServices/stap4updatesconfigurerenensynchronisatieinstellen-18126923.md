---
TOCTitle: 'Stap 4: Updates configureren en synchronisatie instellen'
Title: 'Stap 4: Updates configureren en synchronisatie instellen'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18126923
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708447(v=WS.10)'
---

Stap 4: Updates configureren en synchronisatie instellen
========================================================

Voordat u begint met het downloaden van updates, moet u eerst opgeven welke updates u wilt downloaden. In dit gedeelte wordt beschreven hoe u de gewenste reeks updates kunt configureren.

Deze stap omvat de volgende procedures:

-   Informatie over de upstream-server en de proxyserver downloaden en opslaan
-   De taal van de gewenste updates selecteren
-   De producten selecteren waarvoor u updates wilt ophalen
-   De gewenste updatecategorieën selecteren
-   Het synchronisatieschema voor deze server opgeven

De volgende vijf procedures bevatten de stappen voor het configureren van uw updates met behulp van de configuratiewizard. De daaropvolgende procedures beschrijven hoe u deze configuratie vanuit de WSUS-beheerconsole kunt uitvoeren door bepaalde opties te selecteren.

**Informatie over de upstream-server en de proxyserver downloaden en opslaan**
1.  U moet de configuratie van de upstream-server en de proxyserver hebben voltooid via de configuratiewizard en de pagina **Verbinding maken met upstream-server** moet zijn geopend.

2.  Klik op de knop **Verbinding maken** om uw instellingen op te slaan en te uploaden, en om informatie over beschikbare updates op te halen.

3.  Terwijl de verbinding tot stand wordt gebracht, is de knop **Verbinding verbreken** beschikbaar. Als er problemen zijn met de verbinding, klikt u op **Verbinding verbreken**, lost u de problemen op en maakt u opnieuw verbinding.

4.  Nadat het downloaden is voltooid, klikt u op **Volgende** om naar de pagina **Talen kiezen** te gaan of selecteert u een andere pagina in het linkerdeelvenster.

**Updatetalen kiezen**
1.  Op de pagina **Talen kiezen** kunt u updates voor alle talen of voor een subset talen ophalen. Als u een subset talen selecteert, bespaart dit schijfruimte, maar het is van belang om alle talen te selecteren die voor alle clients van deze WSUS-server vereist zijn.

2.  Als u updates voor slechts enkele talen wilt ophalen, selecteert u **Updates alleen in deze talen downloaden** en selecteert u de talen waarvoor u updates wilt. Klik op **Volgende** om naar de pagina **Producten kiezen** te gaan of selecteer een andere pagina in het linkerdeelvenster.

**Updateproducten kiezen**
1.  Op de pagina **Producten kiezen** kunt u de producten opgeven waarvoor u updates wilt ophalen.

2.  U kunt productcategorieën selecteren, bijvoorbeeld Windows, of specifieke producten opgeven, bijvoorbeeld Windows Server 2003. Als u een productcategorie selecteert, worden alle producten in de categorie geselecteerd. Klik op **Volgende** om naar de pagina **Categorieën kiezen** te gaan of selecteer een andere pagina in het linkerdeelvenster.

**De updatecategorieën kiezen**
1.  Op de pagina **Categorieën kiezen** kunt u de updatecategorieën selecteren die u wilt ophalen. U kunt alle categorieën of een aantal daarvan selecteren.

2.  Klik op **Volgende** om naar de pagina **Synchronisatieschema configureren** te gaan of selecteer een andere pagina in het linkerdeelvenster.

**Het synchronisatieschema configureren**
1.  De pagina **Synchronisatieschema instellen** wordt geopend. Op deze pagina kunt u aangeven of de synchronisatie handmatig of automatisch moet worden uitgevoerd.

2.  Als u ervoor kiest om de synchronisatie op deze server handmatig uit te voeren, moet u de synchronisatieprocedure starten vanuit de WSUS-beheerconsole.

3.  Als u ervoor kiest om de synchronisatie automatisch te laten verlopen, wordt de WSUS-server met een door u opgegeven interval gesynchroniseerd. Geef de tijd op waarop de synchronisatie voor het eerst moet worden uitgevoerd en selecteer het aantal keren per dag dat de server moet worden gesynchroniseerd. Als u bijvoorbeeld opgeeft dat er vier synchronisaties per dag moeten plaatsvinden, beginnend om 3:00 uur 's ochtends, wordt een synchronisatie uitgevoerd om 3:00 uur, 9:00 uur, 15:00 uur en 21:00 uur.

Nadat u de bovenstaande configuratiestappen hebt voltooid, selecteert u de pagina **Voltooid** in de configuratiewizard. U kunt de WSUS-beheerconsole starten door het selectievakje **De invoegtoepassing voor beheer van Windows Server Update Services starten** ingeschakeld te laten en u kunt de eerste synchronisatie starten door het selectievakje **Initiële synchronisatie starten** ingeschakeld te laten.

| ![](images/Cc708447.note(WS.10).gif)Opmerking                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U kunt geen configuratiewijzigingen opslaan die worden aangebracht terwijl de server bezig is met synchroniseren. Wacht totdat de synchronisatie is voltooid voordat u de wijzigingen aanbrengt. |

![](images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

De volgende procedures geven aanwijzingen voor het uitvoeren van de bovenstaande configuratiestappen via de pagina **Opties** van de WSUS-beheerconsole:

-   Producten en categorieën selecteren
-   Bestanden en talen van update

**Producten en categorieën selecteren**
1.  Start de WSUS-beheerconsole: klik op **Start**, wijs achtereenvolgens **Alle programma's** en **Systeembeheer** aan en klik op **Microsoft Windows Server Update Services**.

2.  Selecteer **Opties** onder de WSUS-server in het linkerdeelvenster.

3.  Selecteer **Producten en categorieën** in het middelste deelvenster.

4.  Er wordt een dialoogvenster geopend met twee tabbladen: **Producten** en **Categorieën**.

5.  Selecteer op het tabblad **Producten** de productcategorie of het specifieke product waarvoor deze server updates moet ophalen, of selecteer **Alle producten**.

6.  Selecteer op het tabblad **Categorieën** de gewenste updatecategorieën, of selecteer **Alle categorieën**.

7.  Klik op **OK** om uw selecties op te slaan.

**Bestanden en talen van update**
1.  Selecteer **Updatebestanden en -talen** op de pagina **Opties**.

2.  Er wordt een dialoogvenster geopend met twee tabbladen: **Updatebestanden** en **Talen van update**.

3.  Op het tabblad **Updatebestanden** kunt u aangeven of updatebestanden lokaal moeten worden opgeslagen of dat alle clientcomputers de installatie moeten uitvoeren via Microsoft Update. Als u besluit om updatebestanden op deze server op te slaan, kunt u tevens aangeven of alleen de updates moeten worden gedownload die zijn goedgekeurd of dat bestanden voor snelle installatie moeten worden gedownload.

4.  Op het tabblad **Talen van update** kunt u aangeven of updates voor alle talen moeten worden opgehaald (de standaardinstelling) of dat alleen updates voor de opgegeven talen moeten worden opgehaald. Als aan deze WSUS-server downstream-servers zijn verbonden, halen deze downstream-servers alleen updates op in de talen die door de upstream-server zijn opgegeven.

5.  Klik op **OK** om deze instellingen op te slaan.

Nadat u de netwerkverbinding hebt geconfigureerd, kunt u updates downloaden door de WSUS-server te synchroniseren.

Dit houdt in dat de WSUS-server verbinding moet maken met Microsoft Update. Nadat de verbinding tot stand is gebracht, stelt WSUS vast of er nieuwe updates beschikbaar zijn gesteld sinds de vorige keer dat u de server hebt gesynchroniseerd. Omdat dit de eerste keer is dat u de WSUS-server met Windows Update synchroniseert, zijn alle updates beschikbaar en gereed om door u voor installatie te worden goedgekeurd. De eerste synchronisatie kan redelijk lang duren.

| ![](images/Cc708447.note(WS.10).gif)Opmerking                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| In dit document wordt beschreven hoe u de WSUS-server synchroniseert met de standaardinstellingen, maar WSUS heeft ook opties waarmee u het bandbreedtegebruik tot een minimum kunt beperken tijdens het synchroniseren. |

**De WSUS-server synchroniseren**
1.  Selecteer **Synchronisaties** in de WSUS-beheerconsole.

2.  Klik met de rechtermuisknop of ga naar het deelvenster **Acties** rechts in de console en klik op **Nu synchroniseren**.

| ![](images/Cc708447.note(WS.10).gif)Opmerking                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als het deelvenster **Acties** niet rechts in de console wordt weergegeven, klikt u op de werkbalk van de console op **Beeld**, klikt u op **Aanpassen** en zorgt u ervoor dat het selectievakje **Actiedeelvenster** is ingeschakeld. |

Nadat het synchroniseren is voltooid, klikt u op de **Updates** in het linkerdeelvenster om de lijst met updates weer te geven.
