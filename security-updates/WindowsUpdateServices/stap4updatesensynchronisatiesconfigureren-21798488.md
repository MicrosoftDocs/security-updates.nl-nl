---
TOCTitle: 'Stap 4: updates en synchronisaties configureren'
Title: 'Stap 4: updates en synchronisaties configureren'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21798488
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Dd939924(v=WS.10)'
---

Stap 4: updates en synchronisaties configureren
===============================================

In deze sectie is beschreven hoe u een reeks updates kunt configureren die u wilt downloaden met Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2).

Procedures voor stap 4
----------------------

U kunt deze procedures uitvoeren met de WSUS-configuratiewizard of de WSUS-beheerconsole.

1.  Informatie over de upstream-server en de proxyserver downloaden en opslaan
2.  De taal van de updates kiezen.
3.  De producten selecteren waarvoor u updates wilt ontvangen.
4.  De updatecategorieën kiezen.
5.  Het synchronisatieschema voor deze server opgeven

Nadat u de netwerkverbinding hebt geconfigureerd, kunt u updates downloaden door de WSUS-server te synchroniseren. De synchronisatie wordt gestart wanneer de WSUS-server verbinding maakt met Microsoft Update. Nadat er een verbinding tot stand is gebracht, controleert WSUS of er nieuwe updates zijn toegevoegd sinds de laatste keer dat er een synchronisatie is uitgevoerd. Wanneer u de WSUS-server voor de eerste keer synchroniseert, zijn alle updates beschikbaar. U kunt deze goedkeuren voor installatiedoeleinden. De eerste synchronisatie neemt mogelijk een lange tijd in beslag.

De procedures in deze sectie beschrijven een synchronisatie met de standaardinstellingen. WSUS 3.0 SP2 omvat tevens opties die u in staat stellen om het bandbreedtegebruik tijdens synchronisatiebewerkingen te minimaliseren.

Als u de Wizard Windows Server Update Services configureren gebruikt
--------------------------------------------------------------------

Tijdens de procedures voor stap 3 hebt u het configureren van de upstream-server en de proxyserver voltooid. De volgende reeks procedures start op de pagina **Verbinding maken met upstream-server** van de desbetreffende configuratiewizard.

**Informatie over de upstream-server en de proxyserver downloaden en opslaan**
1.  Klik op de pagina Verbinding maken met upstream-server van de configuratiewizard op de knop **Verbinding maken**. Hierdoor slaat u uw instellingen op en uploadt u deze, waarna er informatie over beschikbare updates wordt verzameld.

2.  Terwijl de verbinding tot stand wordt gebracht, is de knop **Verbinding verbreken** beschikbaar. Als er problemen zijn met de verbinding, klikt u op **Verbinding verbreken**, lost u de problemen op en maakt u opnieuw verbinding.

3.  Klik op **Volgende** nadat het downloaden is voltooid.

**Talen voor updates kiezen**
1.  Op de pagina Talen kiezen kunt u instellen dat u updates wilt ontvangen voor alle talen of voor een subset van talen. Als u ervoor kiest om updates voor een subset van talen te ontvangen, bespaart u schijfruimte. Het is echter belangrijk dat u alle talen kiest die nodig zijn voor alle clients van deze WSUS-server.

    Selecteer **Alleen updates in deze talen downloaden** en selecteer de talen waarvoor u updates wilt ontvangen als u ervoor kiest om alleen updates in specifieke talen te ontvangen.

2.  Klik op **Volgende**.

**Producten voor updates kiezen**
1.  Op de pagina Producten kiezen kunt u de producten selecteren waarvoor u updates wilt ontvangen. Selecteer productcategorieën, zoals Windows of specifieke producten, zoals Windows Server 2008. Als u een productcategorie selecteert, worden alle producten in de desbetreffende categorie geselecteerd.

2.  Klik op **Volgende**.

**Updatecategorieën kiezen**
1.  Op de pagina Categorieën kiezen kunt u de updatecategorieën selecteren die u wilt ophalen. Kies alle categorieën of een subset categorieën.

2.  Klik op **Volgende**.

**Het synchronisatieschema configureren**
1.  Kies op de pagina Synchronisatieschema of u synchronisatiebewerkingen handmatig of automatisch wilt uitvoeren.

    Als u **Handmatig synchroniseren** kiest, moet u het synchronisatieproces starten via de WSUS-beheerconsole.

    Als u **Automatisch synchroniseren** kiest, wordt de WSUS-server op basis van ingestelde intervallen gesynchroniseerd. Stel een tijdstip in voor **Eerste synchronisatie** en geeft bij **Synchronisaties per dag** het aantal synchronisaties op dat u door deze server wilt laten uitvoeren. Wanneer u bijvoorbeeld instelt dat er vier synchronisaties per dag plaatsvinden, waarbij de eerste synchronisatie om 03:00 uur wordt gestart, worden de synchronisaties uitgevoerd om 03:00 uur, 09:00 uur, 15:00 uur en 21:00 uur.

