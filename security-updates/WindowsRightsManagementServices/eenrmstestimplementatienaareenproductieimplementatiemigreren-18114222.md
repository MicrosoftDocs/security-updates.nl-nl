---
TOCTitle: 'Een RMS-testimplementatie naar een productie-implementatie migreren'
Title: 'Een RMS-testimplementatie naar een productie-implementatie migreren'
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18114222
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747789(v=WS.10)'
---

Een RMS-testimplementatie naar een productie-implementatie migreren
===================================================================

Veel organisaties kiezen ervoor de implementatie van RMS eerst uit te proberen voordat zij deze technologie in de gehele organisatie toepassen. Het testprogramma heeft normaal gesproken een beperkt aantal gebruikers en de server wordt wellicht lokaal door een beheerder beheerd in plaats van door een IT-groep in een datacenter. Wanneer na het uitvoeren van de test RMS voor alle clients binnen de organisatie in het datacenter wordt geïmplementeerd, zijn er nieuwe RMS-servers voor het grotere aantal mogelijke gebruikers nodig.

Door RMS beveiligde inhoud is echter gekoppeld aan de RMS-server waarmee die inhoud is gemaakt. Als een server wordt verwijderd of vervangen, moeten er dus stappen worden ondernomen zodat de inhoud die met de RMS-testservers is gecodeerd, kan worden gedecodeerd en worden uitgegeven via de RMS-productieservers.

Als u RMS als een testprogramma hebt geïnstalleerd en u wilt de RMS-server in de productieomgeving van uw organisatie opnemen maar u wilt daarbij de integriteit behouden van de inhoud die door de RMS-testserver wordt beveiligd, moet u een migratieschema voor een geruisloze migratie maken en de mogelijkheid inbouwen dat er kan worden teruggegrepen op het testprogramma mocht het nodig zijn gegevens te herstellen.

