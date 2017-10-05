---
TOCTitle: 'Stap 3: De netwerkverbinding voor WSUS 3.0 configureren'
Title: 'Stap 3: De netwerkverbinding voor WSUS 3.0 configureren'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18126991
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708602(v=WS.10)'
---

Stap 3: De netwerkverbinding voor WSUS 3.0 configureren
=======================================================

Na de installatie van WSUS 3.0 wordt de configuratiewizard automatisch gestart. U kunt de wizard ook later uitvoeren via de pagina **Opties** van de WSUS 3.0-console.

Als u de configuratieprocedure uitvoert, moet u de volgende vragen kunnen beantwoorden:

1. Is de firewall van de server geconfigureerd om clients toegang te geven tot de server?

2. Kan deze computer verbinding maken met de upstream-server (bijvoorbeeld Microsoft Update)?

3. Hebt u de naam van de proxyserver en de gebruikersreferenties voor de proxyserver indien nodig bij de hand?

WSUS is standaard geconfigureerd om updates op te halen bij Microsoft Update. Als er een proxyserver in het netwerk aanwezig is, kunt u WSUS te configureren voor het gebruik van de proxyserver. Als er een bedrijfs-firewall aanwezig is tussen WSUS en internet, moet u de firewall mogelijk configureren om ervoor te zorgen dat WSUS updates kan ophalen.

| ![](images/Cc708602.note(WS.10).gif)Opmerking                                                                                                                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hoewel u verbinding moet hebben met internet om updates te kunnen downloaden van Microsoft Update, biedt WSUS u de mogelijkheid updates te importeren in netwerken die niet verbonden zijn met internet. |

**Stap 3 omvat de volgende procedures**:

-   De firewall configureren
-   Opgeven hoe de server updates moet ophalen (via Microsoft Update of via een andere WSUS-server)
-   De proxyserver-instellingen zodanig configureren dat WSUS updates kan ophalen

**De firewall configureren**
-   Als er een bedrijfs-firewall aanwezig is tussen WSUS en internet, moet u deze firewall mogelijk configureren om ervoor te zorgen dat WSUS updates kan ophalen. Voor het ophalen van updates bij Microsoft Update gebruikt de WSUS-server poort 80 voor het HTTP-protocol en poort 443 voor het HTTPS-protocol. Dit kunt u niet veranderen.

-   Als uw organisatie niet alle adressen toestemming wil geven om poort 80 of poort 443 te gebruiken, kunt u de toegang beperken tot de volgende domeinen, zodat WSUS en de service Automatische updates met Microsoft Update kunnen communiceren:

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

| ![](images/Cc708602.note(WS.10).gif)Opmerking                                                                                                                                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Deze instructies voor het configureren van de firewall zijn bedoeld voor een bedrijfs-firewall die tussen WSUS en internet is geplaatst. Omdat alle WSUS-netwerkverkeer vanuit WSUS wordt gestart, hoeft u Windows Firewall niet te configureren op een WSUS-server. |

Hoewel voor de verbinding tussen Microsoft Update en WSUS de poorten 80 en 443 open moeten zijn, kunt u meerdere WSUS-servers zodanig configureren dat deze kunnen worden gesynchroniseerd via een aangepaste poort.

Bij de volgende twee procedures wordt aangenomen dat u de configuratiewizard gebruikt. In een latere fase van deze stap leert u hoe u de WSUS-beheermodule kunt starten en de server kunt configureren via de pagina **Opties**.

**Opgeven hoe de server updates moet ophalen**
1.  Nadat u zich hebt aangemeld bij het programma voor verbetering van de gebruikerservaring van Microsoft Update, klikt u op **Volgende** om de upstream-server in de configuratiewizard te kiezen.

2.  Als u ervoor kiest om te synchroniseren vanuit Microsoft Update, bent u klaar met deze pagina. Klik op **Volgende** of selecteer **Proxyserver opgeven** in het linkerdeelvenster.

3.  Als u ervoor kiest om te synchroniseren vanaf een andere WSUS-server, moet u de servernaam en de poort opgeven die worden gebruikt voor de communicatie tussen deze server en de upstream-server.

4.  Als u SSL wilt gebruiken, schakelt u het selectievakje **SSL gebruiken voor het synchroniseren van updategegevens** in. In dat geval gebruiken de servers poort 443 voor synchronisatie. (Zowel deze server als de upstream-server moeten SSL ondersteunen.)

5.  Als deze server een replica-server is, schakelt u het selectievakje **Deze server is een replica van de upstream-server** in.

