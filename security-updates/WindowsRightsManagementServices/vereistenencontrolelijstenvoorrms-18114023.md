---
TOCTitle: Vereisten en controlelijsten voor RMS
Title: Vereisten en controlelijsten voor RMS
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18114023
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747582(v=WS.10)'
---

Vereisten en controlelijsten voor RMS
=====================================

Voordat u RMS installeert, dient u eerst de technologische vereisten voor het gebruik van RMS te bekijken. Alle vermelde technologieën gelden voor RMS en een basiskennis van deze vereisten is noodzakelijk om RMS goed te kunnen implementeren. De volgende controlelijsten kunnen helpen bij het maken van takenlijsten en de planningen voor het implementeren en beheren van RMS:

-   [Vereisten technologie](#bkmk_9)
-   [Controlelijsten voor RMS-implementatie](#bkmk_10)
-   [Controlelijsten voor RMS-beheer](#bkmk_14)

<span id="BKMK_9"></span>
Vereisten technologie
---------------------

In deze documentatie vindt u informatie over de werking van Windows RMS, het plannen en uitvoeren van de implementatie in uw organisatie en het dagelijks beheer van het systeem. Er wordt verondersteld dat u enige kennis hebt van:

-   implementatie en beheer van Windows Server 2003;
-   implementatie en beheer van Active Directory;
-   Implementatie en beheer van Internet Information Services 6.0 (IIS);
-   Beheer van Microsoft® SQL Server™ 2000
-   Basisconcepten van PKI (Public Key Infrastructure; infrastructuur met openbare sleutels);
-   Servernetwerken en -beveiliging.

Zie 'Overige informatiebronnen' in [Een RMS-server beheren](http://go.microsoft.com/fwlink/?linkid=42495) in deze documentatie voor meer informatie over deze onderwerpen.

<span id="BKMK_10"></span>
Controlelijsten voor RMS-implementatie
--------------------------------------

In deze sectie staan controlelijsten voor de volgende implementatietaken:

-   [Eén serverinstallatie implementeren](#bkmk_11)
-   [Basiscertificerings- en licentieclusters implementeren](#bkmk_12)
-   [RMS in andere forests implementeren](#bkmk_13)

Zie [Een RMS-systeem implementeren](http://go.microsoft.com/fwlink/?linkid=42494) in deze documentatie voor meer informatie over het implementeren van RMS.

<span id="BKMK_11"></span>
Eén serverinstallatie implementeren
-----------------------------------

Gebruik de volgende controlelijst om één RMS-server te implementeren.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Concepten en planningsgegevens bestuderen.</td>
<td style="border:1px solid black;">'Preparing for an RMS Deployment' op <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Systeemvereisten bestuderen en controleren of alle vereiste hardware en software beschikbaar is.</td>
<td style="border:1px solid black;">'Infrastructuurvereisten voor RMS' in <a href="http://go.microsoft.com/fwlink/?linkid=37537">Een RMS-implementatie plannen</a>.
'De infrastructuur van de databaseserver plannen' in <a href="http://go.microsoft.com/fwlink/?linkid=37537">Een RMS-implementatie plannen</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">De infrastructuur opzetten, waaronder voorwaarden voor hardware en software, beheerdersaccounts en, al naar gelang de situatie, ondersteuning van SMS of groepsbeleid.</td>
<td style="border:1px solid black;">'Een RMS-implementatie voorbereiden' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Installeer en configureer RMS op de server.</td>
<td style="border:1px solid black;">'Certificerings- en licentieservices instellen op de eerste server' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-implementatie plannen</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">De implementatie testen.</td>
<td style="border:1px solid black;">'Een testomgeving instellen' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Implementeer RMS in de productieomgeving.</td>
<td style="border:1px solid black;">'De omvang van de RMS-implementatie plannen' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Basiscertificerings- en licentieclusters implementeren  
------------------------------------------------------
  
Gebruik de volgende controlelijst om basiscertificerings- en licentieclusters te implementeren.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Concepten en planningsgegevens bestuderen.</td>
<td style="border:1px solid black;">'Een RMS-implementatie voorbereiden' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Systeemvereisten bestuderen en controleren of alle vereiste hardware en software beschikbaar is.</td>
<td style="border:1px solid black;">'Infrastructuurvereisten voor RMS' in <a href="http://go.microsoft.com/fwlink/?linkid=37537">Een RMS-implementatie plannen</a>.
'De infrastructuur van de databaseserver plannen' in <a href="http://go.microsoft.com/fwlink/?linkid=37537">Een RMS-implementatie plannen</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Het implementatieplan bestuderen om inzicht te krijgen in de topologie en de onderdelen die moeten worden geïnstalleerd.</td>
<td style="border:1px solid black;">'Uw RMS-topologie bepalen' in <a href="http://go.microsoft.com/fwlink/?linkid=37537">Een RMS-implementatie plannen</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">De infrastructuur opzetten, waaronder voorwaarden voor hardware en software, beheerdersaccounts en, al naar gelang de situatie, ondersteuning van SMS of groepsbeleid.</td>
<td style="border:1px solid black;">'Een RMS-implementatie voorbereiden' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Installeer en configureer RMS op de servers die zich in het basiscertificeringscluster bevinden.</td>
<td style="border:1px solid black;">'Certificerings- en licentieservices instellen op de eerste server' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.
'Servers toevoegen ter ondersteuning van certificering en licenties' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">De RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Installeer en configureer RMS op de servers die zich in de licentieclusters bevinden.</td>
<td style="border:1px solid black;">'Certificerings- en licentieservices instellen op de eerste server' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-implementatie plannen</a>.
'Servers toevoegen ter ondersteuning van certificering en licenties' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-implementatie plannen</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Taakverdeling instellen.</td>
<td style="border:1px solid black;">'De basisinfrastructuur voor ondersteuning van clusters uitbreiden' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">De implementatie testen.</td>
<td style="border:1px solid black;">'Een testomgeving instellen' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Implementeer RMS in de productieomgeving.</td>
<td style="border:1px solid black;">'De omvang van de RMS-implementatie plannen' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
RMS in andere forests implementeren  
-----------------------------------
  
Gebruik de volgende controlelijst om de basisversie van RMS in forests te implementeren.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Concepten en planningsgegevens bestuderen.</td>
<td style="border:1px solid black;">'Een RMS-implementatie voorbereiden' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">De vereiste machtigingen configureren op basis van uw vertrouwensmodel.</td>
<td style="border:1px solid black;">'RMS in andere forests implementeren' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Stel de gewenste Active Directory-kenmerken voor uw forests in.</td>
<td style="border:1px solid black;">'RMS in andere forests implementeren' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
Controlelijsten voor RMS-beheer  
-------------------------------
  
In deze sectie staan controlelijsten voor de volgende beheertaken:
  
-   [Een sjabloon voor het rechtenbeleid implementeren](#bkmk_15)  
-   [Een nieuwe RMS-client implementeren](#bkmk_16)  
-   [Een vertrouwd gebruikersdomein toevoegen](#bkmk_17)  
-   [Een vertrouwd uitgiftedomein toevoegen](#bkmk_18)
  
Zie '[Een RMS-server beheren'](http://go.microsoft.com/fwlink/?linkid=42495) in deze documentatie voor meer informatie over het beheren van RMS.
  
<span id="BKMK_15"></span>
Een sjabloon voor het rechtenbeleid implementeren  
-------------------------------------------------
  
Gebruik de volgende controlelijst om een sjabloon voor rechtenbeleid te implementeren.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Relevante concepten bestuderen.</td>
<td style="border:1px solid black;">'Sjablonen voor het rechtenbeleid' in <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische referentie van RMS</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">De locatie voor de sjablonen voor het rechtenbeleid opgeven.</td>
<td style="border:1px solid black;">'De locatie van de sjablonen voor het rechtenbeleid opgeven' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">De sjabloon voor het rechtenbeleid maken.</td>
<td style="border:1px solid black;">'Sjablonen voor het rechtenbeleid maken en wijzigen' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.
'Een sjabloon voor het rechtenbeleid toevoegen' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">De sjabloon voor het rechtenbeleid distribueren.</td>
<td style="border:1px solid black;">'Sjablonen voor het rechtenbeleid distribueren' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Een nieuwe RMS-client implementeren  
-----------------------------------
  
Gebruik de volgende controlelijst om een nieuwe versie van de RMS-client te implementeren.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Relevante concepten bestuderen.</td>
<td style="border:1px solid black;">'Distributie naar clients plannen' in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Een RMS-systeem implementeren</a>
'Lockbox-versies uitsluiten' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Als u alle clients wilt bijwerken met de meest recente clientversie, moet u de verouderde versie van Lockbox uitsluiten.</td>
<td style="border:1px solid black;">'Lockbox-versies uitsluiten' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Een vertrouwd gebruikersdomein toevoegen  
----------------------------------------
  
Gebruik de volgende controlelijst om een vertrouwd gebruikersdomein toe te voegen.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Relevante concepten bestuderen.</td>
<td style="border:1px solid black;">'Vertrouwde gebruikersdomeinen' in <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische referentie van RMS</a>.
'Vertrouwde gebruikersdomeinen toevoegen en verwijderens' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Het serverlicentiecertificaat verkrijgen van het gebruikersdomein dat u wilt toevoegen. (Dit moet worden verstrekt door de beheerder van de installatie waarmee een vertrouwensrelatie wordt aangegaan.) Het gebruikersdomein toevoegen aan uw installatie.</td>
<td style="border:1px solid black;">'Een vertrouwd gebruikersdomein toevoegen' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Een vertrouwd uitgiftedomein toevoegen  
--------------------------------------
  
Gebruik de volgende controlelijst om een vertrouwd uitgiftedomein toe te voegen.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Stap</th>
<th style="border:1px solid black;" >Zie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Relevante concepten bestuderen.</td>
<td style="border:1px solid black;">'Vertrouwde uitgiftedomeinen' in <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische referentie van RMS</a>.
'Vertrouwde uitgiftedomeinen toevoegen en verwijderen' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Het gecodeerde serverlicentiecertificaat en de persoonlijke sleutel verkrijgen van het uitgiftedomein dat u wilt toevoegen. Vervolgens het uitgiftedomein toevoegen aan uw installatie.</td>
<td style="border:1px solid black;">'Een vertrouwd uitgiftedomein toevoegen' in <a href="http://go.microsoft.com/fwlink/?linkid=42495">Een RMS-server beheren</a>.</td>
</tr>
</tbody>
</table>
