---
TOCTitle: Vereiste accounts en machtigingen voor RMS
Title: Vereiste accounts en machtigingen voor RMS
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18113877
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720178(v=WS.10)'
---

Vereiste accounts en machtigingen voor RMS
==========================================

In de volgende tabel vindt u de gebruikersrechten en machtigingen die nodig zijn als u RMS wilt implementeren en beheren.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Activiteit</th>
<th style="border:1px solid black;" >Gebruikersaccount en machtigingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS installeren</td>
<td style="border:1px solid black;">Meld u aan met een domeinaccount die lid is van de lokale groep Administrators.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS inrichten</td>
<td style="border:1px solid black;">Meld u aan met een domeinaccount die lid is van de lokale groep Administrators. Daarnaast moet de door u gebruikte account op de SQL Server systeembeheerdersmachtigingen hebben voor de SQL Server-database, zodat RMS de databases kan instellen.
Tijdens het inrichten moet u de RMS-serviceaccount opgeven die u al eerder hebt gemaakt. De account moet een standaard gebruikersaccount van een domein zijn, zonder aanvullende machtigingen. Deze account wordt lid gemaakt van de RMS-servicegroep. Dit is de account waaronder RMS tijdens routinebewerkingen wordt uitgevoerd.
Als u op één server wilt installeren en de database zich op dezelfde computer bevindt als de basiscertificeringsserver, kunt u de lokale systeemaccount opgeven. Uit veiligheidsoverwegingen is het echter raadzaam altijd de RMS-serviceaccount op te geven in plaats van de lokale systeemaccount. Wanneer de database zich op een afzonderlijke server bevindt, moet u de RMS-serviceaccount opgeven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS beheren</td>
<td style="border:1px solid black;">Meld u aan met een domeinaccount die lid is van de lokale groep Administrators. U kunt de beveiligingsinstellingen aanpassen om de toegang tot de webpagina's voor beheer te configureren.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720178.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                   |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Voor de account die wordt gebruikt voor het aanmelden bij de RMS-server, is geen lidmaatschap voor de aanvullende domeingroepen zoals de groep domeinbeheerders nodig. Voor sommige beheertaken, zoals het registreren van het serviceverbindingspunt en het aanpassen van het beveiligingsbeleid, is echter een account met aanvullende bevoegdheden nodig. |