6.  U bent nu klaar met de configuratie van de upstream-server. Klik op **Volgende** of selecteer **Proxyserver opgeven** in het linkerdeelvenster.

**Proxyserver-instellingen configureren**
1.  Schakel op de pagina **Proxyserver opgeven** van de configuratiewizard het selectievakje **Een proxyserver gebruiken tijdens het synchroniseren** in en typ de naam en het poortnummer (poort 80 is de standaard) van de proxyserver in de desbetreffende vakken.

2.  Als u via specifieke gebruikersreferenties verbinding wilt maken met de proxyserver, schakelt u het selectievakje **Gebruikersreferenties gebruiken voor het maken van een verbinding met de proxyserver** in en typt u vervolgens de gebruikersnaam, het domein en het wachtwoord van de gebruiker in de desbetreffende vakken. Als u eenvoudige verificatie wilt inschakelen voor de gebruiker die verbinding maakt met de proxyserver, schakelt u het selectievakje **Eenvoudige verificatie toestaan (wachtwoord wordt in leesbare tekst verzonden)** in.

3.  U bent nu klaar met de configuratie van de proxyserver. Klik op **Volgende** om naar de volgende pagina te gaan om de synchronisatieprocedure in te stellen.

Bij de volgende twee procedures wordt aangenomen dat u de WSUS-beheermodule gebruikt voor configuratie. Deze twee procedures laten zien hoe u de WSUS-beheermodule kunt starten en de server kunt configureren vanaf de pagina **Opties**.

**De WSUS-beheerconsole starten**
-   Klik op **Start**, wijs achtereenvolgens **Alle programma's** en **Systeembeheer** aan en klik op **Microsoft Windows Server Update Services 3.0** om de WSUS-beheerconsole te starten.

| ![](images/Cc708602.note(WS.10).gif)Opmerking                                                                                                                                                                                                                            |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u alle functies van de WSUS-console wilt gebruiken, moet u lid zijn van de groep WSUS Administrators of van de lokale beveiligingsgroep Administrators op de server waarop WSUS is geïnstalleerd. Leden van de beveiligingsgroep WSUS-reporters hebben alleen-lezen toegang tot de beheerconsole. |

**Een bron van updates en een proxyserver opgeven**
1.  Klik in de WSUS-console op **Opties** in het linkerdeelvenster onder de naam van deze server en klik op **Bron van update en proxyserver** in het middelste deelvenster.

2.  Er wordt een dialoogvenster weergegeven met de tabbladen **Bron van updates** en **Proxyserver**.

3.  Selecteer op het tabblad **Bron van updates** de locatie waar de server updates moet ophalen. Als u ervoor kiest om te synchroniseren vanuit Microsoft Update (standaardinstelling), bent u klaar met deze pagina.

4.  Als u ervoor kiest om te synchroniseren vanaf een andere WSUS-server, moet u de poort opgeven die wordt gebruikt voor communicatie tussen de servers (de standaardpoort is poort 80). Als u een andere poort kiest, moet u ervoor zorgen dat beide servers de poort kunnen gebruiken.

5.  U kunt ook opgeven of SSL moet worden gebruikt voor het synchroniseren vanaf de upstream-WSUS-server. In dat geval gebruiken de servers poort 443 om te synchroniseren vanaf de upstream-server.

6.  Als deze server een replica is van de tweede WSUS-server, schakelt u het selectievakje **Dit is een replica van de upstream-server** in. In dit geval moeten alle updates uitsluitend op de upstream-WSUS-server worden goedgekeurd.

7.  Schakel op het tabblad **Proxyserver** het selectievakje **Een proxyserver gebruiken tijdens het synchroniseren** in en typ de naam en het poortnummer (poort 80 is de standaard) van de proxyserver in de desbetreffende vakken.

8.  Als u via specifieke gebruikersreferenties verbinding wilt maken met de proxyserver, schakelt u het selectievakje **Gebruikersreferenties gebruiken voor het maken van een verbinding met de proxyserver** in en typt u vervolgens de gebruikersnaam, het domein en het wachtwoord van de gebruiker in de desbetreffende vakken. Als u eenvoudige verificatie wilt inschakelen voor de gebruiker die verbinding maakt met de proxyserver, schakelt u het selectievakje **Eenvoudige verificatie toestaan (wachtwoord wordt in leesbare tekst verzonden)** in.

9.  Klik op **OK** om deze instellingen op te slaan.
