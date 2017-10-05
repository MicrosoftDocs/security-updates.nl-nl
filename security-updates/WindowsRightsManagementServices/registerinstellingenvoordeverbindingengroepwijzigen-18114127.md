---
TOCTitle: Registerinstellingen voor de verbindingengroep wijzigen
Title: Registerinstellingen voor de verbindingengroep wijzigen
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18114127
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747660(v=WS.10)'
---

Registerinstellingen voor de verbindingengroep wijzigen
=======================================================

Als u de systeemprestaties wilt verbeteren, kunt u met vermeldingen in de registersleutel de eigenschappen voor de LDAP-verbindingengroep (Lightweight Directory Access Protocol) in Active Directory instellen die wordt gebruikt door RMS.

Op computers met de 32-bits versie van Windows Server 2003 is de volgende registersleutel het volledige subsleutelpad voor de registervermeldingen van de verbindingengroep:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Op computers met de 64-bits versie van Windows Server 2003 is de volgende registersleutel het volledige subsleutelpad voor de registervermeldingen van de verbindingengroep:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

In de volgende tabel vindt u een overzicht van vermeldingen die u kunt toevoegen om de standaardinstellingen van de Active Directory-verbindingengroep te negeren. De vermelde waarden zijn de standaardwaarden. Zie 'De instellingen van de Active Directory-verbindingengroep optimaliseren' eerder in dit onderwerp voor meer informatie over hoe RMS een zoeklijst maakt en deze instellingen gebruikt.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Naam</th>
<th>Type</th>
<th>Standaardwaarde</th>
<th>Beschrijving</th>
<th>Opmerkingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">Tekenreeks</td>
<td style="border:1px solid black;">name-1, ..., name-n</td>
<td style="border:1px solid black;">Lijst van globale catalogussen gescheiden door komma's (met DNS-namen). Met deze sleutel kan RMS alleen de opgegeven globale catalogussen gebruiken.</td>
<td style="border:1px solid black;">Als u wilt dat RMS geen zoeklijst maakt, geeft u met deze instelling op welke globale catalogussen moeten worden gebruikt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Het minimum aantal globale catalogussen dat beschikbaar moet zijn om RMS te starten.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Het maximum aantal globale catalogussen dat door de algoritme voor het opsporen van topologie wordt toegevoegd aan de zoeklijst.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Het minimum aantal verbindingen dat moet reageren voordat DiscoveryServices begint te zoeken naar globale catalogussen die moeten worden toegevoegd aan de zoeklijst, zodat RMS verzoeken kan accepteren.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Aantal pogingen om opnieuw verbinding te maken voordat wordt vastgesteld dat de verbinding niet reageert.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Aantal seconden dat moet worden gewacht voordat er opnieuw wordt geprobeerd verbinding te maken.</td>
<td style="border:1px solid black;">U hoeft deze standaardinstelling niet te wijzigen, behalve bij uitzonderlijke omstandigheden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Aantal seconden dat moet worden gewacht voordat er opnieuw wordt geprobeerd verbinding te maken met een langzame verbinding.</td>
<td style="border:1px solid black;">U hoeft deze standaardinstelling niet te wijzigen, behalve bij uitzonderlijke omstandigheden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Belang van round robin tijdens taakverdeling.</td>
<td style="border:1px solid black;">Het relatieve belang van round robin in de taakverdeling. De laagste waarde is 1.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Belang van het aantal threads per verbinding tijdens de taakverdeling.</td>
<td style="border:1px solid black;">Het relatieve belang van een laag aantal threads.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Belasting van een langzame verbinding tijdens de taakverdeling.</td>
<td style="border:1px solid black;">Het relatieve belang van een verbinding die niet langzaam is.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Aantal seconden dat moet worden gewacht voordat een aanvraag wordt geblokkeerd om een globale catalogus toe te voegen aan de zoeklijst.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Aantal seconden dat moet worden gewacht voordat er een time-out optreedt voor LDAP API's.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Aantal seconden dat moet worden gewacht voordat er een time-out optreedt voor top-down LDAP-uitbreidingsquery's.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Waarschuwing                                                                                          |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Als u het register onjuist bewerkt, kunt u het systeem ernstig beschadigen. Maak een back-up van alle belangrijke gegevens op de computer voordat u het register wijzigt. |
