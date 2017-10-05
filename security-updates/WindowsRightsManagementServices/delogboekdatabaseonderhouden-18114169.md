---
TOCTitle: De logboekdatabase onderhouden
Title: De logboekdatabase onderhouden
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18114169
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747691(v=WS.10)'
---

De logboekdatabase onderhouden
==============================

De logboekvermeldingen zijn onder andere ook de kopieën van de licenties die voor diverse RMS-bewerkingen zijn uitgegeven, zoals het inschrijven van gebruikers en het toewijzen van gebruikslicenties. In het slechts denkbare scenario, waarin elke logboekvermelding een ingeschreven gebruiker of een geslaagde poging om een gebruikslicentie op te halen is, wordt bij elke logboekvermelding de logboekdatabase ongeveer 200 kB groter.

Stel dat een door RMS beveiligd e-mailbericht wordt gestuurd naar alle 50.000 werknemers van een bedrijf en iedere werknemer leest dat e-mailbericht. Als dit e-mailbericht door alle werknemers op dezelfde dag wordt gelezen, wordt de logboekdatabase 10 GB groter. De listener-service kan zodanig worden geconfigureerd dat de eigenlijke XrML-gegevens niet worden geregistreerd, waardoor er aanzienlijk minder gegevens worden vastgelegd.

