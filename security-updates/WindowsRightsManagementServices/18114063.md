---
TOCTitle: Problemen met het beheer van RMS
Title: Problemen met het beheer van RMS
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18114063
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747605(v=WS.10)'
---

Problemen met het beheer van RMS
================================

Nadat RMS op uw server is ingericht, kunnen er zich tijdens het dagelijkse beheer van RMS problemen voordoen. U kunt met de informatie in de volgende gedeelten een aantal algemene problemen oplossen.

Het bericht 'De SQL-server bestaat niet of de toegang tot de server is geweigerd' verschijnt wanneer u de RMS-beheerwebsite probeert te openen.
-----------------------------------------------------------------------------------------------------------------------------------------------

Als u RMS met behulp van een nieuwe installatie van SQL Server 2005 als de databaseserver hebt geïnstalleerd, start de SQL Server-service waarschijnlijk niet. In SQL Server 2005 is de service MSSQLSERVER niet ingesteld om automatisch te starten wanneer de server wordt gestart. Als u SQL Server na het installeren van RMS opnieuw hebt gestart en deze service niet op automatisch opnieuw starten hebt ingesteld, werkt RMS niet en kan alleen de RMS-webpagina Algemeen beheer worden geopend.

Nadat u de service MSSQLSERVER hebt gestart, moet u IIS opnieuw starten op de RMS-server om de functionaliteit van RMS te herstellen.

Kan de off line inschrijving niet voltooien
-------------------------------------------

Als het bestand voor de inschrijvingsaanvraag niet volledig is of is gewijzigd voordat het naar de EnrollService-website is gestuurd, kunt u de off line inschrijving niet voltooien. Het aanvraagbestand voor de inschrijving kan zijn beschadigd door een schadelijk programma of door een fout van een gebruiker of het systeem.

Afhankelijk van de ontbrekende informatie kan de EnrollService-website het bestand accepteren en een serverlicentieverleningscertificaat terugsturen, maar de website zou het bestand ook kunnen weigeren en een foutmelding kunnen weergeven.

Als er een serverlicentieverleningscertificaat wordt teruggestuurd, geeft dit certificaat aan wat er in het aanvraagbestand voor de inschrijving ontbreekt of waar dat bestand is beschadigd en geeft RMS een foutmelding wanneer u probeert het certificaat te importeren.

Als u de inschrijving niet kunt voltooien, controleer dan of de computer met de internetverbinding niet door een virus is besmet, exporteer vervolgens het aanvraagbestand voor de inschrijving opnieuw vanaf de RMS-server en breng het op een andere manier over naar de computer met de internetverbinding. Wanneer er zich dan weer een fout voordoet, neem dan contact op met de productondersteuning van Microsoft.

Er worden geen logboekbestanden gemaakt
---------------------------------------

De logboekregistratieservice van RMS is afhankelijk van de Message Queuing-service (ook bekend als MSMQ) en de toegang tot de logboekdatabase. Als er geen logboekbestanden worden gemaakt, kan het zijn dat de onderdelen niet goed zijn geconfigureerd of dat de communicatie tussen de onderdelen is verbroken.

Controleer of de RMS-server en de databaseserver op het netwerk zijn aangesloten. Als dat zo is, controleert u als volgt de vereisten voor de logboekregistratieservice van RMS en zorgt u ervoor dat alle software-afhankelijkheden op de juiste manier zijn geconfigureerd.

Controleer eerst de configuratie van Message Queuing. Message Queuing moet zijn geïnstalleerd en Active Directory-integratie moet zijn ingeschakeld.

**Controleren of Message Queuing is geïnstalleerd en goed is geconfigureerd**
1.  Klik in het **Configuratiescherm** op **Software** en vervolgens op **Windows-onderdelen toevoegen/verwijderen** om de **wizard Windows-onderdelen** te openen.

2.  Schakel in de **wizard Windows-onderdelen** het selectievakje **Toepassingsserver** in en klik op **Details**.

3.  Schakel het selectievakje **Message Queuing** in en klik op **Details**.

4.  Als het selectievakje **Active Directory-integratie** is ingeschakeld, gaat u naar de volgende test en controleert u of Message Queuing wordt uitgevoerd. Voer stap 5 tot en met 9 uit als dit selectievakje niet is ingeschakeld.

5.  Klik op **Start**, wijs **Alle programma's** en **Windows RMS** aan en klik op **Windows RMS-beheer** om de pagina Algemeen beheer te openen.

