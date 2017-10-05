---
TOCTitle: 'Een bestaande implementatie bijwerken met RMS Service Pack 1 (SP1)'
Title: 'Een bestaande implementatie bijwerken met RMS Service Pack 1 (SP1)'
ms:assetid: 'a562c4b0-15df-46db-9d61-24db74871cfa'
ms:contentKeyID: 18114117
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747714(v=WS.10)'
---

Een bestaande implementatie bijwerken met RMS Service Pack 1 (SP1)
==================================================================

Deze sectie bevat informatie die u kan helpen bij het installeren van Microsoft® Windows® Rights Management Services (RMS) Service Pack 1 (SP1) in een organisatie met een bestaande RMS-implementatie. Alleen organisaties die al RMS hebben geïmplementeerd moeten hun implementatie bijwerken met RMS SP1. Organisaties die RMS voor het eerst implementeren, kunnen RMS met SP1 implementeren door de aanwijzingen te volgen in Een RMS-implementatie plannen en Een RMS-systeem implementeren in deze documentatie.

U kunt RMS SP1 installeren zonder de bestaande RMS-installatie te verwijderen. Het installatieprogramma van RMS SP1 detecteert dat RMS is geïnstalleerd en voegt de vereiste extra functies en instellingen toe.

**In dit onderwerp**