De volgende procedure is een voorbeeld van de onderdelen die in een migratieschema zouden kunnen worden opgenomen. Binnen uw organisatie zijn er misschien andere stappen nodig.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Server</th>
<th>Stap</th>
<th>Opmerkingen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Test</td>
<td style="border:1px solid black;">Maak een back-up van de RMS-configuratiedatabase.</td>
<td style="border:1px solid black;">Zo kunt u indien nodig de testserver herstellen.
De configuratiedatabase bevat de persoonlijke sleutel van RMS.
Vergeet het wachtwoord van de persoonlijke sleutel niet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Test</td>
<td style="border:1px solid black;">Als u een hardwarebeveiligingsmodule gebruikt voor het beveiligen van de persoonlijke sleutel van RMS, maakt u aan de hand van de richtlijnen van de leverancier een back-up van de configuratie van de hardwarebeveiligingsmodule.</td>
<td style="border:1px solid black;">U gaat de hardwarebeveiligingsmodule op de nieuwe server herstellen.
Zorg dat u alle noodzakelijke onderdelen bij de hand hebt om de beschikbare hardwarebeveiligingsmodule te installeren en te configureren.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Test</td>
<td style="border:1px solid black;">Exporteer het vertrouwd-uitgiftedomeinbestand.</td>
<td style="border:1px solid black;">Zo kan een RMS-server uitgiftelicenties die door deze server zijn gemaakt, decoderen en gebruikslicenties voor de beveiligde inhoud uitgeven.
Het vertrouwde uitgiftedomein bevat het serverlicentieverleningscertificaat, de persoonlijke sleutel van RMS en de eventuele sjablonen voor rechtenbeleid die door deze server zijn ingesteld.
Het vertrouwde uitgiftedomeinbestand is een XML-bestand dat is gecodeerd met een sterk wachtwoord dat u bij het maken van het bestand hebt opgegeven. U hebt dit wachtwoord nodig om het vertrouwde uitgiftedomeinbestand te kunnen importeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Test</td>
<td style="border:1px solid black;">Exporteer het vertrouwde gebruikersdomein.</td>
<td style="border:1px solid black;">Zo kan een RMS-server licenties verstrekken aan gebruikers die hun rechtenaccountcertificaat (RAC) hebben verkregen van de testserver met RMS.
Het vertrouwde gebruikersdomein wordt ingesteld door het serverlicentieverleningscertificaat van deze server naar de andere RMS-server te importeren.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Stel de nieuwe server als de basiscertificeringsserver in.</td>
<td style="border:1px solid black;">Zorg ervoor dat deze server toegang heeft tot de databaseserver en dat IIS en Message Queuing zijn geïnstalleerd.
Gebruik voor deze server indien mogelijk dezelfde servernaam.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Als u een hardwarebeveiligingsmodule gebruikt, installeert u deze en herstelt u de configuratie ervan met behulp van de back-up die u op de testserver hebt gemaakt.</td>
<td style="border:1px solid black;">Stel de referenties in die u nodig hebt om de persoonlijke sleutel van RMS te decoderen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Installeer RMS.</td>
<td style="border:1px solid black;">RMS controleert of alle vereiste services goed zijn geïnstalleerd en geconfigureerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Richt RMS met behulp van een nieuwe persoonlijke sleutel in. Als u on line inschrijving gebruikt, wordt de server tijdens het inrichten ingeschreven bij de inschrijvingsservice van Microsoft waarmee via internet verbinding is gemaakt. Kunt u vanaf deze server geen verbinding met internet maken, dan moet u gebruikmaken van off line inschrijving.</td>
<td style="border:1px solid black;">Heeft deze server een andere naam dan de testserver, dan kunt u de URL van het cluster gelijkmaken aan de URL van de testserver.
Als u dat niet doet, zult u een URL-omleiding van de vorige cluster-URL naar de nieuwe cluster-URL moeten instellen om gebruikers met reeds bestaande inhoud licenties te kunnen verstrekken.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Als u off line inschrijving gebruikt, moet u de nieuwe RMS-server handmatig inschrijven. Zie 'Handmatig een basiscertificeringsserver inschrijven' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.</td>
<td style="border:1px solid black;">De RMS-server kan pas worden gebruikt als deze is ingeschreven.
Dat geldt ook voor de RMS-beheerpagina's die pas kunnen worden geopend wanneer de server is ingeschreven.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Importeer het vertrouwde uitgiftedomeinbestand dat u in stap 3 hebt geëxporteerd.</td>
<td style="border:1px solid black;">De RMS-serviceaccount moet leesmachtigingen hebben voor de locatie waar het bestand is opgeslagen, om het bestand te kunnen importeren.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Onderteken elke sjabloon opnieuw die met het vertrouwde uitgiftedomein is geïmporteerd.</td>
<td style="border:1px solid black;">De sjablonen zijn met de persoonlijke sleutel van de server ondertekend. Omdat deze server een nieuwe persoonlijke sleutel heeft, zijn de sjablonen alleen geldig als ze opnieuw worden ondertekend. Zie 'Een sjabloon voor het rechtenbeleid opnieuw ondertekenen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Distribueer de sjablonen opnieuw naar de clientcomputers die hebben deelgenomen aan de test.</td>
<td style="border:1px solid black;">De oude sjablonen moeten worden verwijderd en worden vervangen door de sjablonen die door deze server zijn ondertekend.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Productie</td>
<td style="border:1px solid black;">Importeer het vertrouwd-gebruiksdomeinbestand dat u in stap 4 hebt geëxporteerd.</td>
<td style="border:1px solid black;">Hierdoor kunnen oude clientlicentieverleningscertificaten en RAC's worden gebruikt.
Als er als onderdeel van deze migratie gebruikersaccounts tussen forests zijn verplaatst, moeten de accounts bijbehorende SMTP-proxyservers hebben.</td>
</tr>
</tbody>
</table>
 

Nadat u de instelling op de productieserver hebt geconfigureerd, controleert u of de testgebruikers nog altijd eerder beveiligde e-mail kunnen lezen en nieuwe beveiligde e-mail kunnen maken. Vervolgens kunt u net zoveel RMS-servers aan het cluster toevoegen als u nodig hebt voor het aantal gebruikers binnen uw organisatie.
