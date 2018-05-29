---
TOCTitle: 'Stap 2: WSUS 3.0 op de server installeren'
Title: 'Stap 2: WSUS 3.0 op de server installeren'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18126739
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720469(v=WS.10)'
---

Stap 2: WSUS 3.0 op de server installeren
=========================================

Nadat u hebt gecontroleerd of uw server aan de installatievereisten voldoet, bent u gereed om WSUS 3.0 te installeren. U moet zich aanmelden bij de server waarop u WSUS 3.0 wilt installeren met een account die lid is van de lokale groep Administrators. Alleen leden van de lokale groep Administrators kunnen WSUS 3.0 installeren.

Voor de volgende procedure worden de standaardinstallatieopties van WSUS gebruikt. Dit betekent dat Windows Internal Database als de databasesoftware voor WSUS 3.0 wordt geïnstalleerd, dat updates lokaal worden opgeslagen en dat de standaardwebsite van IIS op poort 80 wordt gebruikt.

**WSUS 3.0 installeren**
1.  Dubbelklik op het installatieprogrammabestand **WSUSSetup.exe**.

2.  Klik op de **Welkomstpagina** van de wizard op **Volgende**.

3.  Klik op de pagina **Installatiemodus selecteren** op **Volledige serverinstallatie inclusief beheerconsole** als u de server op deze computer wilt installeren, of klik op **Alleen beheerconsole** als u alleen de beheerconsole wilt installeren.

4.  Lees de gebruiksrechtovereenkomst op de pagina **Gebruiksrechtovereenkomst** aandachtig door, klik op **Ik ga akkoord met de voorwaarden van de gebruiksrechtovereenkomst** en klik op **Volgende**.

    ![](/security-updates/images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Op de pagina **Selecteer de bron voor updates** van de installatiewizard kunt u opgeven waar clients updates kunnen ophalen. Als u het selectievakje **Updates lokaal opslaan** inschakelt, worden de updates op de WSUS 3.0-server opgeslagen en kunt u in het bestandssysteem een locatie selecteren waar de updates moeten worden opgeslagen. Als u opgeeft dat de updates niet lokaal moeten worden opgeslagen, maken clientcomputers verbinding met Microsoft Updates om goedgekeurde updates op te halen. Zorg ervoor dat de standaardopties geselecteerd blijven en klik op **Volgende**.

    ![](/security-updates/images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  Op de pagina **Opties voor database** selecteert u de software die moet worden gebruikt om de WSUS 3.0-database te beheren. Als u WSUS installeert op een computer met Windows Server 2003, biedt het installatieprogramma van WSUS u standaard aan het programma Windows Internal Database te installeren.

7.  Als u Windows Internal Database niet wilt gebruiken, moet u een SQL Server-instantie opgeven die WSUS kan gebruiken. Klik daartoe op **Een bestaande databaseserver op deze computer gebruiken** en typ de naam van de instantie in het vak. De naam van de instantie moet worden opgegeven als &lt;*serverName*&gt;\\&lt;*instanceName*&gt;, waarbij *serverName* de naam van de server is en *instanceName* de naam van de SQL-instantie. Maak een keuze en klik vervolgens op **Volgende**.

8.  Op de pagina **Verbinding met instantie van SQL-server maken** probeert WSUS verbinding te maken met de opgegeven instantie van SQL Server. Als de verbinding tot stand is gebracht, klikt u op **Volgende** om door te gaan.

    ![](/security-updates/images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  Op de pagina **Website selecteren** kunt u opgeven welke website WSUS 3.0 moet gebruiken. Als u de standaardwebsite van IIS op poort 80 wilt gebruiken, selecteert u de eerste optie. Als al een website aan poort 80 is gekoppeld, kunt u een alternatieve site op poort 8530 maken door de tweede optie te selecteren. Zorg ervoor dat de standaardoptie geselecteerd blijft en klik op **Volgende**.

10. Bekijk op de pagina **Microsoft Windows Server Update Services kan nu worden geïnstalleerd** de opties die u hebt geselecteerd en klik op **Volgende**.

11. Op de laatste pagina van de installatiewizard wordt gemeld of de installatie van WSUS 3.0 is geslaagd. Als u op **Voltooien** klikt, wordt de configuratiewizard gestart.
