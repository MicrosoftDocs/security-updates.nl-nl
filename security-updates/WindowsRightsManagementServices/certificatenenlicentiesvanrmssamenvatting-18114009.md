---
TOCTitle: 'Certificaten en licenties van RMS: samenvatting'
Title: 'Certificaten en licenties van RMS: samenvatting'
ms:assetid: '637ccfca-318e-4346-85b5-0945b058fb9c'
ms:contentKeyID: 18114009
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747595(v=WS.10)'
---

Certificaten en licenties van RMS: samenvatting
===============================================

De volgende tabel bevat de certificaten en licenties die door RMS worden gebruikt. Deze worden uitvoerig beschreven in de overige onderwerpen in dit gedeelte.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Certificaat of licentie</th>
<th style="border:1px solid black;" >Doel</th>
<th style="border:1px solid black;" >Inhoud</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serverlicentieverleningscertificaten</td>
<td style="border:1px solid black;">Met het serverlicentieverleningscertificaat dat aan licentieservers wordt uitgegeven, kunnen de volgende items worden uitgegeven:
<ul>
<li>Uitgiftelicenties<br />
<br />
</li>
<li>Gebruikslicenties<br />
<br />
</li>
<li>Clientlicentieverleningscertificaten<br />
<br />
</li>
<li>Sjablonen voor het rechtenbeleid<br />
<br />
</li>
</ul>
Met het serverlicentieverleningscertificaat dat aan het basiscertificeringscluster wordt uitgegeven, kunnen daarnaast ook de volgende items worden uitgegeven:
<ul>
<li>rechtenaccountcertificaten aan clients<br />
<br />
</li>
<li>serverlicentieverleningscertificaten aan licentieservers<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Het serverlicentieverleningscertificaat dat aan een licentieserver wordt uitgegeven, bevat de openbare sleutel van de licentieserver.
Het serverlicentieverleningscertificaat dat aan de basiscertificeringsserver wordt uitgegeven, bevat de openbare sleutel van de basiscertificeringsserver.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Clientlicentieverleningscertificaten</td>
<td style="border:1px solid black;">Hiermee kan een gebruiker ook door RMS beveiligde inhoud uitgeven als de computer geen verbinding heeft met het bedrijfsnetwerk.</td>
<td style="border:1px solid black;">Deze certificaten bevatten de openbare sleutel van het certificaat en de persoonlijke sleutel van het certificaat die is gecodeerd met de openbare sleutel van de gebruiker die het certificaat heeft aangevraagd. Deze certificaten bevatten daarnaast de openbare sleutel van de server waarmee het certificaat is uitgegeven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS-computercertificaten</td>
<td style="border:1px solid black;">Hiermee worden computers en apparaten geïdentificeerd die worden vertrouwd door het RMS-systeem.</td>
<td style="border:1px solid black;">Deze certificaten bevatten de openbare sleutel van de geactiveerde computer. De bijbehorende persoonlijke sleutel is opgenomen in de lockbox van die computer.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rechtenaccountcertificaat</td>
<td style="border:1px solid black;">Hiermee wordt een gebruiker in de context van een specifieke computer of specifiek apparaat herkend.</td>
<td style="border:1px solid black;">Deze certificaten bevatten de openbare sleutel van de gebruiker en de persoonlijke sleutel van de gebruiker, die is gecodeerd met de openbare sleutel van de geactiveerde computer.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Uitgiftelicenties</td>
<td style="border:1px solid black;">Hiermee worden de rechten opgegeven die van toepassing zijn op de door RMS beveiligde inhoud.</td>
<td style="border:1px solid black;">Deze licenties bevatten de symmetrische inhoudssleutel voor het decoderen van de inhoud die is gecodeerd met de openbare sleutel van de server waarmee de licentie is uitgegeven.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Gebruikslicenties</td>
<td style="border:1px solid black;">Hiermee worden de rechten opgegeven die van toepassing zijn op de door RMS beveiligde inhoud in de context van een bepaalde geverifieerde gebruiker.</td>
<td style="border:1px solid black;">Deze licenties bevatten de symmetrische inhoudsleutel voor het decoderen van de inhoud. Deze sleutel is gecodeerd met de openbare sleutel van de gebruiker.</td>
</tr>
</tbody>
</table>
