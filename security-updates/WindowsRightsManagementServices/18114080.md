---
TOCTitle: Tabellen voor basisconfiguratiedatabase van RMS
Title: Tabellen voor basisconfiguratiedatabase van RMS
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18114080
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747676(v=WS.10)'
---

Tabellen voor basisconfiguratiedatabase van RMS
===============================================

In dit onderwerp worden de tabellen voor de basisconfiguratiedatabase van RMS beschreven.

DRMS\_ApplicationExclusionList
------------------------------

In de volgende tabel vindt u informatie over uitgesloten toepassingen.

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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Naam</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van de toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Minimale primaire versienummer van de toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Minimale secundaire versienummer van de toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Minimale buildnummer van de toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Minimale revisienummer van de toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Maximale primaire versienummer van de toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Maximale secundaire versienummer van de toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Maximale buildnummer van de toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Maximale revisienummer van de toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beschrijving</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Beschrijving van de toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
In de volgende tabel vindt u informatie over de berichtenwachtrij.
  
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
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Pad naar de berichtenwachtrij</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
In de volgende tabel vindt u informatie over het type certificaat dat voor de client is uitgegeven.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">De id voor het certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Bureaublad, mobiel apparaat of server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
In de volgende tabel vindt u informatie over het huidige serverlicentieverleningscertificaat dat zich bevindt in de tabel DRMS\_LicensorCertificate.
  
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
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Het actieve licentieverleningscertificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
In de volgende tabel vindt u informatie over de locaties waar de clusterbeleidsrichtlijnen worden opgeslagen.
  
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
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Id van beleid</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van beleid</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Beleidsgegevens</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
In de volgende tabel vindt u informatie over de servers in het cluster.
  
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
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Id van de server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet opgegeven</td>
<td style="border:1px solid black;">Computernaam voor server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
In de volgende tabel vindt u informatie over de uitgesloten rechtenaccountcertificaten.
  
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
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Bytes van openbare sleutels</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Index van gebruikers-id</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Datum waarop het rechtenaccountcertificaat verloopt</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beschrijving</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Naam die bij de sleutel van dit uitgesloten rechtenaccountcertificaat hoort</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
In de volgende tabel vindt u informatie over het actieve serverlicentieverleningscertificaat.
  
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
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Id van beleid</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Id-type van sleutelpaar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">GUID van sleutelpaar-id</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Verwijzing naar werkelijk certificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
In volgende tabel vindt u informatie over de persoonlijke sleutel van het actieve serverlicentieverleningscertificaat.
  
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
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Id-type van sleutelpaar</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">GUID van sleutelpaar-id</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Binaire weergave van de sleutel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Naam van de cryptografieprovider</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Type cryptografieprovider</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Niet opgegeven</td>
<td style="border:1px solid black;">Naam van de sleutelcontainer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Sleutelnummer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
In de volgende tabel vindt u informatie over de accounts van Microsoft® .NET Passport waaraan geen licenties mogen worden verleend.
  
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
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Gebruikersnaam/domeinnaam</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
In de volgende tabel vindt u informatie over invoegtoepassingen.
  
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
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Type invoegtoepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naamruimte voor deze invoegtoepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van deze invoegtoepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Volgnummer waarop de invoegtoepassing wordt uitgevoerd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Pad naar het DLL-bestand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Niet in gebruik</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Geeft aan of een invoegtoepassing in de foutopsporingsmodus moet worden uitgevoerd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Openbare sleutel van de invoegtoepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Versie van de invoegtoepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
In de volgende tabel vindt u informatie over de versies van de invoegtoepassing die in het RMS-systeem mogen worden gebruikt.
  
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
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Niet opgegeven</td>
<td style="border:1px solid black;">Versie van de invoegtoepassing</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
In de volgende tabel vindt u informatie over de eigenschappen van de invoegtoepassing.
  
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
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Id van de invoegtoepassing waartoe de eigenschap behoort</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">De eigenschappennaam voor deze configuratiegegevens</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">De eigenschappenwaarde voor deze configuratiegegevens</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
In de volgende tabel vindt u informatie over de typen invoegtoepassingen.
  
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
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Naam van deze invoegtoepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
In de volgende tabel vindt u informatie over sjablonen voor rechtenbeleid.
  
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
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">GUID van de sjabloon voor rechtenbeleid</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Dit veld bevat de XrML-sjabloongegevens.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
In de volgende tabel vindt u informatie over de vertrouwde certificeringsinstanties.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Id van het certificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">GUID van het certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Type certificeringsinstantie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
In de volgende tabel wordt informatie weergegeven over de e-maildomeinen die vertrouwd zijn in de RMS-omgeving
  
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
<td style="border:1px solid black;">Id</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (FK)t</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Lijst met e-maildomeinnamen die geldig zijn voor het vertrouwde gebruikersdomein</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
In de volgende tabel vindt u informatie over de vertrouwde gebruikersdomeinen en de vertrouwde uitgiftedomeinen.
  
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
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Interne index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Type domein</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Type GUID van certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">GUID van het certificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Id van het certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">SID van domein</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Beschrijvende naam van certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met updatedatum/-tijd</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Tijdstempel met aanmaakdatum/-tijd</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
In de volgende tabel vindt u informatie over de XrML-serverlicentieverleningscertificaten waarnaar wordt verwezen in de tabel DRMS\_LicensorCertificate. Hierin wordt ook de certificaatketen aangegeven.
  
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
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) Niet Null</td>
<td style="border:1px solid black;">Verwijzing naar werkelijk certificaat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Niet Null</td>
<td style="border:1px solid black;">Verwijzing naar werkelijk certificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Null</td>
<td style="border:1px solid black;">Verwijzing naar werkelijk certificaat</td>
</tr>
</tbody>
</table>
