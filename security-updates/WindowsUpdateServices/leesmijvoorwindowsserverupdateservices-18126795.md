---
TOCTitle: Leesmij voorWindows Server Update Services
Title: Leesmij voorWindows Server Update Services
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18126795
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720505(v=WS.10)'
---

Leesmij voorWindows Server Update Services
==========================================

In dit document worden kwesties beschreven die betrekking hebben op Windows Server Update Services (WSUS). Het document bevat aanbevelingen en vereisten voor het installeren van WSUS.

| ![](images/Cc720505.note(WS.10).gif)Opmerking                                                                                                              |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U kunt een exemplaar van dit document downloaden via het Downloadcentrum van Microsoft op [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126). |

Voordat u begint
----------------

#### Kwestie 1: IIS moet zijn geïnstalleerd

Voor Microsoft® Windows Server™ Update Services (WSUS) moet IIS (Internet Information Services) zijn geïnstalleerd. Onder Microsoft Windows Server 2003 en Microsoft Windows® 2000 Server wordt IIS evenwel niet standaard geïnstalleerd, zodat de installatie van Windows Server Update Services mogelijk niet kan worden voortgezet en er een foutbericht verschijnt met de mededeling dat IIS niet is geïnstalleerd.

IIS installeren:

1.  Open het Configuratiescherm.
2.  Dubbelklik op **Software**.
3.  Klik op **Windows-onderdelen toevoegen of verwijderen**.
4.  Klik in de lijst **Onderdelen** op **Toepassingsserver**.
5.  Klik op **Details**.
6.  Schakel het selectievakje **ASP.NET** in. Schakel **COM+-netwerktoegang** in. IIS (Internet Information Services) wordt nu automatisch geselecteerd.
7.  Selecteer **Internet Information Services (IIS)** en klik vervolgens op **Details** om de lijst met optionele IIS-onderdelen weer te geven.
8.  Selecteer alle optionele onderdelen die u wilt installeren. Het optionele onderdeel World Wide Web-service bevat belangrijke subonderdelen, zoals Active Server Pages en Extern beheer (HTML). Klik op World Wide Web-service en vervolgens op Details als u deze subonderdelen wilt weergeven en selecteren. Klik op OK totdat u bent teruggekeerd bij de wizard Windows-onderdelen.
9.  Klik op **Volgende** en voltooi de wizard Windows-onderdelen.
10. Nadat u IIS hebt geïnstalleerd, kunt u Windows Server Update Services installeren.

#### Kwestie 2: voor servers waarop Windows 2000 Server wordt uitgevoerd, moet ten minste één website aanwezig zijn in IIS voordat u WSUS installeert

Mogelijk kan er tijdens de installatie van Windows Server Update Services geen website worden gemaakt als er geen sites aanwezig zijn in IIS wanneer de installatie wordt uitgevoerd. Dit kan bijvoorbeeld gebeuren indien u een SUS 1.0-site (Software Update Services) als enige site in IIS had en u deze hebt verwijderd voorafgaand aan de installatie van WSUS.

In dat geval moet u een nieuwe website maken met de module IIS-beheer. Daarna kunt u deze site selecteren of een nieuwe site opgeven tijdens de installatie van WSUS.

Als u al hebt geprobeerd om WSUS te installeren en de installatie is mislukt omdat er geen sites aanwezig waren, opent u de module IIS-beheer en verwijdert u de site met de naam 'Web Site \#1'. Vervolgens voert u de eerder beschreven stappen uit en herhaalt u de installatie opnieuw.

#### Kwestie 3: Noodzakelijke onderdelen installeren

#### Softwarevereisten

