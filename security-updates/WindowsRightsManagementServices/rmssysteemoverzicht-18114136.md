---
TOCTitle: 'RMS-systeem: overzicht'
Title: 'RMS-systeem: overzicht'
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18114136
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747671(v=WS.10)'
---

RMS-systeem: overzicht
======================

Dit onderwerp bevat informatie over de wijze waarop de RMS-webservices en RMS-clienttechnologieën samenwerken in een RMS-systeem.

In de volgende tabel worden de servertypen en de bijbehorende functies beschreven die worden gebruikt in een RMS-implementatie. Zie 'Een RMS-systeem implementeren' in deze documentatie voor gedetailleerde informatie over implementaties.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Server of cluster</th>
<th>Functie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Basiscertificering</td>
<td style="border:1px solid black;">Hiermee worden de volgende RMS-services uitgevoerd:
<ul>
<li><strong>Subinschrijving</strong>. Hiermee wordt een subinschrijving van licentieservers uitgevoerd.<br />
<br />
</li>
<li><strong>Activeringsproxy</strong>. Deze proxy fungeert als een internetproxy bij clientaanvragen voor lockboxes en RMS-computercertificaten.<br />
<br />
</li>
<li><strong>Certificering</strong>. Hiermee worden rechtenaccountcertificaten uitgegeven.<br />
<br />
</li>
<li><strong>Uitgifte</strong>. Hiermee worden uitgiftelicenties uitgegeven.<br />
<br />
</li>
<li><strong>Licentieverlening</strong>. Hiermee worden gebruikslicenties uitgegeven.<br />
<br />
</li>
</ul>
Elke implementatie moet minstens één basiscertificeringsserver of -cluster bevatten. Per Active Directory-forest kan slechts één basiscertificeringscluster aanwezig zijn.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Licentieverlening (optioneel)</td>
<td style="border:1px solid black;">Hiermee worden de volgende RMS-services uitgevoerd:
<ul>
<li><strong>Uitgifte</strong>. Hiermee worden uitgiftelicenties uitgegeven.<br />
<br />
</li>
<li><strong>Licentieverlening</strong>. Hiermee worden gebruikslicenties uitgegeven.<br />
<br />
</li>
</ul>
Licentieservers worden vaak geïmplementeerd ter ondersteuning van afzonderlijke afdelingen of met het doel het basiscertificeringscluster te ontlasten door de verwerking van licentieaanvragen over te nemen. Licentieservers zijn optioneel.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Databaseserver, zoals SQL Server</td>
<td style="border:1px solid black;"><ul>
<li>Hiermee worden de configuratiedatabases, logboekdatabases en databases met adreslijstservices van RMS uitgevoerd.<br />
<br />
</li>
<li>De rechtenaccountcertificaten worden opgeslagen in de configuratiedatabase van het basiscertificeringscluster.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Domeincontrollers en globale catalogus</td>
<td style="border:1px solid black;"><ul>
<li>Hiermee worden gebruikersverificaties en adreslijstservices uitgevoerd.<br />
<br />
</li>
<li>Hiermee wordt de locatie voor het opsporen van services in het basiscertificeringscluster opgeslagen.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

RMS gebruikt de inschrijvings- en activeringsservices waarvoor Microsoft als host optreedt om een gemeenschappelijke vertrouwensbasis voor het systeem te bieden. Zie '[RMS-vertrouwenshiërarchie](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)' verderop in dit onderwerp voor meer informatie.

In het volgende schema worden de verschillende onderdelen van een RMS-systeem en de functies van deze onderdelen in het systeem weergegeven. De pijlen staan voor de aanvragen en antwoorden die van en naar de verschillende onderdelen worden verstuurd.

![](images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Zie '[RMS-softwareonderdelen](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca)' verderop in dit onderwerp voor meer informatie over elk onderdeel.
