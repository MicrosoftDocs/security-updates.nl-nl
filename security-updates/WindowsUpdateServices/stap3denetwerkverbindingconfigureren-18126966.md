---
TOCTitle: 'Stap 3: De netwerkverbinding configureren'
Title: 'Stap 3: De netwerkverbinding configureren'
ms:assetid: 'cd77566d-7780-4ce4-aa56-41183c65c4a7'
ms:contentKeyID: 18126966
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708559(v=WS.10)'
---

Stap 3: De netwerkverbinding configureren
=========================================

Nadat u WSUS hebt geïnstalleerd, kunt u de WSUS-console gebruiken om WSUS te configureren en om vervolgens de eerste updates op te halen. WSUS is standaard geconfigureerd om updates op te halen bij Microsoft Update. Als er een proxyserver in het netwerk aanwezig is, gebruikt u de WSUS-console om WSUS te configureren voor het gebruik van de proxyserver. Als er een bedrijfs-firewall aanwezig is tussen WSUS en internet, moet u de firewall mogelijk configureren om ervoor te zorgen dat WSUS updates kan ophalen.

| ![](images/Cc708559.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hoewel u verbinding moet hebben met internet om updates te kunnen downloaden van Microsoft Update, biedt WSUS u de mogelijkheid updates te importeren in netwerken die niet verbonden zijn met internet. Raadpleeg het Engelstalige document 'Deploying Microsoft Windows Server Update Services' voor meer informatie. |

Stap 3 omvat de volgende procedures:

-   De firewall zodanig configureren dat WSUS updates kan ophalen
-   De WSUS console openen
-   De proxyserver-instellingen zodanig configureren dat WSUS updates kan ophalen

**De firewall configureren**
-   Als er een bedrijfs-firewall aanwezig is tussen WSUS en internet, moet u deze firewall mogelijk configureren om ervoor te zorgen dat WSUS updates kan ophalen. Voor het ophalen van updates bij Microsoft Update gebruikt de WSUS-server poort 80 voor het HTTP-protocol en poort 443 voor het HTTPS-protocol. Dit kunt u niet veranderen.

-   Als uw organisatie niet alle adressen toestemming wil geven deze poorten en protocollen te gebruiken, kunt u de toegang beperken tot de volgende domeinen, zodat WSUS en de service Automatische updates met Microsoft Update kunnen communiceren:

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

| ![](images/Cc708559.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| De hiervoor beschreven stappen voor het configureren van de firewall zijn bedoeld voor een bedrijfs-firewall die tussen WSUS en internet is geplaatst. Omdat alle WSUS-netwerkverkeer vanuit WSUS wordt gestart, hoeft u Windows Firewall niet te configureren op een WSUS-server. Hoewel voor de verbinding tussen Microsoft Update en WSUS de poorten 80 en 443 open moeten zijn, kunt u meerdere WSUS-servers zodanig configureren dat deze kunnen worden gesynchroniseerd via een aangepaste poort. Raadpleeg het Engelstalige document 'Deploying Microsoft Windows Server Update Services' voor meer informatie over het synchroniseren van WSUS-servers via een aangepaste poort. |

**De WSUS-console openen**
-   Klik op de WSUS-server op **Start**, wijs achtereenvolgens **Alle programma's** en **Systeembeheer** aan en klik vervolgens op **Microsoft Windows Server Update Services**.

| ![](images/Cc708559.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| U kunt de WSUS-console alleen gebruiken als u lid bent van de groep WSUS Administrators of van de lokale beveiligingsgroep Administrators op de server waarop WSUS is geïnstalleerd. Als u **http://&lt;***naam van WSUS-website***&gt;** niet toevoegt aan de lijst met websites in de lokale intranetzone in Internet Explorer onder Windows Server 2003, wordt mogelijk telkens wanneer u de WSUS-console opent, naar referenties gevraagd. Als u de poorttoewijzing in IIS wijzigt nadat u WSUS hebt geïnstalleerd, dient u de snelkoppeling in het menu **Start** handmatig aan te passen. U kunt de WSUS-console ook openen vanuit Internet Explorer op elke server of computer in het netwerk door de volgende URL te typen: **http://***WSUS-servernaam***/WSUSAdmin** |

**Een proxyserver opgeven**
1.  Klik op de werkbalk van de WSUS-console op **Opties** en klik vervolgens op **Opties voor synchronisatie**.

2.  Schakel in het vak **Proxyserver** het selectievakje **Proxyserver voor synchroniseren gebruiken** in en typ vervolgens de naam en het poortnummer (poort 80 is de standaard) van de proxyserver in de desbetreffende vakken.

3.  Als u via specifieke gebruikersreferenties verbinding wilt maken met de proxyserver, schakelt u het selectievakje **Gebruikersreferenties gebruiken voor het maken van een verbinding met de proxyserver** in en typt u vervolgens de gebruikersnaam, het domein en het wachtwoord van de gebruiker in de desbetreffende vakken. Als u eenvoudige verificatie wilt inschakelen voor de gebruiker die verbinding maakt met de proxyserver, schakelt u het selectievakje **Eenvoudige verificatie toestaan (wachtwoord wordt in leesbare tekst verzonden)** in.

4.  Klik onder **Taken** op **Instellingen opslaan** en klik vervolgens op **OK** om uw keus te bevestigen.
