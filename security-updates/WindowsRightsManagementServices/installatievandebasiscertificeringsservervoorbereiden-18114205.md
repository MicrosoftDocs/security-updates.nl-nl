---
TOCTitle: Installatie van de basiscertificeringsserver voorbereiden
Title: Installatie van de basiscertificeringsserver voorbereiden
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18114205
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747726(v=WS.10)'
---

Installatie van de basiscertificeringsserver voorbereiden
=========================================================

Bij de testinstallatie in het voorbeeld wordt slechts één basiscertificeringsserver gebruikt. Desgewenst kunt u meer servers instellen, als onderdeel van een basiscertificeringscluster of als apart licentieservercluster. Aangezien de infrastructuurinstelling voor alle servers overeenkomt, moet u de hier beschreven procedure op elke server uitvoeren.

Als u de domeincontroller hebt geïnstalleerd, de databaseservers hebt ingesteld (zie het vorige gedeelte) en de stappen in de volgende tabel hebt uitgevoerd, kunt u RMS gaan installeren.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Infrastructuuronderdeel</th>
<th>De server voorbereiden voor de installatie van RMS</th>
<th>Opmerkingen voor implementatie in een productieomgeving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Besturingssysteem</td>
<td style="border:1px solid black;">Installeer Windows 2003 Server op een computer die voldoet aan de hardwarevereisten voor RMS, maar nog niet is aangesloten op een netwerk. Gebruik het NTFS-bestandssysteem voor de partitie.</td>
<td style="border:1px solid black;">U wordt aangeraden altijd het meest recente Service Pack en de meest recente patches te installeren. Gebruik partities met NTFS-formattering.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetverbinding
(optioneel)</td>
<td style="border:1px solid black;">Maak een Ethernet-verbinding met een netwerk met internetverbinding dat geïsoleerd is van de productieomgeving. Als u de RMS-server on line wilt inschrijven als onderdeel van het inrichtingsproces, moet de server een internetverbinding hebben.</td>
<td style="border:1px solid black;">Zorg ervoor dat er een firewall is geïnstalleerd als u on line (via internet) gaat inschrijven.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IP-adres</td>
<td style="border:1px solid black;">Wijs een statisch IP-adres aan deze computer toe.</td>
<td style="border:1px solid black;">Gebruik altijd statische IP-adressen voor servers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Deze computer toevoegen aan het domein</td>
<td style="border:1px solid black;">Meld u als lokale beheerder bij de computer aan. Klik op <strong>Start</strong>, klik met de rechtermuisknop op <strong>Deze computer</strong> en kies <strong>Eigenschappen.</strong> Klik vervolgens op de tab <strong>Computernaam</strong> en op <strong>Wijzigen</strong>.</td>
<td style="border:1px solid black;">Gebruik hetzelfde domein voor alle servers.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Klik op <strong>Domein</strong>, typ de naam van het domein (bijvoorbeeld Contoso.com) en klik op <strong>OK</strong>. Geef de gebruikersreferenties op waarmee u aan het domein kunt worden toegevoegd en klik op <strong>OK</strong>. Start de computer vervolgens opnieuw op wanneer hierom wordt verzocht. Als de computer opnieuw is opgestart en u naar aanmeldingsreferenties wordt gevraagd, dient u het domein, de gebruikersnaam en het wachtwoord op te geven.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Gebruiker en aanmelden</td>
<td style="border:1px solid black;">Klik met de rechtermuisknop op <strong>Deze computer</strong> en kies <strong>Beheren</strong>. Klik op <strong>Lokale gebruikers en groepenGroepen</strong> en dubbelklik op <strong>Administrators</strong>.
Klik op <strong>Toevoegen</strong>, geef de naam op van de gebruikersaccount die u wilt toevoegen (bijvoorbeeld Michael@contoso.com) en klik op <strong>OK</strong>. Wijs aan de gebruikersaccount Administrator-bevoegdheden toe. Wanneer u om referenties wordt gevraagd, dient u deze op te geven (bijvoorbeeld Contoso\Administrator).
Meld u op de computer aan als domeingebruiker met Administrator-bevoegdheden.</td>
<td style="border:1px solid black;">Als u onderdelen wilt toevoegen aan de computer, moet u over Administrator-bevoegdheden beschikken. Sommige installatiestappen kunnen niet worden uitgevoerd met de account van de lokale beheerder. U moet op deze server minstens één domeingebruiker instellen als beheerder. Daarnaast kunnen in SQL Server alleen systeembeheerders nieuwe databases maken.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetverbinding
(optioneel)</td>
<td style="border:1px solid black;">Ga met een internetbrowser naar http://uddi.microsoft.com/ om te controleren of u toegang hebt tot internet. Op computers met Windows Server 2003 moeten de Lmhosts- en Hosts-bestanden mogelijk worden gewijzigd om de domeincontroller op te nemen.</td>
<td style="border:1px solid black;">Ga naar http://uddi.microsoft.com om te controleren of u toegang hebt tot internet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-activering</td>
<td style="border:1px solid black;">U kunt Windows met de activeringswizard via een internetverbinding of telefonisch bij Microsoft activeren. Raadpleeg Help en ondersteuning van Windows Server 2003 voor meer informatie over de activering van Windows Server 2003.</td>
<td style="border:1px solid black;">Windows Server 2003 moet binnen 14 dagen na installatie worden geactiveerd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Software-updates</td>
<td style="border:1px solid black;">De meest recente softwarepatches moeten zijn geïnstalleerd voor de software die op deze computer is geïnstalleerd.</td>
<td style="border:1px solid black;">Installeer de nieuwste software-updates.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet Explorer configureren</td>
<td style="border:1px solid black;">RMS gebruikt voor het beheer een webinterface. Door sommige standaard beveiligingsinstellingen worden pagina's niet goed weergegeven. Bij sommige pagina's op de beheerwebsite van RMS worden pop-upvensters voor sommige configuratieopties gebruikt.</td>
<td style="border:1px solid black;"> </td>
</tr>
</tbody>
</table>
  
Als u de bovenstaande stappen op beide servers hebt uitgevoerd, kunt u RMS installeren en inrichten op de servers.
