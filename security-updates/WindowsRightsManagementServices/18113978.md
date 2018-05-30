---
TOCTitle: Servicelocatorservice van RMS
Title: Servicelocatorservice van RMS
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18113978
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747548(v=WS.10)'
---

Servicelocatorservice van RMS
=============================

De servicelocatorservice wordt uitgevoerd in de RMS-basisclusters en in de clusters die alleen voor licentieverlening worden gebruikt. Met de servicelocatorservice wordt de serviceverbindings-URL van het cluster beschikbaar gesteld aan Active Directory, zodat deze kan worden gebruikt door clients met RMS-ondersteuning.

Het toepassingsbestand voor de servicelocatorservice, ServiceLocator.asmx, bevindt zich in de virtuele mappen Certification en Licensing in IIS.

In de volgende tabel wordt de standaard-ACL (Access Control List) van deze service weergegeven:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Gebruiker of groep</th>
<th style="border:1px solid black;" >Standaardmachtiging</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Administrators</td>
<td style="border:1px solid black;">Volledig beheer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS-servicegroep</td>
<td style="border:1px solid black;">Lezen en uitvoeren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Volledig beheer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Gebruikers</td>
<td style="border:1px solid black;">Lezen en uitvoeren</td>
</tr>
</tbody>
</table>
