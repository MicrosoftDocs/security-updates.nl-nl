---
TOCTitle: Uitgifteservice van RMS
Title: Uitgifteservice van RMS
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18113917
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720267(v=WS.10)'
---

Uitgifteservice van RMS
=======================

De uitgifteservice, waarmee uitgiftelicenties worden uitgegeven, wordt uitgevoerd in het RMS-basiscluster. Daarnaast wordt de uitgifteservice uitgevoerd in clusters die alleen voor licentieverlening worden gebruikt. Met uitgiftelicenties wordt het beleid bepaald op basis waarvan gebruikslicenties kunnen worden geleverd.

Het toepassingsbestand voor de uitgifteservice, Publish.asmx, bevindt zich in de virtuele map Licensing in IIS.

In de volgende tabel wordt de standaard-ACL (Access Control List) van de service weergegeven:

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