6.  Klik op **RMS van deze website verwijderen** naast de website waarop RMS is ingericht en klik op **OK**.

7.  Ga naar het onderdeel **Software** in het **Configuratiescherm** en klik achtereenvolgens op **Windows-onderdelen toevoegen/verwijderen**, **Toepassingsserver** en **Message Queuing**.

8.  Als u **Active Directory-integratie** wilt inschakelen, klikt u op **Details**, schakelt u het selectievakje **Active Directory-integratie** in en klikt u op **OK**.

9.  Open de pagina **Algemeen beheer**. Klik naast de naam van de website waarop u RMS wilt inrichten, op **RMS op deze website inrichten**.

Controleer vervolgens of Message Queuing op de server wordt uitgevoerd.

**Controleren of Message Queuing op de server wordt uitgevoerd**
1.  Klik in het **Configuratiescherm** op **Systeembeheer** en vervolgens op **Services**.

2.  Zoek in de lijst met services de service **Message Queuing** op.

3.  In de kolom **Status** moet voor de service **Gestart** staan. Als dat niet zo is, klikt u met de rechtermuisknop op de service en klikt u op **Starten**.

Daarna controleert u of de logboekregistratieservice gebeurtenissen naar de logboekdatabase mag wegschrijven. De logboekregistratieservice van RMS wordt uitgevoerd via de RMS-serviceaccount. Controleer of de RMS-serviceaccount kan worden aangemeld bij de databaseserver en dat de vereiste machtigingen zijn toegewezen, zodat er databases kunnen worden gemaakt en gegevens naar de bestanden kunnen worden geschreven.

Zodra er aan al de vereisten is voldaan, stopt u de logboekregistratieservice van RMS en start u deze opnieuw met behulp van de module Services. Nadat de logboekregistratieservice van RMS opnieuw is gestart, moeten er logboekbestanden op de databaseserver worden gemaakt. Als u SQL Server als de databaseserver gebruikt, laat de volgende procedure zien hoe u kunt controleren of er logboekbestanden worden gemaakt.

**Controleren of er logboekbestanden op SQL Server worden gemaakt**
1.  Ga naar de logboekdatabase in SQL Server Enterprise Manager, vouw **Databases** uit en vouw vervolgens de database met de logboekdatabase van RMS uit.

2.  Klik op de logboekdatabase, klik op **Tabellen**, klik met de rechtermuisknop op **DRMS\_log\_master** en klik vervolgens op **Open table – return all rows** (Tabel openen – alle rijen ophalen). Als er logboekbestanden worden gemaakt, worden er een of meer logboekbestanden weergegeven.

De configuratiedatabase herstellen
----------------------------------

RMS kan niet worden uitgevoerd zonder een werkende configuratiedatabase. Als u problemen ondervindt met de configuratiedatabase, zoals een beschadigde database of een kapotte vaste schijf op de databaseserver, kunt u een back-up van de configuratiedatabase terugzetten om de RMS-functionaliteit te herstellen. Voor het herstellen van de RMS-configuratiedatabase vanuit een back-up hebt u de volgende gegevens nodig:

-   De naam van de meest recente back-up van de database.
-   De naam van de computer waarop de back-up van de database wordt hersteld.
-   De accountnaam en het wachtwoord die zijn gebruikt om RMS in te richten.
-   Het wachtwoord dat aanvankelijk is opgegeven voor de beveiliging van de software met een persoonlijke sleutel (als dit van toepassing is).

Voor een herstelbewerking met de back-updatabase is geen nieuw serverlicentieverleningscertificaat of een nieuwe persoonlijke sleutel vereist, aangezien alle instellingen in RMS behouden blijven (deze worden verkregen uit de back-up van de configuratiedatabase).

U kunt als volgt een back-updatabase herstellen:

**Een back-updatabase herstellen**
1.  Klik op **Start**, wijs **Alle programma's** en **Windows RMS** aan en klik op **Windows RMS-beheer** om de pagina **Algemeen beheer** te openen.

2.  Klik op **RMS van deze website verwijderen** naast de website waarop RMS is ingericht en klik op **OK**.

3.  Herstel de back-updatabasebestanden voor de configuratiedatabase. Als u tijdens de back-upprocedure een back-up hebt gemaakt van de logboekdatabase en u wilt continuïteit van gegevens behouden, moet u de logboekdatabase ook herstellen.

    -   Als dit systeem wordt hersteld na een systeemfout, moet u eerst het register herstellen met de back-up van de systeemstatus voordat u de bestanden van de back-updatabase gaat herstellen.

