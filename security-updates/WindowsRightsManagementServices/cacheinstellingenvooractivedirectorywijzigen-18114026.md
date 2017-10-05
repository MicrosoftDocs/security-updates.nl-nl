---
TOCTitle: 'Cache-instellingen voor Active Directory wijzigen'
Title: 'Cache-instellingen voor Active Directory wijzigen'
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18114026
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747586(v=WS.10)'
---

Cache-instellingen voor Active Directory wijzigen
=================================================

De instellingen in het register geven aan hoeveel vermeldingen moeten worden opgeslagen in de Active Directory-cache. Wilt u de reactietijd voor clientaanvragen verbeteren, dan kunt u deze instellingen wijzigen. Zie 'Prestaties van directoryservices optimaliseren' eerder in dit onderwerp voor meer informatie. U kunt ook de geldigheidsduur opgeven voor informatie die is opgeslagen in de cache.

Op computers met de 32-bits versie van Windows Server 2003 is de volgende registersleutel het volledige subsleutelpad voor de cachevermeldingen:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Op computers met de 64-bits versie van Windows Server 2003 is de volgende registersleutel het volledige subsleutelpad voor de cachevermeldingen:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

In de volgende tabel vindt u een overzicht van vermeldingen waarmee het gedrag van de geheugencache wordt beheerd.

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
<th style="border:1px solid black;" >Type</th>
<th style="border:1px solid black;" >Standaardwaarde</th>
<th style="border:1px solid black;" >Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Het maximum aantal principals en de bijbehorende e-mailadressen en beveiligings-id's (SID's) dat in de cache kan worden opslagen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Geldigheidsduur van de gegevens in de cache voor principals.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Het maximum aantal groepen en de bijbehorende e-mailadressen en beveiligings-id's (SID's) dat in de cache kan worden opslagen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Geldigheidsduur van de gegevens in de cache voor groepslidmaatschappen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Het maximum aantal contacten die lid zijn van een groep die kan worden opgeslagen in de cache.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Geldigheidsduur van de gegevens in de cache voor contactpersonen die lid zijn van een groep.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747586.Caution(WS.10).gif)Waarschuwing                                                                                          |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u het register onjuist bewerkt, kunt u het systeem ernstig beschadigen. Maak een back-up van alle belangrijke gegevens op de computer voordat u het register wijzigt. |
  
| ![](images/Cc747586.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                    |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| De registervermeldingen **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** en **ContactMembersofGroupCacheExpireMinutes** hebben ook betrekking op het verlopen van de lokale Active Directory-cache in de directoryservicesdatabase op uw databaseserver. |
