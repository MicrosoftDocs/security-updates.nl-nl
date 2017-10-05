---
TOCTitle: 'RMS-clienttechnologieën'
Title: 'RMS-clienttechnologieën'
ms:assetid: '6980468a-fc8c-489b-966f-2921ec268e74'
ms:contentKeyID: 18113962
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720288(v=WS.10)'
---

RMS-clienttechnologieën
=======================

Voor clientcomputers in een RMS-implementatie worden de volgende technologieën gebruikt. Hiermee kunnen gebruikers door RMS beveiligde inhoud maken, uitgeven en gebruiken.

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
<th style="border:1px solid black;" >Technologie</th>
<th style="border:1px solid black;" >Beschrijving</th>
<th style="border:1px solid black;" >Uitgegeven door</th>
<th style="border:1px solid black;" >Meer informatie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Toepassingen met RMS-ondersteuning</td>
<td style="border:1px solid black;">RMS-ondersteuning is vereist voor het maken en uitgeven van door RMS beveiligde inhoud. Toepassingen kunnen speciaal worden ontwikkeld voor RMS en bestaande toepassingen kunnen worden herschreven voor compatibiliteit met RMS.</td>
<td style="border:1px solid black;">Ontwikkelaars van derden.</td>
<td style="border:1px solid black;">Toepassingen met RMS-ondersteuning</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS-computercertificaten</td>
<td style="border:1px solid black;">Hiermee kan een bepaalde computer worden geïdentificeerd als vertrouwd door RMS.</td>
<td style="border:1px solid black;">Activeringsservice voor RMS versie 1.0. Er is geen service nodig om een computercertificaat met RMS SP1 op te halen.</td>
<td style="border:1px solid black;">RMS-computercertificaten</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lockboxes</td>
<td style="border:1px solid black;">Deze lockboxes bevatten de persoonlijke sleutel van de computer en een bijbehorend certificaat waarin de openbare sleutel van de computer is opgenomen.</td>
<td style="border:1px solid black;">Activeringsservice voor RMS versie 1.0. Er is geen service nodig om een lockbox met RMS SP1 op te halen. De lockbox bevat de persoonlijke sleutel van de computer en is daardoor de belangrijkste beveiligings-principal voor codering en decodering.</td>
<td style="border:1px solid black;">Lockboxes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rechtenaccountcertificaten</td>
<td style="border:1px solid black;">Hiermee kan een bepaalde gebruiker worden geïdentificeerd als vertrouwd door RMS.</td>
<td style="border:1px solid black;">Rechtenaccountcertificeringsservice.</td>
<td style="border:1px solid black;">Rechtenaccountcertificaat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Clientlicentiecertificaten</td>
<td style="border:1px solid black;">Hiermee kunnen gebruikers die niet zijn aangesloten op het netwerk, door RMS beveiligde inhoud uitgeven.
(Optioneel)</td>
<td style="border:1px solid black;">Uitgifteservice van RMS.</td>
<td style="border:1px solid black;">Clientlicentiecertificaten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uitgiftelicenties</td>
<td style="border:1px solid black;">Hiermee worden gebruiksrechten voor inhoud gedefinieerd.</td>
<td style="border:1px solid black;">De licentie kan worden uitgegeven door de uitgifteservice van RMS en off line door het clientlicentieverleningscertificaat.</td>
<td style="border:1px solid black;">Uitgiftelicenties</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Gebruikslicenties</td>
<td style="border:1px solid black;">Hiermee kan een gebruiker door RMS beveiligde inhoud verwerken.</td>
<td style="border:1px solid black;">Licentieservice van RMS.</td>
<td style="border:1px solid black;">Gebruikslicenties</td>
</tr>
</tbody>
</table>
