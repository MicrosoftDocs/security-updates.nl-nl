---
TOCTitle: 'RMS-intrekkingslijsten'
Title: 'RMS-intrekkingslijsten'
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18113961
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720287(v=WS.10)'
---

RMS-intrekkingslijsten
======================

In intrekkingslijsten wordt opgegeven welke inhoud, toepassingen, gebruikers of andere principals zijn ingetrokken. Een of meer van de volgende redenen kunnen voor een organisatie aanleiding zijn een entiteit op te nemen in een intrekkingslijst:

-   Een persoonlijke sleutel is gewijzigd of vermoedelijk gewijzigd.
-   Een eigenaar verzoekt intrekking van een sleutel waarvan wordt vermoed dat deze is gewijzigd.
-   Een principal is niet meer geldig, bijvoorbeeld wanneer een werknemer is ontslagen.
-   Er is een beveiligingsprobleem (een certificaat dat aan een clientcomputer is uitgegeven, kan bijvoorbeeld zijn gewijzigd).
-   Opnieuw certificeren is vereist vanwege machtigingswijzigingen.
-   Een toepassing met RMS-ondersteuning ondervindt beveiligingsproblemen waardoor deze toepassing niet geschikt is voor het gebruik van zeer gevoelige of beveiligde inhoud.
-   Eerder gedistribueerde inhoud is nu gedateerd of niet meer geschikt voor gebruik.

In de volgende tabel worden de entiteiten beschreven die u kunt opgeven in een intrekkingslijst. Daarnaast wordt beschreven welke gegevens worden gebruikt voor het identificeren van deze entiteiten.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Entiteit</th>
<th>Id</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Een groep licenties of certificaten</td>
<td style="border:1px solid black;">Uitgever-id of openbare sleutel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Een groep toepassingsmanifesten</td>
<td style="border:1px solid black;">Uitgever-id of openbare sleutel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Een bepaalde licentie of een bepaald certificaat</td>
<td style="border:1px solid black;">Licentie-id of hash</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Een bepaald toepassingsmanifest</td>
<td style="border:1px solid black;">Licentie-id of hash</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Een bepaalde principal</td>
<td style="border:1px solid black;">Principal-id of openbare sleutel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bepaalde inhoud</td>
<td style="border:1px solid black;">Inhouds-id</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Voor intrekking en uitsluiting worden SHA-1-hashes gebruikt \[NIS94c\], een revisie van SHA (Secure Hash Algorithm). SHA-1 wordt gespecificeerd in de Secure Hash Standard (SHS, FIPS 180). SHA-1 wordt beschreven in deel 2 van de ANSI-norm X9.30. Om op toepassingsmanifest in te trekken dient u de gebruikers-id, openbare sleutel van de uitgever, licentie-id of licentie-hash van het toepassingsmanifest uit te pakken. Toepassingsmanifesten zijn echter gecodeerd volgens base 64. Informatie is niet beschikbaar in ongecodeerde weergave. Met de Rights Management Client SDK kunnen programma's worden ontwikkeld volgens de **DRMConstructCertificateChain**-, **DRMDeconstructCertificateChain**- en **DRMDecode**-methoden, die het toepassingsmanifest decoderen en de benodigde informatie opvragen. Als u wilt voorkomen dat een toepassing bepaalde door RMS beveiligde inhoud ophaalt, kunt u de desbetreffende toepassing uitsluiten zodat de RMS-server geen gebruikslicenties aan die toepassing kan verlenen. De beperking van uitsluiting is dat niet kan worden verhinderd dat iemand met een geldige gebruikerslicentie nog steeds door RMS beveiligde inhoud kan decoderen. Zie 'Toepassingen uitsluiten' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over het uitsluiten van toepassingen. |
  
Intrekkingslijsten zijn XrML-bestanden waarin de volgende parameters worden opgegeven.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Beschrijving</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">Het tijdstip (systeemtijd) waarop het XrML-bestand is gemaakt. Op basis van dit tijdstip wordt de leeftijd van de intrekkingslijst bepaald door de voorwaarde REFRESH in een gebruikslicentie.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">De naam, de id en het adres van de uitgever van de intrekkingslijst.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">De openbare sleutel van de uitgever van de intrekkingslijst.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">De naam, het type en de id van elke ingetrokken eenheid.</td>
</tr>
</tbody>
</table>
