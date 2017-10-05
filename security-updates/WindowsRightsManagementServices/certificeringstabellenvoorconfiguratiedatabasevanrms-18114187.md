---
TOCTitle: Certificeringstabellen voor configuratiedatabase van RMS
Title: Certificeringstabellen voor configuratiedatabase van RMS
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18114187
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747760(v=WS.10)'
---

Certificeringstabellen voor configuratiedatabase van RMS
========================================================

In dit onderwerp worden de certificeringstabellen in de configuratiedatabase van RMS beschreven. De tabellen bevatten informatie over de rechtenaccountcertificaten die worden verleend aan gebruikers van deze installatie.

UD\_Machines
------------

In de volgende tabel vindt u informatie over de hardware-id's voor alle computers.

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
<th>Naam</th>
<th>Gegevenstype</th>
<th>Null-waarden</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Niet Null</td>
<td style="border:1px solid black;">Hash van de hardware-id</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Datum en tijd waarop de vermelding is toegevoegd aan de tabel</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
In de volgende tabel vindt u informatie over Microsoft® .NET Passport voor gebruikers.
  
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
<th>Naam</th>
<th>Gegevenstype</th>
<th>Null-waarden</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) Null</td>
<td style="border:1px solid black;">Id van .NET Passport-gebruikers</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
In de volgende tabel worden gecertificeerde gebruikers gekoppeld aan de bijbehorende computergegevens.
  
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
<th>Naam</th>
<th>Gegevenstype</th>
<th>Null-waarden</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Datum en tijd waarop de vermelding is toegevoegd aan de tabel</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
In de volgende tabel vindt u informatie over gebruikersgegevens.
  
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
<th>Naam</th>
<th>Gegevenstype</th>
<th>Null-waarden</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Niet Null</td>
<td style="border:1px solid black;">Gecodeerde openbare/persoonlijke sleutel van de gebruiker</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Lengte van de niet-gecodeerde openbare/persoonlijke sleutel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Openbare sleutel van gebruiker</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Index van het licentieverleningscertificaat dat wordt gebruikt om het openbare/persoonlijke sleutelpaar te coderen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Niet opgegeven</td>
<td style="border:1px solid black;">Niet in gebruik</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Verloopdatum van de gebruikerssleutel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Verloopdatum en -tijd voor tijdelijk gebruik van de sleutel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Niet in gebruik</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Huidig quotumniveau van de gebruiker</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Aantal dagen voordat extra quotumaanvragen kunnen worden voltooid</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Datum en tijd van het laatste extra gebruikerscertificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Datum en tijd waarop de vermelding is toegevoegd aan de tabel</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
In de volgende tabel vindt u een overzicht van de id's van alle geverifieerde en gecertificeerde gebruikers van Windows.
  
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
<th>Naam</th>
<th>Gegevenstype</th>
<th>Null-waarden</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Beveiligings-id (SID) van de gebruiker</td>
</tr>
</tbody>
</table>