U zou scripts kunnen maken waarmee oudere gegevens worden gearchiveerd vanuit de logboekdatabase naar een andere database. Voorbeelden van logboekscripts kunt u vinden in de RMS Toolkit, die gratis kan worden gedownload van de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=26724) (http://go.microsoft.com/fwlink/?LinkId=26724).

Variabelen die van invloed zijn op de grootte van de logboekdatabase
--------------------------------------------------------------------

Het inschatten van de grootte van een logboekdatabase hangt af van uw omgeving. Voor het logboek kunnen een aantal "beginvermeldingen" worden ingeschat, zoals:

-   De inschrijving van de RMS-server
-   De inschrijving van gebruikers (een unieke aanvraag voor elke computer die door iedere gebruiker wordt gebruikt)
-   Automatische aanvragen van gebruikers voor off line uitgiftecertificaten

Het grootste aantal vermeldingen in de logboekdatabase na de eerste beginvermeldingen is het gevolg van de gebruikslicenties voor beveiligde inhoud. De grootte van deze database hangt van een aantal voorwaarden af:

-   Steeds een nieuwe licentie wanneer een gebruiker beveiligde inhoud benadert. Dit is niet de standaardmethode voor beveiligde documenten, maar is een mogelijke optie. Als u deze vereiste implementeert, zal de database snel groter worden.
-   Het verwachte aantal beveiligde e-mailberichten dat elke dag naar iedere persoon wordt gestuurd.
-   Het verwachte aantal unieke gebruikers dat deze beveiligde e-mailberichten zal lezen.
-   Het verwachte aantal beveiligde Microsoft Office 2003-documenten (Word, PowerPoint en Excel) dat elke dag door iedere gebruiker zal worden gemaakt.
-   Het verwachte aantal ontvangers van de beveiligde documenten.

De logboekdatabase zal in eerste instantie 1,7 MB groot zijn, inclusief de aanvraag voor een certificaat door de RMS-server. Elke keer wanneer er een nieuwe gebruiker wordt ingeschreven, krijgt deze gebruiker een rechtenaccountcertificaat (RAC) en een clientlicentieverleningscertificaat (CLC). Deze twee acties worden in de logboekdatabase geregistreerd, die daardoor 0,06 MB groter wordt. Bij elke geslaagde aanvraag van een gebruiker voor een licentie voor beveiligde inhoud wordt de database 0,19 MB groter.

Aan de hand van een voorbeeld van een bedrijf met 5000 werknemers die allemaal RMS gebruiken, kunt u zien hoe dit in de praktijk werkt. Iedere gebruiker heeft één computer en in de organisatie worden twee RMS-servers gebruikt. Na de implementatie maakt iedere gebruiker gemiddeld één door RMS beveiligd e-mailbericht per dag dat naar vijf andere gebruikers wordt gestuurd. Iedere gebruiker maakt per dag ook één door RMS beveiligd document dat door drie andere gebruikers wordt geopend. In de volgende tabel ziet u wat de gevolgen van al deze activiteiten voor de logboekdatabase zijn.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Handeling</th>
<th style="border:1px solid black;" >Toename van logboek</th>
<th style="border:1px solid black;" >Cumulatieve grootte van logboek</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">De RMS-server is ingericht</td>
<td style="border:1px solid black;">1,7 MB</td>
<td style="border:1px solid black;">1,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">5000 ingeschreven werknemers (5000*0,06)</td>
<td style="border:1px solid black;">300 MB</td>
<td style="border:1px solid black;">301,7 MB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beveiligde e-mailberichten die worden geopend (25000*0,19)</td>
<td style="border:1px solid black;">4750 MB</td>
<td style="border:1px solid black;">5051,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Beveiligde documenten die worden geopend (15000*0,19)</td>
<td style="border:1px solid black;">2850 MB</td>
<td style="border:1px solid black;">7901,7 MB</td>
</tr>
</tbody>
</table>
  
Na de inschrijving is de logboekdatabase ongeveer 300 MB groot. In dit voorbeeld wordt de database elke dag 7,6 GB groter, wat dicht bij de limiet van 8 GB van de standaardinstallatie van Message Queuing is. Als de logboekdatabase langer dan een dag niet beschikbaar is, gaan er logboekvermeldingen verloren.
  
De grootte van de logboekdatabase beheren  
-----------------------------------------
  
Uw implementatieschema moet een methode voor het beheren van de logboekdatabase bevatten. Doorgaans worden dan de volgende procedures gevolgd.
  
-   **Verwijderen en archiveren**  
    Bij deze methode worden SQL Server-scripts gebruikt voor het archiveren van geselecteerde gegevens vanuit de logboekdatabase naar een andere database wanneer de logboekvermeldingen een bepaalde 'leeftijd' bereiken. Ook wordt hierbij de database gefilterd op gegevens die niet van belang zijn, zodat er geen ruimte wordt verspild.  
-   **Beperken van de gegevens die worden geregistreerd**  
    De logboekdatabase bestaat uit drie hoofdtabellen. Een van deze tabellen is **DRMS\_Log\_Filter**, waarin wordt aangegeven welk veld in de hoofdtabel moet worden geregistreerd wanneer het filteren van het logboek is ingeschakeld.  
    Met de aan/uit-opties in de tabel wordt bepaald welke velden in de hoofdtabel door de logboekregistratie-listener op de RMS-server worden geregistreerd. Twee van deze velden (gerelateerd aan XrML) zijn reeds ingesteld op 0 om het registreren uit te schakelen, omdat deze twee velden verantwoordelijk zijn voor 99% van de grootte van elke rij voor licentieaanvraag.  
    Een andere tabel in de database **DRMS\_Config\_ServerName\_Port**, genaamd **DRMS\_ClusterPolicies**, bevat een **PolicyNameLoggingFiltering**. **LoggingFiltering** is niet standaard ingeschakeld. Als u **LoggingFiltering** op 1 instelt en de logboekregistratie-listener opnieuw start, wordt de database uit het voorbeeld elke dag niet 7,6 GB maar ongeveer 160 MB groter.  
-   **De logboekdatabase verplaatsen**  
    Een andere optie om de grootte van de logboekdatabase beheersbaar te houden, is het verplaatsen van de logboekdatabase naar een server met meer schijfruimte. De logboekdatabase kan op een andere databaseserver dan de configuratiedatabase staan. U verplaatst de database als volgt naar een andere server:  
    1.  Stop de logboekregistratie-listener op elke RMS-server.  
    2.  Kopieer de database naar de andere server of maak een nieuwe database op die server.  
    3.  Selecteer in de RMS-database **DRMS\_Config\_ServerName\_Port** de tabel **DRMS\_ClusterPolicies** en bewerk de waarden voor **LoggingDatabaseName** (naam van de databaseserver) en **LoggingDatabaseServer** (naam van de database).  
    4.  Start IIS opnieuw door IISRESET.exe vanaf de opdrachtregel uit te voeren.
