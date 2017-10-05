---
TOCTitle: Beveiliging tijdens de inrichting
Title: Beveiliging tijdens de inrichting
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18114079
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747616(v=WS.10)'
---

Beveiliging tijdens de inrichting
=================================

Met de RMS-beheerwebsite kunt u RMS-bronnen inrichten op een bestaande website. Tijdens de inrichting worden er virtuele mappen en toepassingengroepen op deze website gemaakt en worden er RMS-databases op een databaseserver gemaakt en geconfigureerd. Als de server een internetverbinding heeft, kan de server tijdens het inrichten bij de inschrijvingsservice van Microsoft worden ingeschreven.

In de volgende tabel worden de accounts beschreven die tijdens de inrichting worden gebruikt in RMS.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Account</th>
<th>Doel</th>
<th>Machtigingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Account van de aangemelde gebruiker</td>
<td style="border:1px solid black;">Hiermee worden virtuele mappen en toepassingengroepen gemaakt. Voor IIS is Windows-verificatie vereist. In RMS wordt de aangemelde gebruiker geïmiteerd die lokaal moet zijn aangemeld.</td>
<td style="border:1px solid black;">Volledig beheer (de aangemelde gebruiker moet een lokale beheerder zijn).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Systeemaccount</td>
<td style="border:1px solid black;">Hiermee wordt de tijdelijke assemblage voor serialisatie gemaakt.</td>
<td style="border:1px solid black;">Lees- en schrijfmachtigingen voor de tijdelijke Windows-map C:\Windows\Temp.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ASPNET-account</td>
<td style="border:1px solid black;">Hiermee wordt de tijdelijke assemblage van de ASPX-bestanden gemaakt.</td>
<td style="border:1px solid black;">Standaard toegang tot de cachemap C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files voor de tijdelijke assemblage.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">NetworkService-account</td>
<td style="border:1px solid black;">Hiermee wordt het serviceverbindingspunt in Active Directory geregistreerd.</td>
<td style="border:1px solid black;"><ul>
<li>Alleen-lezenmachtigingen voor de inrichtingssite (doorgaans C:\Inetpub\Wwwroot\Provisioning).<br />
<br />
</li>
<li>Lees- en schrijfmachtigingen voor de registersleutel <strong>DRMS</strong>. De machtigingen worden toegewezen door het installatieprogramma van RMS. Hierin wordt tevens de volgende registersleutel gemaakt.<br />
<br />
Op computers met de 32-bits versie van Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
Op computers met de 64-bits versie van Windows Server 2003<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

Tijdens het inrichten voert RMS de volgende taken uit:

-   Op de databaseserver:
    -   Configuratiedatabases, databases met adreslijstservices en logboekdatabases maken.
    -   Aanmeldingsmachtigingen toewijzen aan de RMS-servicegroep.
    -   Opgeslagen procedures installeren in de databases en uitvoeringsmachtigingen toewijzen aan de RMS-servicegroep.
    -   Query's uitvoeren in de hoofddatabase.
-   De RMS-servicegroep toevoegen aan de groep IIS\_WPG.
-   In C:\\Inetpub\\Wwwroot\\\_wmcs een hiërarchie maken van virtuele mappen, bestanden en toepassingengroepen voor de webservices en de RMS-beheerwebsite.
-   DACL's instellen voor de virtuele mappen, bestanden en toepassingengroepen.
-   Toegang tot de tijdelijke map verlenen aan de RMS-servicegroep.
-   Als u beveiliging voor de softwaresleutel instelt, wordt de persoonlijke sleutel van de serverlicentie gecodeerd voordat deze wordt opgeslagen in de database. In RMS wordt tijdens het inrichten een wachtwoord aangevraagd en er wordt op computerniveau toegang verkregen tot de DPAPI.
-   De service van de logboekregistratie-listener installeren.
-   Een wachtrij voor logboekregistratieberichten maken.
-   Het serviceverbindingspunt in Active Directory instellen bij het inrichten van de basiscertificeringsserver.
