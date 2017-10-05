---
TOCTitle: 'Stap 6: Een computergroep maken'
Title: 'Stap 6: Een computergroep maken'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18126832
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720536(v=WS.10)'
---

Stap 6: Een computergroep maken
===============================

Computergroepen vormen een belangrijk onderdeel van een WSUS-implementatie, zelfs in een zeer eenvoudige implementatie. Computergroepen stellen u in staat bepaalde updates op specifieke computers wel en op andere niet te installeren. Er zijn twee standaardcomputergroepen: Alle computers en Niet-toegewezen computers. Op het moment dat een clientcomputer voor het eerst verbinding maakt met de WSUS-server, wordt deze computer standaard aan deze beide groepen toegevoegd.

U kunt aangepaste computergroepen maken. Een ander voordeel van computergroepen is dat ze u in staat stellen updates te testen voordat u deze updates op grotere schaal installeert. Als uit de test blijkt dat de update geen schade aanricht, kunnen de updates ook worden geïnstalleerd op de computers van de groep Alle computers. Er geldt geen beperking voor het aantal aangepaste groepen dat u kunt maken.

Het instellen van computergroepen is een procedure die uit drie stappen bestaat. Ten eerste geeft u op hoe u computers aan computergroepen wilt toewijzen. U hebt twee keuzemogelijkheden: *toewijzing vanaf de server* en *toewijzing vanaf de client*. Als u kiest voor toewijzing vanaf de server, dient u elke computer handmatig aan de gewenste groep toe te voegen met behulp van WSUS. Als u kiest voor toewijzing vanaf de client, worden clients automatisch toegevoegd met behulp van groepsbeleid of registersleutels. Ten tweede maakt u de computergroepen op de WSUS-server. Ten derde verplaatst u de computers naar de groepen volgens de toewijzingsmethode die u bij de eerste stap hebt gekozen.

In dit document wordt uitgelegd hoe u toewijzing vanaf de server kunt gebruiken en hoe u computers handmatig naar hun groepen kunt verplaatsen via de WSUS-console. Als er erg veel clientcomputers aan computergroepen moeten worden toegevoegd, kunt u ook toewijzing vanaf de client gebruiken, omdat u daarmee het toewijzen van computers aan computergroepen automatiseert.

U kunt stap 6 gebruiken om een testgroep te maken die ten minste één testcomputer bevat.

Deze stap omvat de volgende procedures:

-   Opgeven dat u clientcomputers wilt toewijzen vanaf de server
-   Een groep maken
-   Computers naar de groep verplaatsen

**De methode voor het toewijzen van computers aan groepen opgeven**
1.  Klik op de werkbalk van de WSUS-console op **Opties** en klik vervolgens op **Opties voor computer**.

2.  Klik in het dialoogvenster **Opties voor computer** op **Gebruik de taak Computer verplaatsen in Windows Server Update Services**.

3.  Klik onder **Taken** op **Instellingen opslaan** en klik op **OK** om uw keus te bevestigen.

**Een groep maken**
1.  Klik op **Computers** op de werkbalk van de WSUS-console.

2.  Klik onder **Taken** op **Computergroep maken**.

3.  Typ **Test** in het vak **Groepsnaam** en klik vervolgens op **OK**.

Gebruik de volgende procedure om een clientcomputer die geschikt is als testcomputer, aan de groep Test toe te voegen. Een clientcomputer die geschikt is als testcomputer, is een computer met software en hardware die representatief is voor het merendeel van de computers in het netwerk, maar die geen essentiële rol speelt. Op deze manier kunt u nagaan hoe goed de updates die u goedkeurt, functioneren op computers die vergelijkbaar zijn met de testcomputer

**Een computer handmatig toevoegen aan de computergroep Test**
1.  Klik op **Computers** op de werkbalk van de WSUS-console.

2.  Klik in het vak **Groepen** op de groep van de computer die u wilt verplaatsen.

3.  Klik in de lijst met computers op de computer die u wilt verplaatsen.

4.  Klik onder **Taken** op **Geselecteerde computer verplaatsen**.

5.  Selecteer in de lijst **Computergroep** de groep waarnaar u de computer wilt verplaatsen en klik vervolgens op **OK**.
