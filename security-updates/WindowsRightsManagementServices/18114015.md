---
TOCTitle: 'RMS-database met directoryservices'
Title: 'RMS-database met directoryservices'
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18114015
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747617(v=WS.10)'
---

RMS-database met directoryservices
==================================

De databaseserver treedt als host op voor de database met directoryservices. Deze database bevat informatie over gebruikers, id's (zoals e-mailadressen), beveiligings-id's (SID's), groepslidmaatschappen en alternatieve id's. Deze gegevens worden verkregen via LDAP-aanvragen die met de licentieservice van RMS naar de globale catalogus van Active Directory worden verstuurd. Zie '[Active Directory-cache van RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)' verderop in dit onderwerp voor meer informatie over dit proces en het doel van dit proces.

Aan de RMS-servicegroep zijn uitvoeringsmachtigingen toegewezen voor de opgeslagen procedures in de database met directoryservices.

De volgende tabel bevat de Active Directory-kenmerken die worden opgeslagen in de tabellen in de database met directoryservices.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Tabel</th>
<th style="border:1px solid black;" >Kenmerk</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: de alias voor de groep.<br />
<br />
</li>
<li>GroupID: de unieke id voor deze groep.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: de DN-naam voor deze groep in Active Directory.<br />
<br />
</li>
<li>GroupID: de unieke id voor deze groep.<br />
<br />
</li>
<li>Expiration: de datum en het tijdstip waarop de opgeslagen gegevens voor deze groep verlopen.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: de unieke id voor deze groep.<br />
<br />
</li>
<li>ParentID: de unieke id van de groep waarvan deze groep deel uitmaakt.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: een aliasnaam voor de principal.<br />
<br />
</li>
<li>PrincipalID: de unieke id voor deze principal.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: de unieke id voor deze principal.<br />
<br />
</li>
<li>Expiration: de datum en het tijdstip waarop de opgeslagen gegevens voor deze principal verlopen.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Elke rij van deze tabel bevat de unieke id van een principal en de unieke id van een groep waarvan deze principal deel uitmaakt.
<ul>
<li>PrincipalID: de unieke id voor deze principal.<br />
<br />
</li>
<li>ParentID: de unieke id van een groep waarvan deze principal deel uitmaakt.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
