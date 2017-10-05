---
TOCTitle: Registratiedatabasetabellen van RMS
Title: Registratiedatabasetabellen van RMS
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18114007
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747569(v=WS.10)'
---

Registratiedatabasetabellen van RMS
===================================

In dit gedeelte worden de logboekdatabasetabellen van RMS beschreven.

DRMS\_Log\_Master
-----------------

In de volgende tabel vindt u een overzicht van de vermeldingen voor logboekrecords.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Naam</th>
<th style="border:1px solid black;" >Gegevenstype</th>
<th style="border:1px solid black;" >Null-waarden</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Niet Null</td>
<td style="border:1px solid black;">Unieke id voor deze logboekrecord</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Server die deze record heeft gegenereerd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Aanvraag-id</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Datum en tijd van aanvraag</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">URL-pad van de aanvraag</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Type aanvraag</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">IP-adres van de client</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Gebruikersagent-header van de client</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Verificatiestatus van de aanvraag</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">SSL-beveiliging van de aanvraag</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Id van de geverifieerde gebruiker</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">XrML ontvangen van de client in de aanvraag</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">XrML-licentie verleend in de aanvraag</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Metadata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Aanvraag is gelukt of mislukt</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Fout in gegevens</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Aanmaaktijd van logboek</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
In de volgende tabel vindt u een overzicht van extra gegevens voor een logboekrecord. Doorgaans worden XrML-gegevens in deze tabel geregistreerd.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Naam</th>
<th style="border:1px solid black;" >Gegevenstype</th>
<th style="border:1px solid black;" >Null-waarden</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1)</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Niet Null (FK)</td>
<td style="border:1px solid black;">Id van de bovenliggende logboekrecord</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van de eigenschap</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Waarde van de eigenschap</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
In de volgende tabel vindt u een overzicht van de velden waarin de service van de logboekregistratie-listener wordt geregistreerd.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Naam</th>
<th style="border:1px solid black;" >Gegevenstype</th>
<th style="border:1px solid black;" >Null-waarden</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van het veld</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Beschrijving van het veld</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Geeft aan of het veld is geregistreerd</td>
</tr>
</tbody>
</table>
