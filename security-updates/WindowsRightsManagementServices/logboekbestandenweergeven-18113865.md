---
TOCTitle: Logboekbestanden weergeven
Title: Logboekbestanden weergeven
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18113865
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720228(v=WS.10)'
---

Logboekbestanden weergeven
==========================

Logboekbestanden worden opgeslagen in een databaseserver zoals SQL Server of Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) versie A, afhankelijk van de manier waarop RMS is geïmplementeerd. Met filters kunt u het aantal gegevens verminderen die in de logboekbestanden worden opgeslagen. Raadpleeg de Help van SQL Server Enterprise Manager voor instructies.

De grootte van een normale logboekvermelding is ongeveer 300 bytes. In de volgende tabel worden de velden beschreven die worden vastgelegd.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Veld</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">HostMachineName</td>
<td style="border:1px solid black;">De computer waarmee de aanvraag is verwerkt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">HostMachineRequestId</td>
<td style="border:1px solid black;">De unieke id van deze aanvraag op deze computer. Gezamenlijk vormen de HostMachineName en de HostMachineRequestId een unieke aanduiding van de aanvraag in het cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestTime</td>
<td style="border:1px solid black;">Tijdstip, in Coordinated Universal Time (Greenwich Mean Time), waarop de aanvraag is ontvangen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestPath</td>
<td style="border:1px solid black;">Relatieve URL naar het ASMX-bestand, bijvoorbeeld: /_wmcs/licensing/License.asmx.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestType</td>
<td style="border:1px solid black;">Naam van de aangeroepen webmethode, bijvoorbeeld: AcquireLicense.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestUserAddress</td>
<td style="border:1px solid black;">Bron-IP-adres van de aanvrager.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestUserAgent</td>
<td style="border:1px solid black;">Waarde van de gebruikersagent voor de HTTP-header.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedState</td>
<td style="border:1px solid black;">Hiermee wordt aangegeven of de HTTP-verbinding is geverifieerd (True/False).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SecureConnectionState</td>
<td style="border:1px solid black;">Hiermee wordt aangegeven of dit een SSL-verbinding is (True/False).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedId</td>
<td style="border:1px solid black;">Aanmeldingsnaam voor geverifieerde aanvragen. Deze is leeg als AuthenticatedState=False.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ReceivedXrMLDocument</td>
<td style="border:1px solid black;">Het XrML-document dat is ontvangen van de aanvrager.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ReceivedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">De uitgeverketen voor het ontvangen XrML-document.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IssuedXrMLDocument</td>
<td style="border:1px solid black;">Het XrML-document dat is teruggestuurd naar de aanvrager.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">IssuedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">De uitgeverketen voor het uitgegeven XrML-document.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SuccessOrFailure</td>
<td style="border:1px solid black;">Hiermee wordt aangegeven of de aanvraag is gelukt of mislukt (Succeeded/Failed).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Metadata</td>
<td style="border:1px solid black;">Veld voor metagegevens.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ErrorInformation</td>
<td style="border:1px solid black;">Beschrijvend foutbericht, als er een fout is opgetreden.</td>
</tr>
</tbody>
</table>
