---
TOCTitle: 'Stap 1: Controleren of computers voldoen aan de vereisten voor de installatie van WSUS'
Title: 'Stap 1: Controleren of computers voldoen aan de vereisten voor de installatie van WSUS'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18126814
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720547(v=WS.10)'
---

Stap 1: Controleren of computers voldoen aan de vereisten voor de installatie van WSUS
======================================================================================

Deze handleiding bevat instructies voor het installeren van WSUS (Microsoft Windows Server Update Services) onder Microsoft Windows Server 2003-besturingssystemen (behalve voor Web Edition en alle 64-bits versies). Hebt u een server waarop Microsoft Windows 2000 Server wordt uitgevoerd en hebt u meer informatie nodig, raadpleeg dan het Engelstalige document 'Deploying Microsoft Windows Server Update Services'.

Hier volgen de minimale vereisten voor een installatie waarbij de standaardopties worden gebruikt. Hardware- en softwarevereisten voor overige installaties vindt u in het Engelstalige document 'Deploying Microsoft Windows Server Update Services'.

Voor een server met maximaal 500 clients gelden de volgende aanbevelingen:

-   Een processor van 1 GHz (gigahertz)
-   1 GB (gigabyte) aan RAM

Softwarevereisten
-----------------

Als u WSUS wilt installeren met de standaardopties, moet het volgende op de computer zijn geïnstalleerd: Raadpleeg het Engelstalige document 'Deploying Microsoft Windows Server Update Services' voor meer informatie over de softwarevereisten voor WSUS. Als een van deze updates vereist dat de computer opnieuw wordt gestart wanneer de installatie is voltooid, dient u de server opnieuw te starten voordat u WSUS installeert.

-   Microsoft Internet Information Services (IIS) 6.0. Instructies voor het installeren van IIS vindt in het Engelstalige document 'Deploying Microsoft Windows Server Update Services' en in Help en ondersteuning van Windows Server 2003.
-   Microsoft .NET Framework 1.1 Servicepack 1 voor Windows Server 2003. Als u deze software wilt ophalen, gaat u naar het [Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=47358) op http://go.microsoft.com/fwlink/?LinkId=35326.
    U kunt ook naar http://www.windowsupdate.com gaan en zoeken naar 'essentiële update en servicepacks - microsoft net framework 1.1 service pack 1 voor windows server 2003 installatie'.
-   BITS (Background Intelligent Transfer Service) 2.0. BITS 2.0 voor Windows Server 2003 is momenteel niet beschikbaar in het Downloadcentrum. Ga naar de [Microsoft-website](http://go.microsoft.com/fwlink/?linkid=47357) voor Windows Server Update Services Open Evaluation op http://go.microsoft.com/fwlink/?LinkId=39496 als u deze software wilt downloaden.

| ![](/security-updates/images/Cc720547.note(WS.10).gif)Opmerking                                                                                                                                                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hoewel er databasesoftware is vereist om WSUS te installeren, wordt deze software hier niet vermeld, omdat bij de standaardinstallatie van WSUS onder Windows Server 2003 de databasesoftware Windows SQL Server™ 2000 Desktop Engine (WMSDE) is inbegrepen. |

Vereisten en aanbevelingen voor de vaste schijf
-----------------------------------------------

Als u WSUS wilt installeren, moet het bestandssysteem van de server aan de volgende vereisten voldoen:

-   Zowel de systeempartitie als de partitie waarop u WSUS installeert, moeten zijn geformatteerd met het NTFS-bestandssysteem.
-   Voor de systeempartitie is minimaal 1 GB vrije geheugenruimte vereist.
-   Voor het volume waar WSUS-gegevens zullen worden opgeslagen is minimaal 6 GB vrije geheugenruimte vereist. Aanbevolen wordt een vrije geheugenruimte van 30 GB.
-   Voor het volume waar het installatieprogramma van WSUS het programma Windows SQL Server 2000 Desktop Engine (WMSDE) installeert, is minimaal 2 GB vrije geheugenruimte vereist.

Vereisten voor de service Automatische updates
----------------------------------------------

De service Automatische updates is het onderdeel van WSUS voor clientcomputers. Automatische updates stelt geen speciale eisen aan de hardware, maar de computer dient wel verbinding te hebben met het netwerk. U kunt Automatische updates in combinatie met WSUS gebruiken op computers met een van de volgende besturingssystemen:

-   Microsoft Windows 2000 Professional met servicepack 3 (SP3) of servicepack 4 (SP4), Windows 2000 Server met SP3 of SP4 of Windows 2000 Advanced Server met SP3 of SP4.
-   Microsoft Windows XP Professional met of zonder servicepack 1 of servicepack 2.
-   Microsoft Windows Server 2003 Standard Edition, Windows Server 2003 Enterprise Edition, Windows Server 2003 Datacenter Edition of Windows Server 2003 Web Edition.
