---
TOCTitle: 'Een bestaande implementatie bijwerken met RMS Service Pack 2 (SP2)'
Title: 'Een bestaande implementatie bijwerken met RMS Service Pack 2 (SP2)'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18114030
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720225(v=WS.10)'
---

Een bestaande implementatie bijwerken met RMS Service Pack 2 (SP2)
==================================================================

Deze sectie bevat informatie die u kan helpen bij het inschakelen van Microsoft® Windows® Rights Management Services (RMS) met Service Pack 2 (SP2) in een organisatie met een bestaande RMS-implementatie. Alleen organisaties die al RMS hebben geïmplementeerd moeten hun implementatie bijwerken met RMS met SP2. Organisaties die voor het eerst RMS implementeren kunnen RMS met SP2 implementeren door de aanwijzingen te volgen in Een RMS-implementatie plannen ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) en Een RMS-systeem implementeren ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) in deze documentatie.

U kunt RMS met SP2 installeren zonder de bestaande installatie van RMS met SP1 te verwijderen. Het installatieprogramma van RMS met SP2 detecteert dat RMS met SP1 is geïnstalleerd en voegt de vereiste extra functies en instellingen toe.

| ![](/security-updates/images/Cc720225.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Er is geen ondersteuning voor een upgradepad van RMS-server zonder servicepack naar RMS met SP2. Als u werkt met RMS-server zonder servicepack, moet u een upgrade uitvoeren naar RMS met SP1 voordat u een upgrade kunt uitvoeren naar RMS met SP2. Het uitvoeren van een upgrade van de RMS-client is mogelijk vanaf elke voorgaande versie van de RMS-client. |

**In dit onderwerp**

-   [De RMS met SP2-update voorbereiden](#bkmk_preparingforsp2update)
-   [De RMS met SP2-update uitvoeren](#bkmk_performingsp2update)
-   [Clusters bijwerken](#bkmk_updateclusters)
-   [RMS-clients bijwerken](#bkmk_updateclients)
-   [Interoperabiliteit met RMS versie 1.0](#bkmk_interop)
-   [RMS met SP2 verwijderen](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
De RMS met SP2-update voorbereiden
----------------------------------

De RMS met SP2-update is zo ontworpen dat u RMS zonder onderbreking kunt blijven uitvoeren. Het is echter raadzaam het volgende te doen voordat u een update uitvoert van de RMS-cluster:

-   Maak een back-up van de configuratiedatabase en de persoonlijke sleutel van de RMS-server. Zie Systeemback-ups maken voor RMS ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) in deze documentatie.
-   Als u een op software gebaseerde persoonlijke sleutel gebruikt, zorg er dan voor dat u over het wachtwoord beschikt voor die persoonlijke RMS-sleutel.
-   Maak een back-up van de logboekdatabase als u eerder vastgelegde statistische gegevens wilt behouden.
-   Zorg ervoor dat u over de laatste essentiële updates en beveiligingsupdates beschikt voor het besturingssysteem dat is geïnstalleerd op de clients en servers. Als u wilt controleren of u over alle essentiële updates en beveiligingsupdates beschikt, klikt u op **Start**, klikt u op **Windows Update** en volgt u de aanwijzingen op het scherm.

<span id="bkmk_PerformingSP2Update"></span>
De RMS met SP2-update uitvoeren
-------------------------------

Wanneer de wizard Setup van Windows Rights Management Services met Service Pack 2 een RMS-installatie detecteert, wordt de huidige RMS-installatie met SP1 geanalyseerd en worden uitsluitend nieuwe bestanden toegevoegd en/of worden bestanden vervangen als dat nodig is voor RMS met SP2. Als u al met succes RMS uitvoert, is het niet nodig het systeem opnieuw in te richten of een aanvullende configuratie uit te voeren na het installeren van RMS met SP2 om door te gaan met uitvoeren van RMS.

<span id="bkmk_UpdateClusters"></span>
Clusters bijwerken
------------------

Als u RMS hebt geïnstalleerd in een clusterconfiguratie, moet u een plan maken voor het bijwerken van de clusters om het effect van de update op de installatie te minimaliseren. Houd rekening met de volgende aanbevelingen bij het bepalen van de beste manier om RMS met SP2 te implementeren in uw organisatie:

-   Aanbevolen wordt RMS met SP2 telkens op een gedeelte van een cluster te installeren. Daardoor wordt het uitvoeren van een upgrade van de cluster beter voorspelbaar en bestaat er minder kans op een verslechtering van de service tijdens de upgrade.
-   Als u over meerdere RMS-clusters beschikt, moet u eerst een upgrade uitvoeren van de basiscertificeringsclusters en vervolgens een upgrade van de subingeschreven licentieclusters.
-   Als u gebruikmaakt van groepsuitbreiding naar andere forests, kunt u onafhankelijk van elkaar een upgrade uitvoeren van de clusters in de forests zonder de mogelijkheid van de RMS-servers te beïnvloeden om het groepslidmaatschap uit te breiden naar andere forests.
-   RMS met SP2, RMS met SP1 en RMS-server versie 1.0 kunnen uitsluitend naast elkaar bestaan en samenwerken als zij zich in verschillende Active Directory-forests bevinden. Het wordt afgeraden te werken met verschillende versies van RMS-server in dezelfde cluster.
-   Het RMS met SP2-installatiepakket kan ook worden gebruikt om een nieuwe implementatie van RMS met SP2 te installeren op een server. Daarvoor is het niet nodig dat RMS met SP1 is geïnstalleerd.

<span id="bkmk_UpdateClients"></span>
RMS-clients bijwerken
---------------------

De nieuwe RMS met SP2-client is beschikbaar op Windows Update en het Microsoft Downloadcentrum. Het installatiepakket voor de RMS met SP2-client kan ook worden gebruikt om een nieuwe versie van de RMS met SP2-client op een computer te installeren. Daarvoor is het niet nodig dat de RMS versie 1.0-client is geïnstalleerd. De RMS met SP2-client bevat een functie voor achterwaartse compatibiliteit zodat de client kan worden gebruikt voor toepassingen met RMS-ondersteuning waarvoor RMS versie 1.0 is vereist.

Zie De RMS-client distribueren ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)) voor meer informatie over het bijwerken en installeren van de RMS-client.

<span id="bkmk_InterOp"></span>
Interoperabiliteit met RMS versie 1.0
-------------------------------------

We raden u aan RMS met SP2 gedurende de volgende upgrade-ronde te installeren omdat het vele verbeteringen bevat en betere prestaties levert. Hoewel RMS-servers en -clients die RMS met SP2 uitvoeren volledig interoperabel zijn met RMS-servers en -clients die RMS met SP2 niet uitvoeren, moet u zich bewust zijn van de volgende verschillen in de manier waarop zij functioneren in een gemengde omgeving:

-   Uitsluitend servers die RMS met SP1 of later uitvoeren zijn in staat offline-inschrijving te ondersteunen.
-   Uitsluitend clients die RMS met SP1 of later uitvoeren zijn zelfactiverend.
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
<th style="border:1px solid black;" >RMS Server-versie</th>
<th style="border:1px solid black;" >Ondersteunde functies met versie 1-clients</th>
<th style="border:1px solid black;" >Ondersteunde functies met SP2-clients</th>
<th style="border:1px solid black;" >Ondersteunde functies in omgevingen met gemengde clients</th>
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
SP2-clients zijn zelfactiverend.
Versie 1-clients moeten activeren via internet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Alle voorgaande functies.
Offline-inschrijving van server.
Geen zelfactiverende clients.</td>
<td style="border:1px solid black;">Alle SP1-functies.
Offline-inschrijving van server.
Zelfactiverende clients.
Server-lockbox.
Microsoft SQL Server™ 2005 wordt standaard ondersteund.</td>
<td style="border:1px solid black;">Alle voorgaande functies plus SP2-functies.
Offline-inschrijving van server.
SP2-clients zijn zelfactiverend.
Versie 1-clients moeten activeren via internet.</td>
</tr>
</tbody>
</table>
 

<span id="bkmk_RemovingRMS"></span>
RMS met SP2 verwijderen
-----------------------

Als u de RMS-server wilt herstellen naar de vorige configuratie nadat u RMS met SP2 hebt geïnstalleerd, kunt u **Software** gebruiken in **Configuratiescherm** om RMS met SP2 te verwijderen.
