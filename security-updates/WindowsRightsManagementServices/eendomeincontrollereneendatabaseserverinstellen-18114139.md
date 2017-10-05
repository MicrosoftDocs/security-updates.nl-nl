---
TOCTitle: Een domeincontroller en een databaseserver instellen
Title: Een domeincontroller en een databaseserver instellen
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18114139
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747681(v=WS.10)'
---

Een domeincontroller en een databaseserver instellen
====================================================

Voordat u een basiscertificeringsserver of licentieserver installeert, dient u te controleren of u de juiste domein- en database-ondersteuning hebt geïmplementeerd met behulp van Active Directory alsmede een databaseserver hebt geïmplementeerd, zoals SQL Server 2000 met Service Pack 3 (SP3) of Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) versie A. Hoewel de vereiste onderdelen wellicht al worden uitgevoerd in de productieomgeving, is het raadzaam de productieomgeving niet voor het testen te gebruiken.

Met de volgende procedures worden een domeincontroller en een database op één computer in een geïsoleerd netwerk ingesteld voor testdoeleinden voor een server.

| ![](images/Cc747681.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| In dit voorbeeld wordt de databaseserver uitgevoerd op de domeincontroller. In een productieomgeving kunt u de domeincontroller beter niet laten optreden als host voor andere onderdelen. Active Directory en de databaseserver worden in dit voorbeeld op dezelfde computer geïnstalleerd zodat de volledige infrastructuur op een minimumaantal computers kan worden geïnstalleerd. |

Als u MSDE 2000 als uw databaseserver wilt gebruiken, dient u er wel rekening mee te houden dat er dan geen netwerkinterfaces worden ondersteund en dat door de voorwaarden voor het gebruik van MSDE 2000 u geen SQL Server-clienthulpprogramma's bij een MSDE-database kunt gebruiken. Door deze beperking kunt u geen logboekgegevens weergeven of opgeslagen gegevens in de configuratiedatabase wijzigen. Daarom raden wij aan MSDE 2000 alleen in testomgevingen voor het ondersteunen van RMS-databases te gebruiken.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Infrastructuuronderdeel</th>
<th>Procedure voor het instellen van een domeincontroller en een databaseserver</th>
<th>Opmerkingen voor implementatie in een productieomgeving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Besturingssysteem</td>
<td style="border:1px solid black;">Installeer Windows 2000 Server met SP3 of hoger of Windows 2003 Server op een computer die voldoet aan de hardwarevereisten voor RMS, maar nog niet is aangesloten op een netwerk. Gebruik het NTFS-bestandssysteem voor de partitie.</td>
<td style="border:1px solid black;">U wordt aangeraden altijd het recentste Service Pack en de recentste updates te installeren. Gebruik partities met NTFS-formattering.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netwerkverbinding</td>
<td style="border:1px solid black;">Maak verbinding met een netwerk dat met internet is verbonden maar dat geïsoleerd is van de productieomgeving.</td>
<td style="border:1px solid black;">Voor de internetverbinding moet een geschikte firewall zijn ingesteld.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IP-adres</td>
<td style="border:1px solid black;">Wijs een statisch IP-adres aan deze computer toe.</td>
<td style="border:1px solid black;">Gebruik altijd statische IP-adressen voor servers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Active Directory</td>
<td style="border:1px solid black;">Meld u aan als lokale beheerder.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Klik op <strong>Start</strong>, klik op <strong>Uitvoeren</strong>, typ <code>dcpromo</code> in het vak <strong>Openen</strong> en klik op <strong>OK</strong>.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">In de wizard Active Directory installeren maakt u een nieuw domein in een nieuw forest en accepteert u met uitzondering van de volgende opties de standaardopties:
Geef de domeinnaam op, bijvoorbeeld contos.com.
Geef in de wizard op dat DNS op de computer moet worden geconfigureerd.
Selecteer <strong>Machtigingen die alleen compatibel zijn met Windows 2000-servers</strong> als op alle domeincontrollers Windows 2000 of hoger wordt uitgevoerd.
Geef een sterk wachtwoord op voor de lokale beheerder.</td>
<td style="border:1px solid black;">Als er nieuwe domeinen vereist zijn om RMS te implementeren, maakt u deze in Active Directory.
Gebruik altijd sterke wachtwoorden voor accounts.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Start de computer opnieuw op als hierom wordt gevraagd.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Als u het functionele niveau wilt controleren, opent u de module <strong>Active Directory: gebruikers en computers</strong>, klikt u met de rechtermuisknop op de domeinnaam, kiest u <strong>Eigenschappen</strong> en controleert u de instellingen in het vak <strong>Domeinmodus</strong>. Als er geen domeincontrollers van voor Windows 2000 aanwezig zijn, klikt u op <strong>Modus wijzigen</strong> als u de domeinmodus wilt wijzigen in <strong>Native modus</strong>.
Opmerking: In Windows Server 2003 is de instelling <strong>Domeinmodus</strong> vervangen door <strong>Domeinfunctionaliteitsniveau</strong>.</td>
<td style="border:1px solid black;">Als u een optimale beveiliging en beheermogelijkheden wilt, moet u niet het gemengde functionaliteitsniveau van Windows 2000 voor ondersteuning van RMS gebruiken.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Gebruikersaccounts</td>
<td style="border:1px solid black;">Maak een domeingebruikersaccount die moet worden gebruikt als RMS-serviceaccount voor RMS, bijvoorbeeld ContosoRMS@contoso.com. Geef een sterk wachtwoord op. Geef een e-mailadres op voor de gebruiker. Als het e-mailadres niet in Active Directory is opgegeven, kan de gebruiker geen licenties en certificaten van RMS krijgen.
Opmerking: Gebruik als RMS-serviceaccount niet de domeinaccount waarmee RMS is geïnstalleerd.</td>
<td style="border:1px solid black;">In Active Directory moet u een afzonderlijke account maken die moet worden gebruikt als RMS-serviceaccount. Neem een e-mailadres op. Wijs geen speciale machtigingen aan deze account toe.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2000:</td>
<td style="border:1px solid black;">Meld u aan bij de server waarop u de database wilt installeren. Als dit dezelfde server is als de domeincontroller, moet u zich aanmelden als domeinbeheerder.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Installeer de software van de databaseserver aan de hand van de bijgeleverde instructies.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Hieronder staan enkele tips voor het installeren van de databaseserver:
<ul>
<li>Geef een naam op voor de beheerdersaccount voor het databasesysteem en de organisatie, bijvoorbeeld Contoso.<br />
<br />
</li>
<li>Geef een sterk wachtwoord voor de systeembeheerder op.<br />
<br />
</li>
<li>Gebruik de geïntegreerde verificatiemethoden van Windows.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">U moet een geïntegreerde verificatiemodus van Windows gebruiken. Als deze databaseserver niet kan worden uitgevoerd in deze modus, neemt u contact op met de domeinbeheerder en de beheerder van de databaseserver om te bepalen welke wijzigingen moeten worden doorgevoerd in de RMS-instellingen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Controleer of de databaseservice is beëindigd.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Installeer de software-updates voor de databaseserver. Wanneer naar een wachtwoord wordt gevraagd, gebruikt u het wachtwoord dat u tijdens de installatie hebt opgegeven.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Start de computer opnieuw op. Controleer of de databaseservice is gestart.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Controleer of er voor de gebruikersaccounts geldige e-mailadressen zijn ingesteld in Active Directory.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Zorg dat de domeingebruiker die RMS moet beheren en de basiscertificerings- en licentieservers moet inrichten, over de vereiste machtigingen voor de databaseserver beschikt. Als u SQL Server als de databaseserver gebruikt, kunt u een aanmeldings-id toevoegen voor de gebruiker die de module <strong>SQL Server Enterprise Manager</strong> gebruikt. Vouw in de module de server en de servergroep uit en vouw vervolgens het item <strong>Beveiliging</strong> uit. Klik op het item <strong>Aanmeldingen</strong> en voeg een nieuwe aanmelding toe voor de domeinaccount van de gebruiker. Klik vervolgens op de tab <strong>Serverfuncties</strong> en schakel het selectievakje <strong>Serverbeheerders</strong> in.</td>
<td style="border:1px solid black;">Belangrijk: Voor alle gebruikers en groepen die met RMS licenties willen aanvragen en inhoud willen uitgeven, moet in de MMC-module Active Directory: gebruikers en groepen een e-mailadres voor de account zijn ingesteld op het tabblad <strong>Algemeen</strong> in <strong>Eigenschappen</strong>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetverbinding
(optioneel)</td>
<td style="border:1px solid black;">Controleer of uw browser en server (inclusief vereiste proxyserverconfiguraties, TCP/IP en LMHOSTS/HOSTS) correct zijn geconfigureerd voor toegang tot internet. Test dit door naar http://uddi.microsoft.com te gaan. Als u deze pagina kunt openen, kan er met RMS verbinding met de inschrijvingsservice van Microsoft worden gemaakt.</td>
<td style="border:1px solid black;">Ga naar http://uddi.microsoft.com om te controleren of u toegang hebt tot internet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Software-updates</td>
<td style="border:1px solid black;">Download en installeer de meest recente updates voor de software die op deze computer is geïnstalleerd, en de laatste Windows-updates van www.microsoft.com.</td>
<td style="border:1px solid black;">Download en installeer altijd de meest recente service-updates.</td>
</tr>
</tbody>
</table>
  
Als u de bovenstaande stappen hebt uitgevoerd, kunt u de installatie van RMS voorbereiden op de computers. Het installeren van vereiste software maakt deel uit van deze voorbereiding.
