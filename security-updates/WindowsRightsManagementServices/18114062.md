---
TOCTitle: Activeringsproxyservice van RMS
Title: Activeringsproxyservice van RMS
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18114062
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747608(v=WS.10)'
---

Activeringsproxyservice van RMS
===============================

Alle aanvragen voor computeractivering in RMS versie 1.0 worden verwerkt in de activeringsproxyservice, die alleen wordt uitgevoerd in het RMS-basiscluster. U moet een clientcomputer activeren voordat u hierop door rechten beveiligde inhoud kunt uitgeven of gebruiken met RMS. De RMS-client voor Service Pack 1 is een 'zelfactiverende' client. Deze client heeft niet de activeringsproxyserver of de activeringsservice van Microsoft nodig om een lockbox en computercertificaat te genereren.

Met de activeringsproxyservice worden aanvragen voor computeractivering van RMS versie 1-clients doorgestuurd naar de activeringsservice van Microsoft. Vervolgens worden een gegenereerde lockbox en een bijbehorend RMS-computercertificaat teruggestuurd die uniek zijn voor de specifieke gebruiker en computer. Daarna worden deze items met de activeringsproxyservice doorgestuurd naar de client waarmee de aanvraag is verzonden.

Het toepassingsbestand voor de activeringsproxyservice, Activation.asmx, bevindt zich in de virtuele map Certification in IIS. In de volgende tabel wordt de standaard-ACL (Access Control List) van deze service weergegeven:

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
<td style="border:1px solid black;">Gasten</td>
<td style="border:1px solid black;">Lezen en uitvoeren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS-servicegroep</td>
<td style="border:1px solid black;">Lezen en uitvoeren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Volledig beheer</td>
</tr>
</tbody>
</table>
