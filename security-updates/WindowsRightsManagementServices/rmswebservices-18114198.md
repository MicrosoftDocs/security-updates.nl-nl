---
TOCTitle: 'RMS-webservices'
Title: 'RMS-webservices'
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18114198
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747728(v=WS.10)'
---

RMS-webservices
===============

RMS levert de servercomponent van een RMS-systeem. De kernfuncties worden geïmplementeerd als een set Microsoft® ASP.NET-webservices die worden uitgevoerd op Microsoft® Internet Information Services (IIS). De RMS-webservices worden beschikbaar gesteld via de SOAP-interface of via externe .NET-aanroepen.

De webservices verzorgen:

-   Subinschrijving van servers
-   Accountcertificering van vertrouwde entiteiten
-   Licentiëren van met rechten beschermde informatie
-   Beheerfuncties van RMS

In de volgende tabel worden de RMS-webservices beschreven.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Service</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Subinschrijving</td>
<td style="border:1px solid black;">Verstrekt onderliggende serverlicentieverleningscertificaten aan servers in clusters exclusief voor licentieverlening. Deze certificaten stellen clusters die exclusief zijn ingericht voor licentieverlening in staat uitgifte- en gebruikslicenties te verstrekken.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Accountcertificering</td>
<td style="border:1px solid black;">Levert rechtenaccountcertificaten aan gebruikers. Gebruikers moeten over deze certificaten beschikken om uitgifte- en gebruikslicenties op te vragen voor het produceren en gebruiken van met rechten beschermde inhoud.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Activeringsproxy</td>
<td style="border:1px solid black;">Deze service is gehandhaafd om compatibel te blijven met versie 1 van de RMS-client. De service geeft aanvragen voor computeractivering door aan de activeringsservice van Microsoft en levert als resultaat lockboxes en RMS-computercertificaten aan versie 1 RMS-clients. Deze service wordt niet gebruikt door RMS-clients met Service Pack 1 (SP1) of later.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uitgeven</td>
<td style="border:1px solid black;">Verstrekt uitgiftelicenties waarmee auteurs met rechten beschermde inhoud kunnen maken en uitgeven. Verstrekt tevens clientlicentieverleningscertificaten waarmee auteurs met rechten beschermde inhoud kunnen uitgeven zonder verbinding te hebben met het interne netwerk waarop RMS is ondergebracht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Licentieverlening</td>
<td style="border:1px solid black;">Verstrekt gebruikslicenties waarmee gebruikers met rechten beschermde inhoud kunnen gebruiken.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Beheer</td>
<td style="border:1px solid black;">Stelt te beheerder in staat RMS te beheren.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">Stelt de webservices in staat onderling te communiceren en met andere componenten van het RMS-systeem door externe .NET-aanroepen beschikbaar te stellen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Uit bedrijf nemen</td>
<td style="border:1px solid black;">Maakt de bescherming ongedaan van inhoud die eerder met rechten werd beveiligd en draagt die over aan de client. Deze service wordt geïnstalleerd door het installatieprogramma van RMS, maar de service heeft geen overeenkomende virtuele hoofdmap in IIS totdat de service wordt ingeschakeld door de beheerder. Met het inschakelen van deze service worden alle andere services uitgeschakeld.</td>
</tr>
</tbody>
</table>
  
Naast de webservices installeert RMS tevens een logboekregistratie-listener-service. Elke webservice verzendt geregistreerde gegevens naar de wachtrij voor logboekregistratieberichten. De service logboekregistratie-listener stuurt de geregistreerde gegevens vervolgens door van de wachtrij naar de logboekdatabase.
  
De webservicetoepassingen bevinden zich in virtuele IIS-mappen. Deze virtuele mappen worden op elke RMS-server geïnstalleerd, onder de website die u hebt geselecteerd tijdens het inrichten.
  
Verificatie en toegang worden afzonderlijk geconfigureerd voor elke virtuele map. Daarnaast wordt toegang voor elke webservice afzonderlijk geconfigureerd. Zie [IIS-ondersteuning voor RMS](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c) verderop in dit onderwerp voor informatie over de beveiligingsinstellingen voor virtuele mappen en webservicesbestanden.
  
Zie [RMS-softwareonderdelen](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca) verderop in dit onderwerp voor meer informatie over elk van de webservices.
