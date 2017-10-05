---
TOCTitle: Serverlicentieverleningscertificaten beheren
Title: Serverlicentieverleningscertificaten beheren
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18113921
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720272(v=WS.10)'
---

Serverlicentieverleningscertificaten beheren
============================================

Serverlicentieverleningscertificaten verlopen na een bepaalde periode (doorgaans een jaar). Als u een serverlicentieverleningscertificaat wilt vernieuwen, moet u zijn aangemeld als lokale beheerder. Wanneer u het serverlicentieverleningscertificaat voor het basiscertificeringscluster vernieuwt, wordt in RMS een aanvraag voor vernieuwing van het serverlicentieverleningscertificaat naar de activeringsservice van Microsoft verstuurd. Vernieuwt u het certificaat voor een licentieserver, dan wordt de vernieuwingsaanvraag verstuurd naar de basiscertificeringsserver waarmee het huidige certificaat is uitgegeven.

In RMS worden drie gebeurtenissen in het systeemlogboek vastgelegd die u in de gaten moet houden. Met deze gebeurtenissen wordt aangegeven dat de vernieuwingsdatum voor het serverlicentieverleningscertificaat nadert of dat het certificaat is verlopen. In de volgende tabel vindt u een overzicht van de gebeurtenis-id's en -namen.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Gebeurtenis-id</th>
<th style="border:1px solid black;" >Gebeurtenisnaam</th>
<th style="border:1px solid black;" >Gebeurtenistype</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Waarschuwing Service blijft normaal functioneren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Waarschuwing Service blijft normaal functioneren.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Fout. Service is uitgeschakeld.</td>
</tr>
</tbody>
</table>
