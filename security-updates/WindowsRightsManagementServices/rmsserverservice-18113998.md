---
TOCTitle: 'RMS-serverservice'
Title: 'RMS-serverservice'
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18113998
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747566(v=WS.10)'
---

RMS-serverservice
=================

De serverservice wordt alleen uitgevoerd in het RMS-basiscluster. Met de serverservice wordt een aanvraag, die met een client via on line uitgifte is gemaakt, weergegeven om een serverlicentieverleningscertificaat op te halen.

Het toepassingsbestand voor de serverservice, Server.asmx, bevindt zich in de virtuele map Certification in IIS.

In de volgende tabel wordt de standaard-ACL (Access Control List) van deze service weergegeven:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Gebruiker of groep</th>
<th>Standaardmachtiging</th>
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
