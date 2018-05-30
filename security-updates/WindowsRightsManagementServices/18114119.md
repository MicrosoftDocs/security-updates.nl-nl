---
TOCTitle: 'IIS-ondersteuning voor RMS'
Title: 'IIS-ondersteuning voor RMS'
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18114119
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747649(v=WS.10)'
---

IIS-ondersteuning voor RMS
==========================

De primaire RMS-services worden geleverd via een verzameling ASP .NET-webservices. Deze webservices worden uitgevoerd in Microsoft® Internet Information Services (IIS). Tijdens het inrichten van de server worden er virtuele mappen ingesteld in IIS. De toepassingsbestanden voor de webservices worden geïnstalleerd in de virtuele mappen.

Tijdens het inrichten van de server kunt u in een lijst met beschikbare websites de website selecteren waaronder u virtuele mappen wilt instellen. Voordat u een server inricht, kunt u een speciale website voor RMS maken. Als u dit doet, kunt u verificatie- en toegangsbeperkingen configureren voor uw specifieke RMS-implementatie.

Standaard worden de webservicebestanden en virtuele mappen met DACL (Discretionary Access Control Lists) beveiligd zodat onbevoegden geen toegang tot de functies hebben. De ACE's (Access Control Entries) voor deze items zijn als volgt ingesteld:

-   De groep Beheerders heeft volledig beheer.
-   Het lokale systeem heeft volledig beheer.
-   De RMS-servicegroep heeft de machtiging Lezen en uitvoeren.
-   Gasten en gebruikers hebben de machtigingen Lezen en uitvoeren, Mapinhoud weergeven en Lezen.
-   Anonieme toegang is niet toegestaan.

In de volgende tabel zijn de virtuele mappen opgenomen die in IIS worden gemaakt en de services die in de virtuele mappen worden geïnstalleerd.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Virtuele map</th>
<th style="border:1px solid black;" >Service</th>
<th style="border:1px solid black;" >Webservicebestand</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Dit is de virtuele map voor RMS-clusterbeheer</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Certification</td>
<td style="border:1px solid black;">Deze virtuele map bevat de services die RMS-certificering ondersteunen</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Activeringsproxy</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Accountcertificering</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Precertificering</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Servicelocator</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Servercertificering</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Certificering van mobiele apparaten</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Inschrijving</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licentie</td>
<td style="border:1px solid black;">Deze virtuele map bevat de services die RMS-licentieverlening ondersteunen</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Licentie</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Uitgifte</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Server</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Servicelocator</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Deze virtuele map bevat de services die RMS-beheer ondersteunen</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Beheer</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">.NET Remoting-interface</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Dit is een submap van DrmRemote.</td>
<td style="border:1px solid black;">Niet van toepassing</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747649.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Voor de beheerservice gelden strengere beperkingen dan voor de andere webservices omdat u RMS kunt configureren met de bijbehorende interfaces. Als gevolg daarvan hebben leden van de groep Gebruikers geen toegang tot de beheerservice. Daarnaast is IP-filtering ingeschakeld, zodat alleen toegang tot de lokale computer is toegestaan. Gastgebruikers hebben geen toegang tot de virtuele map DirectoryServices. De Servicelocatorservice wijst volledig beheer toe aan de NetworkService-account. Als u een licentieserver wilt inrichten, moet u de standaard-ACE's wijzigen zodat toegang voor de RMS-beheerder is toegestaan. |
