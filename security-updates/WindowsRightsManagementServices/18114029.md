---
TOCTitle: Intrekking in sjablonen voor het rechtenbeleid
Title: Intrekking in sjablonen voor het rechtenbeleid
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18114029
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720226(v=WS.10)'
---

Intrekking in sjablonen voor het rechtenbeleid
==============================================

Voorwaarden voor intrekking worden opgegeven in sjablonen voor het rechtenbeleid. De waarden die u in een sjabloon voor het rechtenbeleid opgeeft voor de intrekkingsvoorwaarden, worden opgenomen in de XrML-code REFRESH in de uitgiftelicentie die wordt uitgegeven op basis van dat sjabloon. De resulterende gebruikslicentie die door de server wordt uitgegeven, bevat eveneens de code REFRESH.

In de volgende tabel worden de parameters beschreven die worden opgenomen in de code REFRESH.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parameter</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">De id van de intrekkingslijst.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">De URL of UNC voor de intrekkingslijst.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">De openbare sleutel van de uitgever van de intrekkingslijst. Deze openbare sleutel komt overeen met de persoonlijke sleutel waarmee de intrekkingslijst is ondertekend.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">De maximale geldigheidsduur van de intrekkingslijst in dagen. Als de intrekkingslijst in de cache ouder is dan is toegestaan volgens INTERVALTIME, wordt de meest recente intrekkingslijst door de RMS-client uit de URL in ADDRESS opgehaald. Zo wordt gegarandeerd dat er een bijgewerkte intrekkingslijst wordt gebruikt.</td>
</tr>
</tbody>
</table>
  
Zie 'Sjablonen voor het rechtenbeleid maken en wijzigen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over het maken van sjablonen voor het rechtenbeleid.
