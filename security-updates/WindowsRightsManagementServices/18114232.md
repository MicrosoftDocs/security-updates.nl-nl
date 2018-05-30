---
TOCTitle: Clustervereisten voor RMS plannen
Title: Clustervereisten voor RMS plannen
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18114232
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747792(v=WS.10)'
---

Clustervereisten voor RMS plannen
=================================

Als u RMS in een clusterinstallatie gebruikt, moet u weten hoe u met de volgende condities om moet gaan die binnen uw organisatie aanwezig kunnen zijn.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Voorwaarde</th>
<th style="border:1px solid black;" >Aanbevolen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Groot aantal computers dat RMS gebruikt.</td>
<td style="border:1px solid black;">U kunt de Microsoft Windows Rights Management Services-clientsoftware met behulp van Windows Update, een script of een softwaredistributiemethode, zoals Systems Management Server (SMS) of Groepsbeleid, installeren en activeren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Groot aantal aanvragen van clients.</td>
<td style="border:1px solid black;">Gebruik een taakverdelingsserver, de NLB-service (Network Load Balancing), of taakverdeling van de hardware om de aanvragen over het cluster te verdelen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Twee netwerkadapters die gebruikmaken van virtuele IP-adressering om aan de aanvragen van het extranet en het intranet te voldoen.</td>
<td style="border:1px solid black;">Zorg ervoor dat eventuele DNS-toewijzingen die worden uitgevoerd om het virtuele IP-adres zichtbaar te maken in het extranet, ook worden uitgevoerd om het adres zichtbaar te maken in het intranet.
Wordt voor het intranet geen DNS-registratie uitgevoerd, dan mislukken interne aanvragen voor gebruikslicenties. Als u de DNS-bronrecords niet kunt veranderen, wijzigt u de hosts-tabel van elke server in het cluster om de cluster-URL toe te wijzen aan het virtuele IP-adres van het cluster. De DNS-registratie moet zijn uitgevoerd voordat u RMS inricht. Als u RMS al hebt ingericht, moet u dit ongedaan maken en vervolgens het inrichtingsproces herhalen.</td>
</tr>
</tbody>
</table>