4.  Als de database die wordt hersteld, bedoeld is voor één basiscertificeringsserver, moet u de volgende registersleutel aanpassen voordat u de service opnieuw inricht:

    -   Op computers met de 32-bits versie van Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   Op computers met de 64-bits versie van Windows Server 2003
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Voeg alleen de volgende vermelding als een tekenreekswaarde toe zonder een waarde op te geven:

    `GicURL`

    Zodoende wordt de opsporing van de basiscertificeringsserver door Active Directory genegeerd en krijgt u toegang tot de pagina's voor het inrichten van de basiscertificeringsserver.

5.  Als u een hardwarebeveiligingsmodule gebruikt om de persoonlijke sleutel van RMS te beveiligen, moet u de back-upbeveiligingsomgeving herstellen, zodat de sleutels kunnen worden opgehaald.

6.  Voer een van de volgende stappen uit:

    -   Als u de database voor één server wilt herstellen in plaats van voor een cluster, klikt u op RMS op deze website inrichten naast de website waarop u RMS wilt inrichten.
        - of -
    -   Als u de database voor een cluster wilt herstellen, klikt u op Deze server aan een cluster toevoegen naast de website waarop u RMS wilt inrichten.

7.  Geef de RMS-serviceaccount op die is gebruikt voor het inrichten van de server.

8.  Geef de back-upconfiguratiedatabase op die u wilt gebruiken (inclusief de databasenaam en de naam van de computer waarop de database zich bevindt).

9.  Geef hetzelfde wachtwoord op dat u hebt gebruikt bij het inrichten van de server.

10. Klik op **Verzenden**.

Het inrichtingsproces wordt gestart en RMS wordt opnieuw op de server ingericht.

Zie 'Systeemherstel plannen' en 'Een back-up van het RMS-systeem maken en het RMS-systeem herstellen' in 'Een RMS-implementatie plannen' in deze documentatie voor meer informatie hierover.

Wachtwoord van de RMS-serviceaccount is verlopen
------------------------------------------------

Als RMS niet meer functioneert, is het wachtwoord van de RMS-serviceaccount mogelijk verlopen. Zoek in IIS Manager. Als de toepassingsgroepen van RMS worden gestopt en u deze niet meer opnieuw kunt starten, is het wachtwoord van de RMS-serviceaccount wellicht verlopen.

Wanneer het wachtwoord van de RMS-serviceaccount verloopt, moet u het wachtwoord wijzigen op elke RMS-server die de account met het verlopen wachtwoord gebruikt. Start vervolgens IIS opnieuw. Zie 'Het wachtwoord voor de RMS-serviceaccount wijzigen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.

Een vorige RMS-installatie herstellen
-------------------------------------

Als er een fout optreedt in de hardware of software van de server, kunt u een RMS-server herstellen door een nieuw exemplaar van een server in te richten met de vorige configuratiedatabase.

