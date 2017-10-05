---
TOCTitle: De databases beveiligen die door RMS worden gebruikt
Title: De databases beveiligen die door RMS worden gebruikt
ms:assetid: '65802f9a-81bc-4398-968a-00c9b1dca2fa'
ms:contentKeyID: 18113949
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720285(v=WS.10)'
---

De databases beveiligen die door RMS worden gebruikt
====================================================

In RMS worden drie databases gemaakt, waarvoor verschillende beveiligingsvereisten gelden:

-   **Database met directoryservices**. In deze database worden de resultaten van Active Directory-query's over groepslidmaatschappen opgeslagen. Omdat in deze database alleen Active Directory-gegevens worden opgeslagen, volstaan de beveiligingsinstellingen die tijdens de RMS-inrichting automatisch worden geconfigureerd.
-   **Logboekdatabase**. De gegevens in deze database zijn gevoeliger dan de gegevens in de database met Active Directory-gegevens omdat de openbaarmaking van deze gegevens van invloed kan zijn op de privacy van gebruikers. Microsoft heeft extra veel moeite gedaan om ervoor te zorgen dat er geen persoonsgegevens worden vastgelegd en dat alle gegevens die in deze database worden opgenomen afdoende worden beveiligd. Voor deze database zijn geen extra beveiligingsmaatregelen vereist, tenzij de database wordt verplaatst naar een andere computer waarop SQL-server wordt uitgevoerd. Als de database naar een andere server wordt verplaatst, moet u ervoor zorgen dat in de nieuwe omgeving dezelfde beveiligingsmechanismen worden toegepast.
-   **Configuratiedatabase**. Op de persoonlijke sleutels van de server na is deze database de belangrijkste en meest waardevolle bron in uw RMS-implementatie. In deze database worden gevoelige en essentiële gegevens opgenomen die goed moeten worden beveiligd. Deze database bevat de certificaten en sleutels, de gecodeerde persoonlijke sleutel van de server (tenzij u de aanbevolen hardwarecodering gebruikt), de hash met het wachtwoord van de persoonlijke sleutel en de configuratiegegevens.

Wanneer de RMS-configuratiedatabase wordt gemaakt, worden er machtigingen ingesteld waarmee de toegang wordt beperkt en de beveiliging van de database wordt verbeterd.

Databasebeveiliging verbeteren
------------------------------

U kunt de volgende extra maatregelen nemen om de algehele beveiliging van de databases in de netwerk- en serveromgeving te verbeteren:

-   Voer de databaseserver uit op een computer met Windows Server 2003. Dit besturingssysteem is standaard beter beveiligd dan Windows 2000 Server. U kunt een Windows 2000 Server-computer weliswaar vergrendelen, maar dit kan lang duren en u kunt fouten maken waarvan kwaadwillende gebruikers kunnen profiteren om toegang te krijgen tot uw database.
-   Beperk de fysieke toegang tot de databaseserver.
-   Stel de databasemachtigingen en DACL's voor databasebestanden zo in, dat alleen gemachtigde medewerkers toegang hebben. De standaardmachtigingen en DACL's in RMS zijn veilig. Wijzig een standaardinstelling alleen als u de op de hoogte bent van de consequenties.
-   Voer geen overbodige services op de databaseserver uit, zoals Microsoft Internet Information Services (IIS), Message Queuing of Terminal Services.
-   Voer alleen RMS-databases uit op de databaseserver.

Beveilig SQL Server-databases met SSL (Secure Sockets Layer) of IPsec (Internet Protocol security) om gecodeerde kanalen te bieden. Met gecodeerde databasecommunicatie helpt u voorkomen dat kwaadwillende gebruikers toegang kunnen krijgen tot of wijzigingen kunnen doorvoeren in vastgelegde gegevens.

Raadpleeg voor meer informatie over het configureren van SSL voor SQL Server, de website van MSDN ([http://go.microsoft.com/fwlink/?LinkID=17060](http://go.microsoft.com/fwlink/?linkid=17060)).

Raadpleeg voor meer informatie over het configureren van IPsec voor SQL Server 2000, de website van MSDN ([http://go.microsoft.com/fwlink/?LinkID=17061](http://go.microsoft.com/fwlink/?linkid=17061)).

Download voor meer informatie over het beveiligen van de Microsoft Windows Server 2003-besturingssystemen de "Windows Server 2003 Security Guide" vanaf het Microsoft Downloadcentrum ([http://go.microsoft.com/fwlink/?LinkId=36719](http://go.microsoft.com/fwlink/?linkid=36719)).
