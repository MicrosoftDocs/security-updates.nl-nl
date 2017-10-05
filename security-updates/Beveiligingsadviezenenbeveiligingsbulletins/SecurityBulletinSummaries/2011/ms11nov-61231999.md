---
TOCTitle: 'MS11-NOV'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor november 2011'
ms:assetid: 'ms11-nov'
ms:contentKeyID: 61231999
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms11-nov(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor november 2011
======================================================================

Gepubliceerd: dinsdag 8 november 2011

**Versie:** 1.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor november 2011.

Met de beveiligingsbulletins voor november 2011 wordt de vooraankondiging van de bulletins, die oorspronkelijk werd uitgegeven op 3 november 2011, vervangen. Ga voor meer informatie over de vooraankondiging naar [Vooraankondiging van Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=217213).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 9 november 2011 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van november](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487958). Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://go.microsoft.com/fwlink/?linkid=217214) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

Samenvattingen
--------------

<span></span>
In de volgende tabel staat de beveiligingsbulletins voor deze maand op volgorde van prioriteit.

Zie de volgende sectie **Software waarin dit probleem optreedt en Downloadlocaties** voor meer informatie over software die last heeft van een probleem.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bulletin-id</th>
<th style="border:1px solid black;" >Titel bulletin en samenvatting</th>
<th style="border:1px solid black;" >Maximaal prioriteitsniveau en gevolgen van het beveiligingslek</th>
<th style="border:1px solid black;" >Opnieuw opstarten vereist</th>
<th style="border:1px solid black;" >Software waarin dit probleem optreedt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229071">MS11-083</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in TCP/IP kan externe code worden uitgevoerd (2588516)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een aanvaller een ononderbroken reeks speciaal vervaardigde UDP-pakketten naar een gesloten poort op een doelsysteem stuurt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229638">MS11-085</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Windows Mail en Windows Meeting Space kan leiden tot uitvoering van externe code (2620704)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Door het beveiligingslek kan externe code worden uitgevoerd als een gebruiker een legitiem bestand (zoals een .eml- of .wcinv-bestand) opent dat zich in dezelfde netwerkmap bevindt als een speciaal vervaardigd DLL-bestand (Dynamic Link Library). Wanneer het legitieme bestand wordt geopend, kan Windows Mail of Windows Meeting Space proberen het DLL-bestand te laden en code in dat bestand uit te voeren. Een aanval lukt alleen als een gebruiker een niet-vertrouwde externe bestandssysteemlocatie of WebDAV-locatie bezoekt en vanaf die locatie een legitiem bestand (zoals een .eml- of .wcinv-bestand) opent dat vervolgens door een kwetsbare toepassing wordt geladen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229253">MS11-086</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Active Directory kan leiden tot misbruik van bevoegdheden (2630837)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Active Directory, Active Directory Application Mode (ADAM) en Active Directory Lightweight Directory Service (AD LDS) opgelost. Het beveiligingslek kan leiden tot misbruik van bevoegdheden als Active Directory wordt geconfigureerd voor het gebruik van LDAP over SSL (LDAPS) en een aanvaller een ingetrokken certificaat bemachtigt dat is gekoppeld aan een geldig domeinaccount en vervolgens dat ingetrokken certificaat gebruikt om zich aan te melden bij het Active Directory-domein. Standaard is Active Directory niet geconfigureerd voor het gebruik van LDAP over SSL.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=229245">MS11-084</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in de Windows-stuurprogramma's voor de kernelmodus kan leiden tot denial of service (2617657)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Windows opgelost. Het beveiligingslek kan leiden tot denial of service als een gebruiker een speciaal vervaardigd TrueType-lettertypebestand als een e-mailbijlage opent of naar een netwerkshare of WebDAV-locatie met een speciaal vervaardigd TrueType-lettertypebestand gaat. Een aanval lukt alleen als een gebruiker de niet-vertrouwde externe bestandssysteemlocatie of WebDAV-share met het speciaal vervaardigde TrueType-lettertypebestand bezoekt of het bestand opent als een e-mailbijlage. Een aanvaller kan een gebruiker er echter niet toe dwingen om deze handelingen uit te voeren. In plaats daarvan moet een aanvaller een gebruiker daartoe overhalen. In de meeste gevallen doet de aanvaller dat door de gebruiker ertoe te bewegen op een koppeling in een e-mailbericht of een verzoek in een expresbericht te klikken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Gemiddeld</a><br />
Denial of service</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden vermeld in volgorde van bulletin-id en daarna van CVE-id. Alleen beveiligingslekken met het prioriteitsniveau Kritiek of Belangrijk in de bulletins zijn opgenomen.
  
**Gebruik van deze tabel?**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins externe code wordt uitgevoerd en denial of service optreedt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de prioriteit van de implementatie van de updates van deze maand vast te stellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.
  