-   [De RMS SP1-update voorbereiden](#bkmk_1)
-   [De RMS SP1-update uitvoeren](#bkmk_2)
-   [Clusters bijwerken](#bkmk_3)
-   [RMS-clients bijwerken](#bkmk_4)
-   [Interoperabiliteit met RMS versie 1.0](#bkmk_5)
-   [RMS met SP1 verwijderen](#bkmk_6)

<span id="BKMK_1"></span>
De RMS SP1-update voorbereiden
------------------------------

De RMS SP1-update is zo ontworpen dat u RMS zonder onderbreking kunt blijven uitvoeren. Het is echter raadzaam het volgende te doen voordat u een update uitvoert van de RMS-servers:

-   Maak een back-up van de configuratiedatabase en de persoonlijke sleutel van de RMS-server. Zie "Systeemback-ups maken voor RMS" in de sectie "Een RMS-implementatie plannen" in deze documentatie voor meer informatie.
-   Zorg ervoor dat u over het wachtwoord beschikt voor de persoonlijke RMS-sleutel
-   Maak een back-up van de logboekdatabase als u eerder vastgelegde statistische gegevens wilt behouden.
-   Zorg ervoor dat u over de laatste essentiële updates en beveiligingsupdates beschikt voor het besturingssysteem dat is geïnstalleerd op de clients en servers. Als u wilt controleren of u over alle essentiële updates en beveiligingsupdates beschikt, klikt u op **Start**, klikt u op **Windows Update** en volgt u de aanwijzingen op het scherm.

<span id="BKMK_2"></span>
De RMS SP1-update uitvoeren
---------------------------

Wanneer de wizard Setup van RMS SP1 een RMS-installatie detecteert, worden uitsluitend nieuwe bestanden toegevoegd of bestanden vervangen als dat nodig is voor RMS SP1. Als u al met succes RMS uitvoert, is het niet nodig het systeem opnieuw in te richten of een aanvullende configuratie uit te voeren na het installeren van RMS SP1 om door te gaan met uitvoeren van RMS.

<span id="BKMK_3"></span>
Clusters updaten
----------------

Als u RMS hebt geïnstalleerd in een clusterconfiguratie, moet u een plan maken voor het bijwerken van de clusters om de het effect van de update op de installatie te minimaliseren. Houd rekening met de volgende aanbevelingen bij het bepalen van de beste manier om RMS SP1 te implementeren in uw organisatie:

-   Aanbevolen wordt RMS SP1 telkens op een gedeelte van een cluster te installeren. Daardoor wordt het uitvoeren van een upgrade van de cluster beter voorspelbaar en bestaat er minder kans op een verslechtering van de service tijdens de upgrade.
-   Als u over meerdere RMS-clusters beschikt, moet u eerst een upgrade uitvoeren van de basiscertificeringsclusters en vervolgens een upgrade van de subingeschreven licentieclusters.
-   Als u gebruikmaakt van groepsuitbreiding naar andere forests, kunt u onafhankelijk van elkaar een upgrade uitvoeren van de clusters in de forests zonder de mogelijkheid van de RMS-servers te beperken om het groepslidmaatschap uit te breiden naar andere forests.
-   RMS SP1- en RMS versie 1.0-server kunnen naast elkaar bestaan en samenwerken.
-   Het RMS SP1-installatiepakket kan ook worden gebruikt om een nieuwe versie van RMS SP1 te installeren op een server. Daarvoor is het niet nodig dat RMS versie 1.0 is geïnstalleerd.

<span id="BKMK_4"></span>
RMS-clients bijwerken
---------------------

RMS met SP1 bevat een nieuwe RMS-client. Het installatiepakket voor RMS SP1-client kan ook worden gebruikt om een nieuwe versie van de RMS SP1-client op een computer te installeren. Daarvoor is het niet nodig dat de RMS versie 1.0-client is geïnstalleerd. De RMS SP1-client bevat een functie voor achterwaartse compatibiliteit zodat de client kan worden gebruikt voor toepassingen met RMS-ondersteuning waarvoor RMS versie 1.0 is vereist.

Deze nieuwe RMS-client ondersteunt de volgende functies:

-   De client hoeft niet langer via internet verbinding te maken met Microsoft en een lockbox te downloaden.
-   Als u RMS-client installeert met SMS of Groepsbeleid, zijn voor de installatie geen beheerdersbevoegdheden vereist.
-   De RMS SP1-client bevat een nieuwe server-lockbox (ook wel server security processor genoemd) die kan worden gebruikt om RMS-ondersteuning door webservices of serverzijdetoepassingen te realiseren, bijvoorbeeld Windows SharePoint® Services en Exchange Server 2003, zodat de service in staat is door RMS beveiligde inhoud te gebruiken en te herdistribueren. De lockbox is ontworpen voor het leveren van maximale prestaties en schaalbaarheid bij gebruik in vertrouwde servertoepassingen
-   RMS-client werkt met FIPS 140-2 gecertificeerde cryptografische algoritmen. Daardoor kan de client worden geïmplementeerd in een FIPS-compatibele organisatie.

<span id="BKMK_5"></span>
Interoperabiliteit met RMS versie 1.0
-------------------------------------

Omdat RMS SP1 vele verbeteringen bevat en grotere prestaties levert, raden we u aan het te installeren nadat u het testen hebt afgerond. Hoewel RMS-servers en -clients die RMS SP1 uitvoeren volledig interoperabel zijn met RMS-servers en -clients die RMS SP1 niet uitvoeren, moet u zich bewust zijn van de volgende verschillen in de manier waarop zij functioneren in een gemengde omgeving:

-   Uitsluitend servers die RMS SP1 uitvoeren zijn in staat off line-inschrijving te ondersteunen.
-   Alleen clients die RMS SP1 uitvoeren zijn zelfactiverend.
-   De volgende tabel bevat een overzicht van de ondersteunde functionaliteit voor gemengde omgevingen:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>RMS Server-versie</th>
<th>Ondersteunde functies met v1-clients</th>
<th>Ondersteunde functies met SP1-clients</th>
<th>Ondersteunde functies in gemengde (v1 en SP1) client-omgevingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Alle voorgaande functies.
Geen offline-inschrijving van server. Server moet inschrijven via internet.
Geen zelfactiverende clients.</td>
<td style="border:1px solid black;">Alle voorgaande functies.
Geen offline-inschrijving van server.
Zelfactiverende clients.</td>
<td style="border:1px solid black;">Alle voorgaande functies.
SP1-clients zijn zelfactiverend.
Versie 1-clients moeten activeren via internet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP1</td>
<td style="border:1px solid black;">Alle voorgaande functies.
Offline-inschrijving van server.
Geen zelfactiverende clients.</td>
<td style="border:1px solid black;">Alle SP1-functies.
Offline-inschrijving van server.
Zelfactiverende clients.
Server-lockbox.</td>
<td style="border:1px solid black;">Alle voorgaande functies plus SP1-functies.
Offline-inschrijving van server.
SP1-clients zijn zelfactiverend.
Versie 1-clients moeten activeren via internet.</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_6"></span>
RMS met SP1 verwijderen
-----------------------

Als u de RMS-server wilt herstellen naar de vorige configuratie nadat u RMS SP1 hebt geïnstalleerd, kunt u **Software** gebruiken in **Configuratiescherm** om RMS SP1 te verwijderen.

**Opmerking**   Als u voorafgaand aan de installatie van RMS SP1 een back-up hebt gemaakt van de configuratiedatabase, kunt u die herstellen om alle wijzigingen die zijn aangebracht door RMS SP1 volledig teniet te doen. Als u geen back-up hebt genaakt van de configuratiedatabase, kunt u mogelijk de configuratiedatabase van de RMS SP1-installatie gebruiken voor de herstelde RMS-installatie. De herstelde RMS-installatie negeert de extra velden die de RMS SP1-installatie aan de configuratiedatabase heeft toegevoegd. De herstelde RMS-installatie maakt geen gebruik van die velden.