| ![](/security-updates/images/Cc747605.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Deze procedure is alleen van toepassing als er een fout optreedt op de server waarop RMS wordt uitgevoerd. Zie 'De configuratiedatabase herstellen' eerder in dit onderwerp als er een fout optreedt op de server waarop de configuratiedatabase wordt uitgevoerd. Is de RMS-server ook de databaseserver, dan zult u de gehele server vanuit een back-up moeten herstellen. |

Als u naar dezelfde configuratiedatabase wilt verwijzen die is gebruikt voor de oorspronkelijke installatie, voert u de volgende procedure uit:

**Een vorige RMS-installatie herstellen**
1.  Meld u aan met een account met beheerdersbevoegdheden bij de computer die u wilt configureren als RMS-server. Controleer of de computer voldoet aan de minimale systeemvereisten voor RMS. Zie 'Hardwarevereisten voor RMS' in de sectie 'Een RMS-implementatie plannen' van deze documentatie voor meer informatie over de systeemvereisten.

2.  Als u een hardwarebeveiligingsmodule gebruikt om de persoonlijke sleutels van RMS te beveiligen, moet u controleren of de hardwarebeveiligingsmodule is geconfigureerd met dezelfde instellingen en beveiligingsomgeving als de vorige RMS-installatie.

3.  Installeer RMS op de computer.

4.  Nadat u de installatie van RMS hebt voltooid, klikt u op **Start** en wijst u **Alle programma's** en **Windows RMS** aan. Klik vervolgens op **Windows RMS-beheer** om de pagina **Algemeen beheer** te openen.

5.  Klik naast de website waarop u RMS wilt inrichten, op **Deze server aan een cluster toevoegen**.

6.  Typ in het gedeelte **RMS-serviceaccount** de naam van de RMS-serviceaccount in de indeling domeinnaam\\gebruikersnaam en het wachtwoord van de RMS-serviceaccount waaronder RMS actief moet zijn voor de meeste routinebewerkingen. Dit moet een domeinaccount zijn.

7.  Geef in het gedeelte **Configuratiedatabase** de naam op van de databaseserver en de naam van de configuratiedatabase van de oorspronkelijke RMS-installatie die u wilt herstellen.

8.  Selecteer in het gedeelte **Persoonlijke-sleutelbeveiliging** het mechanisme dat door dit cluster moet worden gebruikt voor de beveiliging van de persoonlijke sleutel. Als u softwarebeveiliging voor persoonlijke sleutels hebt gebruikt, moet u het wachtwoord opgeven dat bij het inrichten van dit cluster is gebruikt voor het coderen van de persoonlijke sleutel.

9.  Klik op **Verzenden**.

Clients kunnen vanwege verlopen machtigingen geen door RMS beveiligde inhoud openen
-----------------------------------------------------------------------------------

Als de machtigingen van een gebruiker zijn verlopen, kan de gebruiker geen inhoud meer gebruiken die door RMS wordt beveiligd. Als de systeemklok op de RMS-server voorloopt op de systeemklok van de RMS-client, kan de gebruiker waarschijnlijk ook geen inhoud gebruiken die door RMS wordt beveiligd, zelfs als de machtigingen nog niet zijn verlopen. Omdat de systeemklokken op de twee computers niet gelijk lopen, kan het volgende foutbericht verschijnen wanneer vanaf de clientcomputer wordt geprobeerd de inhoud te openen:

**U hebt geen toestemming om dit bericht te openen omdat uw machtiging is verlopen. Wilt u het bericht met behulp van andere referenties openen?**

Zowel de clientlicentie als de inhoudslicentie zijn geldig, maar door het tijdsverschil denkt de client dat de inhoudslicentie niet geldig is en geeft deze een fout. Voor een gebruiker kan het lijken alsof er een probleem is met zijn of haar RMS-accountcertificaat of met de machtigingen die aan het document zijn toegekend. Als de tijd van de klok binnen de geldigheidsperiode van de uitgiftelicentie voor de inhoud valt, kan de gebruiker de inhoud openen.

Daarom moeten de klokken op de client en de servers in het RMS-systeem gelijk lopen.

De fout 'Toegang geweigerd' verschijnt wanneer RMS probeert gebeurtenissen naar het gebeurtenislogboek voor toepassingen weg te schrijven.
------------------------------------------------------------------------------------------------------------------------------------------

Standaard worden onderdelen zoals RMS die vanaf een ASP-pagina worden uitgevoerd, onder de account IUSR\_COMPUTERNAME gemaakt. Deze account behoort tot de groep Gasten. Omdat beveiligingsrechten nodig zijn om naar het gebeurtenislogboek voor toepassingen te kunnen schrijven, kunnen de gastaccounts geen gegevens in het gebeurtenislogboek opslaan.

U lost dit op door met de registereditor de registersleutel te wijzigen die hiervoor verantwoordelijk is.

| ![](/security-updates/images/Cc747605.Caution(WS.10).gif)Waarschuwing                                                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u het register onjuist bewerkt, kunt u het systeem ernstig beschadigen. Maak een back-up van alle belangrijke gegevens op de computer voordat u het register wijzigt. |

Stel de volgende registersleutel in op 0 in plaats van op 1 en start vervolgens de computer opnieuw op om deze wijziging door te voeren.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Naam: `RestrictGuestAccess`

Type: `REG_DWORD`

| ![](/security-updates/images/Cc747605.note(WS.10).gif)Opmerking                 |
|--------------------------------------------------------------------------------------------|
| Hierdoor kunnen alle gastaccounts naar het gebeurtenislogboek voor toepassingen schrijven. |

Zie het artikel over het inschakelen van de registratie vanaf ASP-pagina's in de [Knowledge Base van Microsoft](http://go.microsoft.com/fwlink/?linkid=44167) voor meer informatie over de oorzaak van deze fout.