In de onderstaande kolommen verwijst "Nieuwste softwarerelease" naar de nieuwste release van de software en verwijst "Oudere softwarereleases" naar alle oudere, ondersteunde releases van de software die wordt genoemd in de tabel "Software waarin dit probleem optreedt" of de tabel "Software waarin dit probleem niet optreedt" in het bulletin.
  
| Bulletin-id                                               | Titel van beveiligingslek                                                              | CVE-id                                                                           | Beoordeling van het risico op misbruik door het uitvoeren van code voor de nieuwste softwarerelease              | Beoordeling van het risico op misbruik door het uitvoeren van code voor oudere softwarereleases                  | Beoordeling van het risico op misbruik door denial of service | Belangrijke opmerkingen |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|-------------------------|  
| [MS11-083](http://go.microsoft.com/fwlink/?linkid=229071) | Beveiligingslek met betrekking tot overloop van de referentieteller                    | [CVE-2011-2013](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2013) | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | [2](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Permanent                                                     | (Geen)                  |  
| [MS11-085](http://go.microsoft.com/fwlink/?linkid=229638) | Beveiligingslek in Windows Mail met betrekking tot het onveilig laden van bibliotheken | [CVE-2011-2016](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2016) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                  |  
| [MS11-086](http://go.microsoft.com/fwlink/?linkid=229253) | Beveiligingslek met betrekking tot het niet uitvoeren van LDAPS-verificatie            | [CVE-2011-2014](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2014) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Niet van toepassing                                           | (Geen)                  |
  
Software waarin het probleem optreedt en Downloadlocaties  
---------------------------------------------------------
  
<span></span>
In de volgende tabellen staan de bulletins volgens belangrijke softwarecategorie en prioriteit.
  
**Gebruik van deze tabellen**
  
In deze tabellen vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of -onderdeel in de tabel controleren of er nieuwe beveiligingsupdates zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.
  
**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.
  
#### Windows-besturingssysteem en -onderdelen

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="7">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=8c7c21c5-677d-4a5d-8f2b-8ca7691b6b00)  
(KB2616310)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=989cca2d-cce1-4f52-b50e-43152693f240)  
(KB2616310)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=08b27ce7-c32e-41e4-ad04-481c5eab17a7)  
(KB2601626)  
(Belangrijk)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f116824e-ea48-422d-b284-c9ffa7604bf5)  
(KB2616310)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=de5a74f2-2cc8-4677-b495-3a40fe3d6b9e)  
(KB2601626)  
(Belangrijk)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1af1b734-62c7-4e08-91c8-90b6d026da84)  
(KB2616310)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=6168bc67-3d59-450f-bd8a-02d61dabe16b)  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Geen
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc3fe87c-2493-431d-a904-dec9310f6042)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e08266d8-fffa-40bf-b8f6-10a65ee27524)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=2bd602cf-ae0d-4790-a5d0-6133fd7d01a0)  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=042c1a8f-834d-4eed-8a59-9e030ccc6d39)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4f2365ed-d50e-44d9-b859-1ec54d3b4d38)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=783521ad-5c50-4194-a582-4e5a1c9999e7)  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
Geen
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79382bf2-d2cb-42ea-92dc-64f949353521)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f82dc413-668c-4ca8-a8c8-db74f05346bc)\*\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory and Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b5688923-3914-4f6c-8bc9-036fb4870cc6)\*  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71ff3a89-d7ad-4dda-9e59-fab54b21bd5d)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06ad5637-56a1-4478-aaa0-063e877503c9)\*\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory and Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=51f47181-08f6-4de1-80e5-253355675965)\*  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1c0cb05-c284-49b1-ae4f-92813fdf520f)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2de5de74-e643-4045-9c22-ff95b0dbcafc)  
(Gemiddeld)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Laag**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4ddb4c2a-bada-49b0-ad78-e07e7e11ced7)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2307fa93-8e45-4841-a5a9-7e89960712f9)  
(Laag)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=b06f9f55-e3b2-4705-83d0-1b9f5de9d378)  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 voor 32-bits systemen en Windows 7 voor 32-bits systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=156c1bd9-55bc-482c-874b-61998d1ef153)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=05eef5d7-acf6-46e4-abfc-dc83f0a7cae5)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=62603d18-1b21-400c-8eba-202193182960)  
(Laag)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=790f1d99-96a5-438d-b433-895b692912ce)  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows 7 voor x64-systemen en Windows 7 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5c7db930-5495-43f0-928c-d586ac9e80d0)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS11-083**](http://go.microsoft.com/fwlink/?linkid=229071)
</td>
<td style="border:1px solid black;">
[**MS11-085**](http://go.microsoft.com/fwlink/?linkid=229638)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-086**](http://go.microsoft.com/fwlink/?linkid=229253)
</td>
<td style="border:1px solid black;" colspan="2">
[**MS11-084**](http://go.microsoft.com/fwlink/?linkid=229245)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Laag**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;" colspan="2">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f9f74a6-e984-4aab-837c-ef7286e7305f)\*  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c9cf6a22-f9ab-427a-9b16-33c60baaabb5)\*\*  
(Laag)
</td>
<td style="border:1px solid black;" colspan="2">
[Active Directory and Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=cc1e99af-fc67-400b-a82c-171f8c4d1ac9)\*  
(KB2601626)  
(Belangrijk)
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 voor x64-systemen en Windows Server 2008 R2 voor x64-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5d810dae-5c52-4155-b5c2-163d27be6e78)\*\*\*  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b20bfcbd-a515-4074-b56e-b82539fe5bad)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=012777f5-51f2-4944-91af-a9c79b8081a1)  
(Laag)
</td>
<td style="border:1px solid black;" colspan="2">
Niet van toepassing
</td>
<td style="border:1px solid black;" colspan="2">
[Windows Server 2008 R2 voor Itanium-systemen en Windows Server 2008 R2 voor Itanium-systemen met Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=395819e2-1028-44b7-ace4-ca754b1a7543)  
(Gemiddeld)
</td>
</tr>
</table>
 