In de volgende tabel wordt de vereiste software voor elk ondersteund besturingssysteem weergegeven. Zorg dat de WSUS-server voldoet aan de vereisten in deze lijst voordat u de installatie van WSUS uitvoert. Als een van deze updates vereist dat de computer opnieuw wordt opgestart wanneer de installatie is voltooid, moet u de server opnieuw starten voordat u WSUS installeert.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Besturingssysteem</th>
<th style="border:1px solid black;" >Vereisten</th>
<th style="border:1px solid black;" >Downloads</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alle besturingssystemen</td>
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS) 5.0</td>
<td style="border:1px solid black;">Moet worden geïnstalleerd vanuit het besturingssysteem.
Zie Kwestie 1: IIS moet zijn geïnstalleerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alle besturingssystemen</td>
<td style="border:1px solid black;">Background Intelligent Transfer Service (BITS) 2.0</td>
<td style="border:1px solid black;">Raadpleeg voor Windows Server 2003-besturingssystemen het <a href="http://go.microsoft.com/fwlink/?linkid=47251">artikel met informatie over de update voor Background Intelligent Transfer Service (BITS) 2.0 en WinHTTP 5.1 Windows Server 2003</a> (KB842773) in het Downloadcentrum (http://go.microsoft.com/fwlink/?LinkId=47251).
Raadpleeg voor Windows Server 2000-besturingssystemen het <a href="http://go.microsoft.com/fwlink/?linkid=46794">artikel met informatie over de update voor Background Intelligent Transfer Service (BITS) 2.0 en WinHTTP 5.1 Windows Server 2000</a> (KB842773) in het Downloadcentrum (http://go.microsoft.com/fwlink/?LinkId=46794).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1 voor Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1,1 Service Pack 1 voor Windows Server 2003</a>
U kunt ook naar <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> gaan en controleren welke Essentiële updates en Service Packs beschikbaar zijn. Installeer Microsoft .NET Framework 1.1 Service Pack 1 voor Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Databasesoftware die volledig compatibel is met Microsoft SQL</td>
<td style="border:1px solid black;">N.v.t.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Databasesoftware die volledig compatibel is met Microsoft SQL</td>
<td style="border:1px solid black;">Als u geen Microsoft SQL Server 2000 gebruikt, kunt u Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) installeren. Hiervoor moet u diverse stappen uitvoeren. Zie MSDE installeren onder Windows 2000 verderop voor meer informatie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft Internet Explorer 6.0 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Herdistribueerbaar pakket voor Microsoft .NET Framework versie 1.1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Herdistribueerbaar pakket voor Microsoft .NET Framework versie 1.1</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
U kunt ook naar <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> gaan en controleren welke Essentiële updates en Service Packs beschikbaar zijn. Installeer Microsoft .NET Framework 1.1 Service Pack 1 voor Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Naast deze vereisten is het mogelijk dat tijdens de installatie van WSUS zo nodig ASP.NET versie 1.1 op uw server wordt geïnstalleerd of geconfigureerd. (Tijdens de installatie van WSUS wordt ASP.NET geconfigureerd.)

#### MSDE 2000 installeren onder Windows 2000

Als u Windows 2000 voor WSUS gebruikt en u geen toegang tot Microsoft SQL Server 2000 hebt, moet u Microsoft SQL Server 2000 Desktop Engine (MSDE) installeren voordat u WSUS installeert. Als u MSDE al hebt geïnstalleerd op uw WSUS-server, hoeft u geen speciaal exemplaar van MSDE in te stellen voor WSUS. U kunt eenvoudig de naam van het bestaande exemplaar opgeven tijdens de installatie van WSUS.

Het installeren van MSDE onder Windows 2000 Server is een proces van vier stappen. Allereerst moet u het MSDE-archief naar een map op uw WSUS-server downloaden en decomprimeren. Vervolgens gebruikt u een opdrachtprompt en opdrachtregelopties om de installatie van MSDE uit te voeren, het systeembeheerderswachtwoord in te stellen en WSUS toe te wijzen als de naam van het exemplaar. Wanneer de installatie van MSDE is voltooid, moet u controleren of het WSUS-exemplaar wordt uitgevoerd als een NT-service. Ten slotte moet u een beveiligingsupdate toevoegen aan MSDE om uw WSUS-server te beveiligen.

#### Stap 1: download het MSDE-archief en decomprimeer het

U moet het MSDE-archief naar een map op uw WSUS-server downloaden en decomprimeren. Zie [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Stap 2: installeer MSDE

Gebruik een opdrachtprompt en opdrachtregelopties om de installatie van MSDE uit te voeren, het systeembeheerderswachtwoord in te stellen en WSUS toe te wijzen als de naam van het exemplaar. Wanneer de installatie van MSDE is voltooid, moet u controleren of het WSUS-exemplaar wordt uitgevoerd als een NT-service.

Als u MSDE wilt installeren, stelt u het systeembeheerderswachtwoord in en geeft u de naam voor een exemplaar op:

1.  Navigeer in een opdrachtvenster naar de installatiemap voor MSDE die is opgegeven in 'Stap 1: download het MSDE-archief en decomprimeer het.'
2.  Typ het volgende: **setup sapwd="***wachtwoord***" naamexemplaar=WSUS**
    waarbij *wachtwoord* een sterk wachtwoord voor de systeembeheerdersaccount op dit exemplaar van MSDE is en **naamexemplaar** de naam van het database-exemplaar is. U kunt ook de standaardnaam van het exemplaar (in plaats van 'WSUS') gebruiken voor uw WSUS-database. Als u dat doet, hoeft u niet **naamexemplaar=WSUS** op te geven als opdrachtregelparameter. Met deze opdracht wordt het installatieprogramma voor MSDE gestart, het systeembeheerderswachtwoord ingesteld en de naam van dit MSDE-exemplaar ingesteld op een waarde die u opgeeft.

#### Stap 3: controleer of het WSUS-exemplaar van MSDE is geïnstalleerd

U moet controleren of u het WSUS-exemplaar van MSDE kunt zien.

1.  Klik achtereenvolgens op **Start** en **Uitvoeren**.
2.  Typ **services.msc** in het vak **Openen** en klik op **OK**.

Schuif omlaag in de lijst met services en controleer of een service met de naam MSSQL$WSUS (als u 'WSUS' hebt gebruikt als de naam van het exemplaar) of MSSQLSERVER (als u de standaardnaam voor het exemplaar hebt gebruikt) bestaat.

#### Stap 4: start het MSDE-exemplaar.

Aan het einde van de installatie van MSDE moet u het exemplaar starten. Als u 'WSUS' hebt gebruikt als de naam van het exemplaar, moet u 'MSSQL$WSUS' starten. Als u de standaardnaam van het exemplaar hebt gebruikt, moet u MSSQLSERVER starten. Alleen als u deze service start, kan WSUS gebruikmaken van het database-exemplaar.

#### Stap 5: werk MSDE bij

U moet de beveiligingsupdate downloaden en installeren die wordt beschreven in bulletin [MS03-031: Cumulatieve beveiligingspatch voor SQL Server](http://go.microsoft.com/fwlink/?linkid=47364).

Zie [SQL Server 2000 (32-bit) Beveiligingspatch MS03-031](http://go.microsoft.com/fwlink/?linkid=47363) als u deze beveiligingsupdate wilt downloaden.

#### Kwestie 4: Minimale eisen die worden gesteld aan de schijfruimte

Hier volgen de minimale eisen die worden gesteld aan de schijfruimte voor het installeren van Windows Server Update Services:

-   1 GB (gigabyte) op de systeempartitie
-   2 GB voor het volume waarop de databasebestanden worden opgeslagen
-   6 GB, gebaseerd op de verwachte aantallen gegevens

#### Kwestie 5: voordat u de laatste versie van WSUS installeert, moet u voorgaande versies verwijderen met het onderdeel Software

Als u WSUS wilt installeren op een server waarop Windows Update Services Beta 1 of Beta 2 is geïnstalleerd, moet eerst voorgaande versies verwijderen met het onderdeel Software in het Configuratiescherm.

#### Kwestie 6: voor WSUS is het vereist dat de optie voor geneste triggers in SQL Server wordt ingeschakeld

Deze optie is standaard ingeschakeld, maar kan worden uitgeschakeld door een SQL Server-beheerder.

Als u van plan bent een SQL Server-database als gegevensarchief voor Windows Server Update Services te gebruiken, moet de SQL Server-beheerder controleren of de optie voor geneste triggers is ingeschakeld voordat de WSUS-beheerder WSUS installeert en de database opgeeft tijdens de installatie.

Tijdens de installatie van WSUS wordt de databasespecifieke optie RECURSIVE\_TRIGGERS ingeschakeld. De optie voor geneste triggers wordt echter niet ingeschakeld, omdat dit een algemene optie is die geldt voor de gehele server.

Als u wilt controleren of de optie voor geneste triggers is ingeschakeld, gebruikt u de volgende opdracht:

**sp\_configure 'nested triggers'**

Als u de optie voor geneste triggers in SQL Server wilt inschakelen, voert u de volgende opdracht uit vanuit een batchbestand op de computer waarop SQL Server wordt uitgevoerd:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Kwestie 7: opdrachtregelparameters voor de installatie van WSUS

U kunt WSUS zonder toezicht installeren. Zie 'Appendix A: Unattended Installation' in [Deploying Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777).

Bekende problemen
-----------------

#### Kwestie 1: wizard IIS Lockdown

Als u IIS uitvoert op een computer met Windows 2000 Server, installeert u de laatste versie van de wizard IIS Lockdown (die URLScan bevat) vanaf de pagina voor IIS Lockdown op Microsoft TechNet. Microsoft raadt u ten zeerste aan deze functie te installeren om uw IIS-servers te beveiligen. De wizard IIS Lockdown schakelt niet-vereiste functies van IIS uit, zodat de beveiligingsrisico's afnemen.

| ![](images/Cc720505.note(WS.10).gif)Opmerking                                                                                                                                                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Deze onderdelen worden niet geïnstalleerd tijdens de installatie van WSUS. U moet deze handmatig installeren. U hoeft IIS Lockdown niet te installeren op computers waarop Windows Server 2003 wordt geïnstalleerd, omdat deze functionaliteit is ingebouwd. |

#### Kwestie 2: de WSUS-configuratie kan niet rechtstreeks in de database worden gewijzigd

De configuratiegegevens van Windows Server Update Services worden in een database opgeslagen (MSDE of SQL Server). U kunt de configuratiegegevens echter niet wijzigen door rechtstreeks in de database wijzigingen aan te brengen. Beheerders moeten niet proberen om de configuratie van WSUS op deze manier te wijzigen. De ondersteunde manier om de configuratie van WSUS te wijzigen is door de WSUS-console te gebruiken of de API's van WSUS aan te roepen.

#### Kwestie 3: u moet Active Scripting inschakelen om toegang tot de WSUS-beheersite te krijgen

Op het beheerderswerkstation moet u Internet Explorer zodanig configureren dat Active Scripting is toegestaan voordat u met Internet Explorer toegang tot de beheersite voor WSUS kunt verkrijgen.

#### Kwestie 4: IIS wordt opnieuw gestart tijdens de installatie van WSUS

IIS wordt zonder waarschuwing opnieuw gestart tijdens de installatie van Windows Server Update Services. Dit kan gevolgen voor bestaande websites in uw organisatie hebben.

#### Kwestie 5: de toegang tot virtuele mappen voor WSUS- of SMS-beheerpunten wijzigen

De virtuele map voor inhoud voor Windows Server Update Services is standaard ingesteld op anonieme toegang. Als u deze instelling wijzigt zodat verificatie is vereist, ontvangen clients verificatiefouten en kunnen deze geen updates downloaden. Dit is een bekend probleem waarbij Winhttp.dll de verkeerde verificatiecontext gebruikt wanneer impliciete verificatie vereist is, zodat de verificatiecontrole mislukt. Als u dit probleem wilt voorkomen, moet u zorgen dat beheerpunten van WSUS-server en SMS worden ingesteld op anonieme toegang tot virtuele mappen van IIS.

#### Kwestie 6: bij het installeren van WSUS onder Windows Small Business Server 2003 moeten de vroots-toegangsinstellingen van WSUS voor de standaardwebsite worden gewijzigd zodat WSUS-clients automatisch kunnen worden bijgewerkt vanaf de server

De WSUS-server installeert twee vroots, SelfUpdate en ClientWebService, en enige bestanden onder de hoofdmap van de standaardwebsite (op poort 80). Hierdoor kunnen clients automatisch worden bijgewerkt via de standaardwebsite. De standaardwebsite is onder Windows Small Business Server 2003 standaard zodanig geconfigureerd dat de toegang wordt geweigerd aan elk IP-adres of elke localhost die niet van de server is. Dit betekent dat de vroots SelfUpdate en ClientWebService geen toegang kunnen verkrijgen en dat de clients niet kunnen worden bijgewerkt. Voer de volgende stappen uit op de vroots SelfUpdate en ClientWebService van de standaardwebsite als u de clients toegang wilt verlenen, zodat deze automatisch kunnen worden bijgewerkt.

1.  Klik op **Eigenschappen** voor de vroot, klik op **Mapbeveiliging**, klik op **Beperkingen voor IP-adressen en domeinnamen** en klik op **Bewerken**.
2.  Selecteer **Toegang verleend** en klik op **OK**. Sluit alle eigenschappenpagina's.

#### Kwestie 7: integratieproblemen bij het installeren van WSUS onder Small Business Server

-   Als Windows Small Business Server 2003 een ISA-proxyserver gebruikt om toegang te krijgen tot internet, moeten de volgende instellingen handmatig bij **Instellingen** worden ingevoerd: de instellingen, naam en poort van de proxyserver.
-   Als ISA Windows-verificatie gebruikt, moeten de referenties voor de proxyserver in de volgende vorm worden ingevoerd: 'DOMEIN\\gebruiker' (de gebruiker die behoort tot de groep Internetgebruikers).

#### Kwestie 8: wanneer u een computer tussen computergroepen verplaatst, kan het één uur duren voordat de computer in de nieuwe groep wordt weergegeven in de beheerconsole

Wanneer een computer voor de eerste keer aan een doelgroep wordt toegewezen, worden de groepsgegevens voor de computer gewijzigd. Deze gegevens worden periodiek of om het uur vernieuwd. Wanneer u een computer tussen computergroepen verplaatst, kan het daarom één uur duren voordat deze gegevens worden vernieuwd op de client en gewijzigd worden weergegeven in de beheerconsole van WSUS.

#### Kwestie 9: Als u WSUS installeert op een lidserver en u de lidserver vervolgens wilt promoveren tot een domeincontroller, moet u eerst WSUS verwijderen

Als u WSUS installeert op een lidserver en u de lidserver vervolgens wilt promoveren tot een domeincontroller, moet u de volgende stappen uitvoeren:

1.  Verwijder WSUS.
2.  Promoveer de server tot een domeincontroller.
3.  Installeer WSUS opnieuw.

#### Kwestie 10: als u een WSUS-server van een domeincontroller wilt degraderen tot een lidserver, moet u eerst WSUS verwijderen

Als u een WSUS-server uitvoert op een domeincontroller en u de domeincontroller wilt degraderen tot een lidserver, moet u de volgende stappen uitvoeren:

1.  Installeer WSUS en behoud de database.
2.  Maak een gebruikersaccount met de naam ASPNET.
3.  Typ **aspnet\_regiis -i** achter de opdrachtprompt.
4.  Installeer WSUS opnieuw en gebruik de behouden database.

#### Kwestie 11: als .NET Framework 1.0 of 2.0 wordt geïnstalleerd nadat WSUS wordt geïnstalleerd, wordt de beheerconsole van WSUS niet weergegeven

Dit komt doordat .NET Framework 1.0 is geregistreerd bij IIS terwijl de WSUS-server .NET Framework 1.1 nodig heeft. U kunt dit probleem oplossen door aspnet\_regiis.exe te openen en de volgende opdrachten uit te voeren waarbij *website-id* de waarde in de volgende registersleutel is:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*website id*&gt;\\ROOT\\Content

#### Kwestie 12: beperkingen voor externe SQL

WSUS biedt beperkte ondersteuning voor het uitvoeren van databasesoftware op een computer die gescheiden is van de computer met de rest van de WSUS 3.0-toepassing.

-   U kunt Windows 2000 Server niet als front-endcomputer in een extern SQL-paar uitvoeren.
-   U kunt geen server gebruiken die als een domeincontroller is geconfigureerd voor de front-end- of back-endcomputer van een SQL-paar.
-   U kunt WMSDE of MSDE niet gebruiken voor databasesoftware op de back-endcomputer.
-   De installatie van een externe SQL-server (om te gebruiken als WSUS-database) mislukt als Terminal Services op de externe server wordt geïnstalleerd en wordt uitgevoerd in de toepassingsmodus. Bij het installeren van SQL Server op een Terminal Services-server, moet u de volgende stappen uitvoeren:
    1.  Open een opdrachtvenster en typ het volgende voordat u de installatie uitvoert: **change user /install**
    2.  Voer de installatie van SQL Server uit.
    3.  Typ na de installatie het volgende achter de opdrachtprompt: **change user /execute**
-   U moet lid van de lokale beveiligingsgroep Administrators zijn op de front-end- en back-endcomputer als u de WSUS-database voor de externe SQL-server wilt instellen.
-   Zie 'Appendix C: Remote SQL' in [Deploying Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777). voor meer informatie over problemen met externe SQL.

#### Kwestie 13: een downstream-replica-server kan minder goedkeuringen hebben dan de bovenliggende upstream-server

Een downstream-replica-server kan minder goedkeuringen hebben dan de bovenliggende upstream-server. Dit komt doordat installatiegoedkeuringen pas naar een downstream-server worden overgebracht wanneer het downloaden van de inhoud is voltooid op de upstream-server.

#### Kwestie 14: Als het synchronisatieproces mislukt, moet een nieuwe synchronisatiepoging worden uitgevoerd

Als het synchronisatieproces mislukt, kan er een foutbericht verschijnen. Als dat gebeurt, moet u eerst proberen te synchroniseren.

#### Kwestie 15: wanneer u toegang tot de beheerconsole van WSUS probeert te verkrijgen, kan het foutbericht System.IO.FileNotFoundException worden weergegeven

Als het volgende foutbericht wordt weergegeven, moet u mogelijk de machtigingen voor de account Netwerkservice of ASP.NET aanpassen:

System.IO.FileNotFoundException: Kan de bestands- of assembly-naam *xxxxxx*.dll of een afhankelijkheid ervan, niet vinden.

Daarbij is *xxxx* een willekeurige naam.

Als u dit probleem wilt oplossen in Windows Server 20003 besturingssystemen, verleent u de account Netwerkservice lees-/schrijftoegang tot %systemroot%\\Temp. In Windows 2000 Server verleent u de account ASP.NET lees-/schrijftoegang tot %systemroot%\\Temp.

#### Kwestie 16: beveiligingspatch voor SQL MS03-031 (KB815495)

Deze update kan op de WSUS-server als geïnstalleerd worden weergegeven terwijl de installatie is mislukt op de client. Hierdoor kan het pakket opnieuw worden aangeboden aan de client. U kunt dit probleem omzeilen door de goedkeuring van de update ongedaan te maken op de server.

#### Kwestie 17: IIS-instellingen gaan verloren tijdens het uitvoeren van een upgrade van RTM.

Als u WSUS RTM installeert op een server waarop een vorige versie van WSUS is geïnstalleerd (bijvoorbeeld RC), wordt de vorige versie verwijderd door WSUS RTM en wordt vervolgens de nieuwe versie geïnstalleerd. Dit betekent dat vroots en bestanden voor WSUS in IIS worden verwijderd.

Als u WSUS op de standaardwebsite hebt geïnstalleerd, gaan instellingen voor WSUS verloren die u hebt aangebracht in de vroots van WSUS. Als u bijvoorbeeld de WSUS-vroots voor SSL hebt geconfigureerd om WSUS te beveiligen, moet u deze opnieuw configureren nadat u de RTM-versie van WSUS hebt geïnstalleerd. Opmerking: u ontvangt op de WSUS-console de melding dat SSL niet is ingeschakeld.

Als u WSUS op een andere website dan de standaardwebsite hebt geïnstalleerd, gaan alle aanvullende instellingen op het websiteniveau voor WSUS verloren.

#### Kwestie 18: Hostkopteksten gebruiken

Als u waarden voor hostkopteksten wilt toewijzen aan de standaardwebsite (WSUS-website) in IIS, moet u 'Alle niet-toegewezen' of een toegewezen IP-adres toevoegen aan de lijst met IP-adressen zonder waarde voor hostkoptekst voor de standaardwebsite. Deze waarde moet ook worden toegevoegd aan de website die niet standaard is

**Waarschuwing**: Hierdoor kan de werking van Windows® SharePoint® Services en Exchange worden verstoord.

#### Kwestie 19: de URL van de WSUS-console moet worden toegevoegd aan de lijst met de webinhoudzones Vertrouwde websites en Lokaal intranet op computers waarop Internet Explorer-beveiliging is ingeschakeld

Als u Internet Explorer-beveiliging (ook bekend als het onderdeel Verbeterde beveiliging voor Internet Explorer van Microsoft Windows Server 2003) hebt ingeschakeld op een computer en u de WSUS-console niet toevoegt aan de webinhoudzones Vertrouwde websites en Lokaal intranet, wordt u steeds gevraagd om gebruikersreferenties op te geven wanneer u een pagina opent in de WSUS-console.

De WSUS-console toevoegen aan de webinhoudzones **Lokaal intranet** en **Vertrouwde websites**:

1.  Open **Internet-opties** (klik bijvoorbeeld op **Start**, wijs **Configuratiescherm** aan en klik op **Internet-opties**).
2.  Klik op het tabblad **Beveiliging** op **Lokaal intranet**, klik op **Sites**, klik op **Geavanceerd**, voeg de URL toe (http://*WSUSServernaam*/WSUSAdmin) en klik op **OK**.
3.  Klik op **Vertrouwde websites**, klik op **Sites**, voeg de URL van de WSUS-console toe, klik op **OK** en klik opnieuw op **OK** om het venster **Internet-opties** te sluiten.

#### Kwestie 20: het uitvoeren van een upgrade van de voorlopige versie van WSUS mislukt

Het uitvoeren van een upgrade van de voorlopige versie van WSUS kan mislukken als gevolg van een probleem met de structuur voor automatische updates. Dit kan gebeuren als meerdere clients automatisch worden bijgewerkt op hetzelfde moment dat u probeert de upgrade uit te voeren.

Oplossing:

1.  verbreek de verbinding tussen de WSUS-server en het netwerk, zodat clients geen verbinding kunnen maken.
2.  Typ het volgende achter een opdrachtprompt: **iisrestart /reset** en druk op ENTER.
3.  Voer de upgrade uit.

#### Kwestie 21: bepaalde goedkeuringen van SUS 1.0 kunnen niet worden gemigreerd naar WSUS.

Wanneer u SUS 1.0 naar WSUS migreert, kunnen bepaalde goedkeuringen op de SUS 1.0-server niet worden gemigreerd naar de WSUS-server. Dit komt doordat bepaalde updates die beschikbaar waren voor SUS 1.0, niet meer beschikbaar zijn voor WSUS. Omdat WSUS ondersteuning voor meer updates biedt dan SUS, kunnen er belangrijke updates op uw WSUS-server zijn die niet zijn goedgekeurd nadat het migratieproces is voltooid.

Microsoft raadt u aan om de verzameling niet-goedgekeurde updates op uw WSUS-server te controleren na de migratie vanaf SUS 1.0.

Zie [Step-by-Step Guide to Migrating from Software Update Services to Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=48042) op http://go.microsoft.com/fwlink/?LinkId=48042 voor meer informatie over de migratie van SUS 1.0 naar WSUS.

#### Kwestie 22: wijzig deze registervermelding voorafgaand aan de upgrade naar WSUS 2.0 Service Pack 1 als u WMSDE hebt gemigreerd naar SQL Server

Als u een upgrade van WSUS 2.0 wilt uitvoeren naar Service Pack 1 en u uw WMSDE-installatie hebt gemigreerd naar SQL Server (extern of lokaal), wijzigt u de volgende registervermelding:

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled

De waarde moet worden gewijzigd van 1 in 0.

#### Kwestie 23: een externe SQL-installatie migreren naar WSUS 2.0 Service Pack 1

Voer de volgende stappen uit bij het migreren van WSUS 2.0 Service Pack 1 met een externe SQL-configuratie:

1) Voer het installatiepakket zonder schakelopties op de front-endcomputer uit en kies voor een upgrade.

2) Voer het installatiepakket zonder schakelopties op de back-endcomputer uit en kies voor een upgrade.

#### Copyright

De informatie in dit document weerspiegelt de huidige zienswijze van Microsoft Corporation over de onderwerpen die vanaf de publicatiedatum zijn besproken. Aangezien Microsoft moet reageren op een veranderende marktsituatie, vormt dit document geen garantie van de zijde van Microsoft en kan Microsoft de juistheid van deze informatie die na de publicatiedatum wordt gepresenteerd, niet garanderen.

Dit document is alleen bedoeld ter informatie. MICROSOFT BIEDT GEEN GARANTIES MET BETREKKING TOT DE INFORMATIE IN DIT DOCUMENT, ONGEACHT OF DEZE GARANTIES EXPLICIET, IMPLICIET OF WETTELIJK ZIJN.

Het is de verantwoordelijkheid van de gebruiker zich te houden aan alle relevante copyrightwetgeving. Met inachtneming van de geldende auteursrechten, mag niets uit dit document worden gereproduceerd, opgeslagen in of toegevoegd aan gegevensbestanden, of openbaar gemaakt in enige vorm of op enige wijze, hetzij elektronisch, mechanisch, door opnamen of anderszins, of voor andere doeleinden worden gebruikt, zonder schriftelijke toestemming van Microsoft Corporation.

Microsoft heeft mogelijk patenten, patentaanvragen, merken, auteursrechten of andere intellectuele eigendomsrechten die van toepassing zijn op de inhoud in dit document. Tenzij uitdrukkelijk anders vermeld in de schriftelijke gebruiksrechtovereenkomst van Microsoft, geeft dit document u geen recht op deze patenten, merken, auteursrechten of andere intellectuele eigendommen.

Tenzij anders vermeld, zijn alle in dit document vermelde bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen fictief. Eventuele overeenkomsten met bestaande bedrijven, organisaties, producten, domeinnamen, e-mailadressen, logo's, personen, plaatsen en gebeurtenissen berusten geheel op toeval.

© 2005 Microsoft Corporation. Alle rechten voorbehouden.

Microsoft, SQL Server, Windows en Windows Server zijn merken of gedeponeerde merken van Microsoft Corporation.

De namen van bestaande bedrijven en producten die in dit document worden vermeld, kunnen merken zijn van de desbetreffende eigenaren.
