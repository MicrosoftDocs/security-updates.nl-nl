---
TOCTitle: Licentieservice van RMS
Title: Licentieservice van RMS
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18113934
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720278(v=WS.10)'
---

Licentieservice van RMS
=======================

De licentieservice, waarmee gebruikslicenties worden uitgegeven, wordt uitgevoerd in het RMS-basiscluster. Daarnaast wordt de licentieservice uitgevoerd in clusters die alleen voor licentieverlening wordt gebruikt. Met gebruikslicenties kunnen gebruikers met door rechten beveiligde inhoud werken.

Het toepassingsbestand voor de licentieservice, License.asmx, bevindt zich in de virtuele map Licensing in IIS.

| ![](/security-updates/images/Cc720278.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voor de verwerking van licentieaanvragen die afkomstig zijn van het basiscluster kunt u een apart cluster implementeren dat alleen voor licentieverlening wordt gebruikt. U kunt ook aparte licentieservers of -clusters voor afdelingen implementeren, bijvoorbeeld als u afdelingen de mogelijkheid wilt bieden hun eigen rechtenbeleid in te stellen. Zie voor meer informatie over deze afwegingen "Kernonderdelen identificeren" in "RMS: Planning en architectuur " in deze documentatie. |

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