**Opmerkingenvoor Windows Server 2008 en Windows Server 2008 R2**

**\*Treedt op bij Server Core-installatie.** Deze update is met hetzelfde prioriteitsniveau van toepassing op ondersteunde edities van Windows Server 2008 en Windows Server 2008 R2, zoals is aangegeven, ongeacht of deze zijn geïnstalleerd met de optie Server Core-installatie. Zie de TechNet-artikelen [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) en [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Server Core-installatie niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op de ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2, zoals is aangegeven, als deze zijn geïnstalleerd met behulp van de Server Core-installatieoptie. Zie de TechNet-artikelen [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) en [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Server Core-installatie is niet getroffen.** Het beveiligingslek dat wordt opgelost door deze update heeft geen invloed op de aangegeven ondersteunde edities van Windows Server 2008 of Windows Server 2008 R2 als deze zijn geïnstalleerd met de ServerCore-installatieoptie, ook al kunnen zich bestanden op het systeem bevinden die door dit beveiligingslek worden getroffen. Gebruikers die deze bestanden op hun systeem hebben, krijgen deze update toch aangeboden omdat de updatebestanden nieuwer zijn (met hogere versienummers) dan de bestanden die zich momenteel op uw systeem bevinden. Zie de TechNet-artikelen [Managing a Server Core Installation](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) en [Servicing a Server Core Installation](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008 en Windows Server 2008 R2. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging voor thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn beschikbaar op [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) en [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130). Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.

Gebruikers van Microsoft Office voor Mac kunnen Microsoft AutoUpdate voor Mac gebruiken om hun Microsoft-software up-to-date te houden. Raadpleeg [Automatisch op software-updates controleren](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea) voor meer informatie over het gebruik van Microsoft AutoUpdate voor Mac.

Ten slotte kunt u beveiligingsupdates downloaden uit de [Microsoft Update-catalogus](http://go.microsoft.com/fwlink/?linkid=96155). In de Microsoft Update-catalogus vindt u een doorzoekbare catalogus met inhoud die beschikbaar is gesteld via Windows Update en Microsoft Update, waaronder beveiligingsupdates, stuurprogramma's en service packs. Door tijdens het zoeken het nummer van het beveiligingsbulletin (bijvoorbeeld “MS07-036”) te gebruiken, kunt u alle beschikbare updates toevoegen aan uw winkelmand (waaronder de verschillende talen voor een update) en de map van uw keuze downloaden. Raadpleeg de veelgestelde vragen van de [Microsoft Windows Update-catalogus](http://go.microsoft.com/fwlink/?linkid=97900) voor meer informatie over de Microsoft Windows Update-catalogus.

**Richtlijnen voor detecteren en implementeren:**

Microsoft biedt zoekfuncties en richtlijnen voor het implementeren van beveiligingsupdates. Deze begeleiding bevat aanbevelingen en informatie die IT-professionals kunnen helpen verschillende hulpprogramma's voor het zoeken naar en toepassen van beveiligingsupdates te gebruiken. Zie [Microsoft Knowledge Base-artikel 961747](http://support.microsoft.com/kb/961747) voor meer informatie.

**Microsoft Baseline Security Analyzer**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders de nieuwste essentiële updates en beveiligingsupdates snel en betrouwbaar implementeren voor Microsoft Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 voor Microsoft Windows-besturingssysteem Windows 2000 en later.

Ga naar de website [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**System Center Configuration Manager 2007**

Configuration Manager 2007 Software-updates beheren vereenvoudigt de complexe taak van het verspreiden en beheren van updates aan IT-systemen binnen een onderneming. Met Configuration Manager 2007 kunnen IT-beheerders updates van Microsoft-producten verspreiden over diverse apparaten, waaronder pc's, laptops, servers en mobiele apparaten.

De geautomatiseerde beveiligingslekbeoordeling in Configuration Manager 2007 bepaalt of updates nodig zijn en rapporteert over aanbevolen acties. Software-updates beheren van Configuration Manager 2007 is ingebouwd in Microsoft Windows Software Update Services (WSUS), een langdurig geteste update-infrastructuur die vertrouwd is voor IT-beheerders over de gehele wereld. Zie [Software-updates beheren](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx) voor meer informatie over hoe beheerders Configuration Manager 2007 kunnen gebruiken om updates te implementeren. Ga naar [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx) voor meer informatie over Configuration Manager.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers.

**Opmerking** De algemene ondersteuning van System Management Server 2003 is beëindigd met ingang van 12 januari 2010. Voor meer informatie over productlevenscycli gaat u naar [Microsoft Support Lifecycle](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle). De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar. Zie **System Center Configuration Manager 2007**.

Voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren, gaat u naar [Scenario's en procedures voor Microsoft Systems Management Server 2003: Softwaredistributie en patchbeheer](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Voor informatie over SMS gaat u naar het [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Opmerking** SMS maakt gebruik van de Microsoft Baseline Security Analyzer om brede ondersteuning te kunnen bieden voor het zoeken en installeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en)) gebruiken.

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows-updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibility Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Microsoft Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Niet-beveiligingsupdates op MU, WU en WSUS:

Voor informatie over andere releases voor Windows Update en Microsoft Update (geen beveiligingsreleases), verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services. Heeft betrekking op alle Windows-inhoud.
-   [Updates van vorige maanden voor Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Toont alle nieuwe, herziene en opnieuw uitgebrachte updates voor alle Microsoft-producten behalve Microsoft Windows.

#### Microsoft Active Protections Program (MAPP)

Om de beveiliging voor klanten te verbeteren, verstrekt Microsoft bij elke maandelijkse uitgifte van beveiligingsupdates informatie over beveiligingslekken aan de grote producenten van beveiligingsprogramma's. Deze producenten kunnen dan die informatie over beveiligingslekken gebruiken om hun klanten een betere beveiliging te bieden door hun software of apparatuur aan te passen, zoals antivirusprogramma's, inbraakdetectiesystemen voor netwerken of inbraakpreventiesystemen voor hosts. Op de websites van de programmapartners (zie [Microsoft Active Protections Program (MAPP)-partners](http://go.microsoft.com/fwlink/?linkid=215201)) kunt u nagaan of de leveranciers van beveiligingsprogramma's hun producten steeds aanpassen.

#### Veiligheidsstrategieën en community

**Strategieën voor updatebeheer**

Op de website [Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) kunt u extra informatie vinden over aanbevelingen van Microsoft voor het toepassen van beveiligingsupdates.

**Verkrijgen van andere beveiligingsupdates**

Op de volgende locaties zijn updates verkrijgbaar voor andere beveiligingsproblemen:

-   Beveiligingsupdates zijn verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.
-   Updates voor consumentenplatforms zijn verkrijgbaar op de website [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747).
-   U kunt de beveiligingsupdates van deze maand die op Windows Update staan, via het ISO CD-imagebestand met beveiligingsupdates en essentiële updates vanaf het Downloadcentrum ophalen. Zie [Microsoft Knowledge Base-artikel 913086](http://support.microsoft.com/kb/913086) voor meer informatie.

**IT Pro Security-community**

Leer de beveiliging te verbeteren en uw IT-infrastructuur te optimaliseren en bespreek beveiligingsonderwerpen met andere IT-professionals op de website [IT Pro Security Community](http://go.microsoft.com/fwlink/?linkid=21164).

#### Dankbetuiging

Microsoft [bedankt](http://go.microsoft.com/fwlink/?linkid=21127) de volgende partijen voor de samenwerking bij het verbeteren van de beveiliging voor klanten:

-   Will Dorman van de [CERT/CC](http://www.cert.org/) voor het melden van het probleem dat wordt beschreven in MS11-084
-   Ivan Sanchez van EvilCode voor het melden van een probleem dat wordt beschreven in MS11-085
-   Xavier Lassoie en Sébastien Godard van Autosécurité voor het melden van een probleem dat wordt beschreven in MS11-086

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (8 november 2011): Samenvatting van de gepubliceerde bulletins.

*Built at 2014-04-18T01:50:00Z-07:00*
