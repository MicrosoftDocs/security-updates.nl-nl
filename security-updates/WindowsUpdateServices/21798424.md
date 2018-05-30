---
TOCTitle: 'Stap 2: WSUS-server of de beheerconsole installeren'
Title: 'Stap 2: WSUS-server of de beheerconsole installeren'
ms:assetid: '6db6fcb0-c55d-43b9-9b07-4040c6267759'
ms:contentKeyID: 21798424
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Dd939859(v=WS.10)'
---

Stap 2: WSUS-server of de beheerconsole installeren
===================================================

Nadat u hebt gecontroleerd of de server aan de minimum installatievereisten voldoet en of de benodigde accountmachtigingen zijn toegekend, kunt u Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2) installeren. Start de installatie van WSUS 3.0 SP2. Maak daartoe gebruik van de toepasselijke procedure voor uw besturingssysteem en type installatie (via Serverbeheer of het bestand WUSSetup.exe).

Als u gebruikmaakt van Serverbeheer
-----------------------------------

**De installatie van WSUS 3.0 SP2 Server starten via Serverbeheer**
1.  Meld u aan op de server waarop u WSUS 3.0 SP2 wilt installeren. U moet daartoe gebruikmaken van een account die lid is van de lokale groep Administrators.

2.  Klik op **Start**, wijs **Systeembeheer** aan en klik vervolgens op **Serverbeheer**.

3.  Klik in de sectie Functieoverzicht die wordt weergegeven in het rechterdeelvenster van het Serverbeheer-venster op **Functies toevoegen**.

4.  Klik op **Volgende** als de pagina Voordat u begint wordt weergegeven.

5.  Selecteer **Windows Server Update Services** op de pagina Serverfuncties selecteren.

6.  Klik op **Volgende** op de pagina Windows Server Update Services.

7.  Klik op **Installeren** op de pagina Bevestiging van items die voor installatie zijn geselecteerd.

8.  Sla de volgende sectie over en zie de procedure Doorgaan met de installatie van WSUS 3.0 SP2 wanneer de installatiewizard van WSUS 3.0 SP2 wordt gestart.

Als u gebruikmaakt van het bestand WUSSetup.exe
-----------------------------------------------

**Start de installatie van WSUS 3.0 SP2 Server of de WSUS 3.0 SP2-beheerconcole door gebruik te maken van het bestand WUSSetup.exe.**
1.  Meld u aan op de server waarop u WSUS 3.0 SP2 wilt installeren. U moet daartoe gebruikmaken van een account die lid is van de lokale groep Administrators.

2.  Dubbelklik op het installatiebestand **WSUSSetup.exe**.

3.  Zie de procedure Doorgaan met de installatie van WSUS 3.0 SP2 wanneer de installatiewizard van WSUS 3.0 SP2 wordt gestart.

De installatiewizard van WSUS 3.0 SP2 Setup gebruiken
-----------------------------------------------------

De WSUS-installatiewizard wordt gestart vanuit Serverbeheer of via het bestand WUSSetup.exe.

**Doorgaan met de installatie van WSUS 3.0 SP2**
1.  Klik op de welkomstpagina van de installatiewizard van Windows Server Update Services 3.0 op **Volgende**.

2.  Selecteer op de pagina Installatiemodus selecteren de optie **Volledige serverinstallatie inclusief beheerconsole** als u de WSUS-server op deze computer wilt installeren of selecteer **Alleen beheerconsole** als u alleen de beheerconsole wilt installeren.

3.  Lees op de pagina Gebruiksrechtovereenkomst de voorwaarden van de gebruiksrechtovereenkomst, klik op **Ik ga akkoord met de voorwaarden in deze gebruiksrechtovereenkomst** en klik vervolgens op **Volgende**.

4.  U kunt op de pagina Selecteer de bron voor updates van de installatiewizard specificeren vanaf welke locatie clients updates kunnen downloaden. Het selectievakje **Updates lokaal opslaan** is standaard ingeschakeld en updates worden opgeslagen op de locatie op de WSUS-server die door u wordt opgegeven. Als u het selectievakje **Updates lokaal opslaan** uitschakelt, kunnen clientcomputers goedgekeurde updates ophalen door verbinding te maken met Microsoft Update. Maak een keuze en klik vervolgens op **Volgende**.

5.  Selecteer op de pagina Opties voor database de software die wordt gebruikt voor het beheren van de WSUS 3.0-database. De installatiewizard biedt standaard aan om de interne database van Windows te installeren.

    Als u geen gebruik wilt maken van de interne database van Windows, moet u een exemplaar van SQL Server voor WSUS opgeven dat kan worden gebruikt door **Een bestaande databaseserver op deze computer gebruiken** of **Een bestaande databaseserver gebruiken op een externe computer** te selecteren. Typ de exemplaarnaam in het toepasselijke vak. De naam van het exemplaar moet worden opgegeven als &lt;*servernaam*&gt;\\&lt;*exemplaarnaam*&gt;, waarbij *servernaam* staat voor de naam van de server en waarbij *exemplaarnaam* staat voor de naam van het SQL-exemplaar. Maak een keuze en klik vervolgens op **Volgende**.

6.  Als u ervoor gekozen hebt om een verbinding met een SQL-server te maken, wordt op de pagina **Verbinding met instantie van SQL-server maken** geprobeerd om een verbinding met het opgegeven exemplaar van SQL-server tot stand te brengen. Als de verbinding tot stand is gebracht, klikt u op **Volgende** om door te gaan.

7.  Selecteer op de pagina Website selecteren de website die door WSUS zal worden gebruikt. Selecteer **Bestaande standaardwebsite van IIS gebruiken (aanbevolen)** als u gebruik wilt maken van de standaardwebsite op poort 80. Als u reeds over een website op poort 80 beschikt, kunt u een alternatieve website op poort 8530 maken door **Website van Windows Server Update Services 3.0 SP2 maken** te selecteren. Klik op **Volgende**.

8.  Controleer op de pagina **Microsoft Windows Server Update Services kan nu worden geïnstalleerd** de opties die u hebt geselecteerd en klik op **Volgende**.

9.  Op de laatste pagina van de installatiewizard wordt weergeven of de installatie van WSUS is gelukt. Nadat u op **Voltooien** hebt geklikt, wordt de configuratiewizard gestart.

Volgende stap
-------------

[Stap 3: de netwerkverbindingen configureren](https://technet.microsoft.com/42a144c5-f08e-4a6e-b360-47ddea77bd24).

Aanvullende bronnen
-------------------

[Stapsgewijze handleiding voor Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
