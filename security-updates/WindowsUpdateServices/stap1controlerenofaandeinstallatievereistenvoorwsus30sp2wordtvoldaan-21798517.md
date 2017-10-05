---
TOCTitle: 'Stap 1: controleren of aan de installatievereisten voor WSUS 3.0 SP2 wordt voldaan.'
Title: 'Stap 1: controleren of aan de installatievereisten voor WSUS 3.0 SP2 wordt voldaan.'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21798517
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Dd939916(v=WS.10)'
---

Stap 1: controleren of aan de installatievereisten voor WSUS 3.0 SP2 wordt voldaan.
===================================================================================

Voordat u Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2) installeert of voordat u een upgrade naar Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2) uitvoert, moet u controleren of de server en de clientcomputers voldoen aan de systeemvereisten voor WSUS 3.0 SP2 en of u over de benodigde machtigingen beschikt om de installatie te kunnen voltooien.

Hardware- en softwarevereisten voor de server voor het installeren van WSUS 3.0 SP2
-----------------------------------------------------------------------------------

1.  Controleer of de server voldoet aan de WSUS 3.0 SP2-systeemvereisten voor hardware, het besturingssysteem en andere vereiste software. De systeemvereisten worden weergegeven in de releaseopmerkingen voor WSUS 3.0 SP2 op [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840). Als u voor het installeren van WSUS 3.0 SP2 Server gebruikmaakt van Serverbeheer, moet u controleren of er aan de softwarevereisten wordt voldaan door de stappen in de sectie De installatie van WSUS 3.0 SP2 voorbereiden te volgen.
2.  Als u functies of software-updates installeert waarvoor het is vereist dat de server opnieuw wordt opgestart zodra de installatie is voltooid, moet u de server opnieuw opstarten voordat u WSUS 3.0 SP2 installeert.

Clientsoftwarevereisten
-----------------------

Automatische updates is de client van WSUS 3.0. Automatische updates stelt geen speciale eisen aan de hardware, maar de computer moet wel verbinding hebben met het netwerk.

1.  Controleer of de computer waarop u Automatische updates installeert, voldoet aan de WSUS 3.0 SP2-systeemvereisten voor clientcomputers. De systeemvereisten worden weergegeven in de releaseopmerkingen voor WSUS 3.0 SP2 op [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840).
2.  Als u software-updates installeert waarvoor het is vereist dat de server opnieuw wordt opgestart, moet u de computer opnieuw opstarten voordat u WSUS 3.0 SP2 installeert.

Machtigingen
------------

De volgende machtigingen zijn vereist voor de gespecificeerde gebruikers en mappen:

1.  De account NT Authority\\Network Service moet beschikken over de machtiging Volledig beheer voor de volgende mappen, zodat de WSUS-beheermodule correct wordt weergegeven:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  Controleer of de account die u wilt gebruiken voor het installeren van WSUS 3.0 SP2 lid is van de lokale groep Administrators.

De installatie van WSUS 3.0 SP2 voorbereiden
--------------------------------------------

Als u Windows 7 of Windows Server 2008 SP2 uitvoert, kunt u WSUS 3.0 SP2 installeren via Serverbeheer. Als u gebruikmaakt van een ander ondersteund besturingssysteem of als u alleen de WSUS-beheerconsole installeert, gaat u naar de volgende sectie van deze handleiding, zodat u WSUS 3.0 SP2 kunt installeren met behulp van het bestand WUSSetup.exe.

**De installatie van WSUS 3.0 SP2 Server via Serverbeheer voorbereiden**
1.  Meld u aan op de server waarop u WSUS 3.0 SP2 wilt installeren. U moet hiertoe gebruikmaken van een account die lid is van de lokale groep Administrators.

2.  Klik op **Start**, wijs **Systeembeheer** aan en klik vervolgens op **Serverbeheer**.

3.  Klik in de sectie Functieoverzicht die wordt weergegeven in het rechterdeelvenster van het Serverbeheer-venster op **Functies toevoegen**.

4.  Klik op **Volgende** als de pagina Voordat u begint wordt weergegeven.

5.  Controleer op de pagina Serverfuncties selecteren of de selectievakjes **Toepassingsserver** en **Webserver (IIS)** zijn ingeschakeld. Als deze selectievakjes zijn ingeschakeld, moet u controleren of de vereiste functieservices zijn geselecteerd. Als deze selectievakjes niet zijn ingeschakeld, installeert u Toepassingsserver en Webserver (IIS) op de volgende wijze.

    1.  Schakel de selectievakjes **Toepassingsserver** en **Webserver (IIS)** in op de pagina Serverfuncties selecteren. Klik op **Volgende**.
    2.  Klik op de pagina Toepassingsserver op **Volgende** als u Services voor functie van toepassingsserver wilt installeren. Accepteer de standaardinstellingen op de pagina Services voor functie van toepassingsserver en klik vervolgens op **Volgende**.
    3.  Klik op de pagina Webserver (IIS) op **Volgende** als u Webserver IIS installeert. Selecteer op de pagina Services voor functie van webserver (IIS) naast de standaardinstellingen de opties **ASP.NET**, **Windows-verificatie**, **Dynamische inhoudcompressie** en **Compatibiliteit met IIS 6-beheer**. Klik op **Vereiste functieservices toevoegen** als de wizard Functies toevoegen wordt weergegeven. Klik op **Volgende**.
    4.  Klik op **Installeren** op de pagina Bevestiging van items die voor installatie zijn geselecteerd.
    5.  Controleer op de pagina Installatieresultaten of het bericht Installatie geslaagd wordt weergegeven voor de functieservices die u tijdens deze stap hebt geïnstalleerd en klik vervolgens op **Sluiten**.

Volgende stap
-------------

[Stap 2: WSUS-server of de beheerconsole installeren](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759).

Aanvullende bronnen
-------------------

[Stapsgewijze handleiding voor Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