2.  Klik op **Volgende**.

3.  U kunt op de pagina Voltooid de WSUS-beheerconsole starten door het selectievakje **De invoegtoepassing voor beheer van Windows Server Update Services starten** ingeschakeld te laten en u kunt de eerste synchronisatie starten door het selectievakje **Initiële synchronisatie starten** ingeschakeld te laten.

4.  Klik op **Voltooien**.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th><img src="images/Dd939924.Important(WS.10).gif" />Belangrijk</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">U kunt geen configuratiewijzigingen opslaan die worden aangebracht terwijl de server bezig is met synchroniseren. Wacht tot de synchronisatie is voltooid en breng vervolgens de gewenste wijzigingen aan.
    </td>
    </tr>
    </tbody>
    </table>
 

Als u de WSUS-beheerconsole gebruikt
------------------------------------

In de volgende procedures wordt uitgelegd hoe u de configuratiestappen kunt uitvoeren via de WSUS-beheerconsole.

**Producten en updatecategorieën kiezen**
1.  Klik in het paneel **Opties** op **Producten en categorieën**. Er wordt een dialoogvenster weergegeven met de tabbladen **Producten** en **Categorieën**.

2.  Selecteer op het tabblad **Producten** de productcategorie of specifieke producten waarvoor deze server updates moet ontvangen of selecteer **Alle producten**.

3.  Selecteer op het tabblad **Categorieën** de gewenste updatecategorieën, of selecteer **Alle categorieën**.

4.  Klik op **OK** om uw selecties op te slaan.

**Updatebestanden en talen kiezen**
1.  Klik in het paneel **Opties** op **Updatebestanden en -talen**. Er wordt een dialoogvenster weergegeven met de tabbladen **Updatebestanden** en **Talen van update**.

2.  Kies de optie **Updatebestanden lokaal op de server opslaan** op het tabblad **Updatebestanden** of stel in dat alle clientcomputers updates moeten installeren vanaf Microsoft Update. Als u besluit om updatebestanden op deze server op te slaan, kunt u tevens aangeven of alleen de updates moeten worden gedownload die zijn goedgekeurd of dat bestanden voor snelle installatie moeten worden gedownload.

3.  Kies op het tabblad **Talen van update** de optie **Updates in alle talen downloaden, inclusief nieuwe talen** (de standaardinstelling) of de optie **Updates alleen in deze talen downloaden** als u de updatebestanden lokaal opslaat. Als aan deze WSUS-server downstream-servers zijn verbonden, halen deze downstream-servers alleen updates op in de talen die door de upstream-server zijn opgegeven.

4.  Klik op **OK** om deze instellingen op te slaan.

**De WSUS-server synchroniseren**
1.  Klik in het paneel **Opties** op **Synchronisatieschema**.

2.  Kies op de pagina **Synchronisatieschema** of u synchronisatiebewerkingen handmatig of automatisch wilt uitvoeren.

    Als u **Handmatig synchroniseren** kiest, moet u het synchronisatieproces starten via de WSUS-beheerconsole.

    Als u **Automatisch synchroniseren** kiest, wordt de WSUS-server op basis van ingestelde intervallen gesynchroniseerd. Stel een tijdstip in voor **Eerste synchronisatie** en geeft bij **Synchronisaties per dag** het aantal synchronisaties op dat u door deze server wilt laten uitvoeren. Wanneer u bijvoorbeeld instelt dat er vier synchronisaties per dag plaatsvinden, waarbij de eerste synchronisatie om 03:00 uur wordt gestart, worden de synchronisaties uitgevoerd om 03:00 uur, 09:00 uur, 15:00 uur en 21:00 uur.

3.  Klik op **OK** om uw selecties op te slaan.

4.  Selecteer **Synchronisaties** in het navigatievenster van de WSUS-beheerconsole.

5.  Klik met de rechtermuisknop of ga naar het deelvenster **Acties** dat rechts wordt weergegeven en klik op **Nu synchroniseren**.

    Als het deelvenster **Acties** niet rechts in de console wordt weergegeven, klikt u op de werkbalk van de console op **Beeld**, klikt u op **Aanpassen** en zorgt u ervoor dat het selectievakje **Actiedeelvenster** is ingeschakeld.

6.  Klik nadat de synchronisatie is voltooid in het linkerdeelvenster op **Updates** om de lijst met updates weer te geven.

Volgende stap
-------------

[Stap 5: clientupdates configureren](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a).

Aanvullende bronnen
-------------------

[Stapsgewijze handleiding voor Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
