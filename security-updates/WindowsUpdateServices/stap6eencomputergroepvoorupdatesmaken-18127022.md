---
TOCTitle: 'Stap 6: Een computergroep voor updates maken'
Title: 'Stap 6: Een computergroep voor updates maken'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18127022
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc708629(v=WS.10)'
---

Stap 6: Een computergroep voor updates maken
============================================

Computergroepen vormen een belangrijk onderdeel van een WSUS-implementatie, zelfs in een zeer eenvoudige implementatie. Computergroepen stellen u in staat bepaalde updates op specifieke computers wel en op andere niet te installeren. Er zijn twee standaardcomputergroepen: Alle computers en Niet-toegewezen computers. Op het moment dat een clientcomputer voor het eerst verbinding maakt met de WSUS-server, wordt deze computer standaard aan deze beide groepen toegevoegd.

U kunt aangepaste computergroepen maken. Een ander voordeel van computergroepen is dat ze u in staat stellen updates te testen voordat u deze updates op grotere schaal implementeert. Als uit de test blijkt dat de update geen schade aanricht, kunnen de updates ook worden geïnstalleerd op de computers van de groep Alle computers. Er geldt geen beperking voor het aantal aangepaste groepen dat u kunt maken.

**Computergroepen instellen**
1.  Geef op hoe u computers aan computergroepen wilt toewijzen. U hebt twee keuzemogelijkheden: toewijzing vanaf de server en toewijzing vanaf de client. Als u kiest voor toewijzing vanaf de server, moet u elke computer handmatig aan de gewenste groep toevoegen met behulp van WSUS. Als u kiest voor toewijzing vanaf de client, worden clients automatisch toegevoegd met behulp van groepsbeleid of registersleutels.

2.  Maak de computergroep op de WSUS-server.

3.  Plaats de computers in groepen aan de hand van de methode die u in stap 1 hebt gekozen.

In dit gedeelte wordt uitgelegd hoe u toewijzing vanaf de server kunt gebruiken en hoe u computers handmatig naar hun groepen kunt verplaatsen via de WSUS-beheerconsole. Als er meerdere clientcomputers aan computergroepen moeten worden toegevoegd, kunt u ook toewijzing vanaf de client gebruiken, omdat u daarmee het toewijzen van computers aan computergroepen automatiseert.

U kunt stap 6 gebruiken om een testgroep te maken die ten minste één testcomputer bevat.

**Stap 6 omvat de volgende procedures:**

-   Een groep maken
-   Een computer aan de groep toevoegen

**Een groep maken**
1.  Vouw **Computers** uit in de WSUS-beheerconsole en selecteer **Alle computers.**

2.  Klik met de rechtermuisknop op **Alle computers** of ga naar het deelvenster **Acties** en klik op **Computergroep toevoegen**.

3.  Het dialoogvenster **Computergroep toevoegen** wordt geopend. Geef de naam van de nieuwe groep op.

Gebruik de volgende procedure om een clientcomputer aan de testgroep toe te voegen. Een clientcomputer die geschikt is als testcomputer, is een computer met software en hardware die representatief is voor het merendeel van de computers in het netwerk, maar die geen essentiële rol speelt. Op deze manier kunt u nagaan hoe goed de updates die u goedkeurt, functioneren op computers die vergelijkbaar zijn met de testcomputer.

**Een computer aan de groep toevoegen**
1.  Klik op **Computers** in de WSUS-beheerconsole.

2.  Klik op de groep van de computer die u wilt verplaatsen.

3.  Selecteer in de lijst met computers de computer die u wilt verplaatsen.

4.  Klik met de rechtermuisknop op **Lidmaatschap wijzigen**.

5.  Het dialoogvenster **Lidmaatschap van computergroep instellen** wordt geopend en een lijst met groepen wordt weergegeven.

6.  Selecteer de groep waarnaar u de computer wilt verplaatsen en klik op **OK**.
