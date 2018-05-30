---
TOCTitle: Serverlicentieverleningscertificaten
Title: Serverlicentieverleningscertificaten
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18113836
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720184(v=WS.10)'
---

Serverlicentieverleningscertificaten
====================================

Met een serverlicentieverleningscertificaat wordt aan een RMS-server het recht verleend certificaten en licenties uit te geven. Wanneer de eerste basiscertificeringsserver van uw RMS-implementatie wordt ingericht, ontvangt deze server een serverlicentieverleningscertificaat van de inschrijvingsservice van Microsoft. Dit proces wordt 'inschrijving' genoemd. Het certificaat bevat de openbare sleutel van de basiscertificeringsserver en is ondertekend met de persoonlijke sleutel van de inschrijvingsservice. Voor andere servers die aan het basiscertificeringscluster worden toegevoegd, wordt hetzelfde certificaat gebruikt.

Tijdens het inrichten ontvangt de eerste licentieserver in een cluster een serverlicentieverleningscertificaat van de RMS-basiscertificeringsserver of het RMS-basiscertificeringscluster. Dit proces wordt subinschrijving genoemd. Het certificaat bevat de openbare sleutel van de licentieserver en is ondertekend met de persoonlijke sleutel van de basiscertificeringsserver of het basiscertificeringscluster. Voor andere servers die aan het licentiecluster worden toegevoegd, wordt hetzelfde certificaat gebruikt.

In de volgende tabel worden de rechten beschreven die met serverlicentieverleningscertificaten aan servers worden toegewezen.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Hiermee wordt het recht toegewezen voor het uitgeven van</th>
<th style="border:1px solid black;" >Serverlicentieverleningscertificaat dat is verleend aan een basiscertificeringsserver</th>
<th style="border:1px solid black;" >Serverlicentieverleningscertificaat dat is verleend aan een licentieserver</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Rechtenaccountcertificaten</td>
<td style="border:1px solid black;">Ja</td>
<td style="border:1px solid black;">Nee</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uitgiftelicenties</td>
<td style="border:1px solid black;">Ja</td>
<td style="border:1px solid black;">Ja</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Gebruikslicenties</td>
<td style="border:1px solid black;">Ja</td>
<td style="border:1px solid black;">Ja</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Onderliggende serverlicentieverleningscertificaten</td>
<td style="border:1px solid black;">Ja</td>
<td style="border:1px solid black;">Nee</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Clientlicentieverleningscertificaten</td>
<td style="border:1px solid black;">Ja</td>
<td style="border:1px solid black;">Ja</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720184.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Voor RMS zijn aparte licentieservers of -clusters niet vereist, maar deze kunnen worden gebruikt voor het overnemen van licentieaanvragen die afkomstig zijn van het basiscertificeringscluster. Beheerders kunnen bovendien licentieservers instellen en zodoende tegemoetkomen aan de wensen van interne organisaties die rechtstreekse controle moeten hebben over het uitgeven van beveiligde inhoud. Het kan gebeuren dat in het algemene bedrijfsbeleid, in de sjablonen voor het rechtenbeleid op een basiscertificeringsserver of -cluster wordt opgegeven, enkele rechten niet zijn opgegeven die voor een bepaalde afdeling vereist zijn. In dat geval kan voor de betreffende afdeling een aparte licentieserver of een apart licentiecluster worden geïmplementeerd om de sjablonen voor het rechtenbeleid op te slaan en de licentieaanvragen te verwerken. |
