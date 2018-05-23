---
TOCTitle: 'MS08-JUL'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor juli 2008'
ms:assetid: 'ms08-jul'
ms:contentKeyID: 61231959
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms08-jul(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor juli 2008
==================================================================

Gepubliceerd: dinsdag 8 juli 2008 | Bijgewerkt: woensdag 11 februari 2009

**Versie:** 1.1

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor juli 2008.

Met de release van de bulletins voor juli 2008 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die oorspronkelijk werd uitgegeven op 3 juli 2008. Ga voor meer informatie over de vooraankondiging van de bulletins naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op woensdag 9 juli 2008 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van juli.](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032374629&culture=en-us) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

### Bulletininformatie

#### Samenvattingen

De beveiligingsbulletins zijn voor deze maand als volgt, in volgorde van prioriteit:

Belangrijk (4)
--------------

<span></span>

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-040                                                                                                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslekken in Microsoft SQL Server kunnen leiden tot misbruik van bevoegdheden (941203)**](http://technet.microsoft.com/security/bulletin/ms08-040)                                                                                                                                                                                                                                                                         |
| **Samenvatting**                          | Met deze beveiligingsupdate worden vier privé gemelde beveiligingslekken opgelost. In het ergste geval kan er als gevolg van het beveiligingslek externe code worden uitgevoerd door een aanvaller die volledige controle over een getroffen systeem kan krijgen. Een geverifieerde aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, en nieuwe accounts met volledige beheerdersrechten maken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                             |
| **Gevolgen van het beveiligingslek**      | Misbruik van bevoegdheden                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Mogelijk moet voor deze update het systeem opnieuw worden gestart.                                                                                                                                                                                                                                                           |
| **Software waarin dit probleem optreedt** | **Microsoft Windows, Microsoft SQL Server.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                        |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-038                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|-------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Beveiligingslek in Windows Verkenner kan leiden tot uitvoering van externe code (950582)**](http://technet.microsoft.com/security/bulletin/ms08-038)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Samenvatting**                          | Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek in Windows Verkenner opgelost waardoor externe code kan worden uitgevoerd wanneer een speciaal vervaardigd, opgeslagen zoekbestand wordt geopend en opgeslagen. Als er een gebruiker met beheerdersrechten is aangemeld, kan een aanvaller die misbruik weet te maken van dit beveiligingslek, volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Gevolgen van het beveiligingslek**      | Uitvoering van externe code mogelijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

| Bulletin-id                               | Microsoft-beveiligingsupdateMS08-037                                                                                                                                                                                                                                                                                                                                 |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in DNS is spoofing mogelijk (953230)**](http://technet.microsoft.com/security/bulletin/ms08-037)                                                                                                                                                                                                                                          |
| **Samenvatting**                          | Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in het Windows Domain Name System (DNS) waardoor spoofing mogelijk is, opgelost. Door deze beveiligingslekken, die voorkomen in zowel de DNS-client als de DNS-server, kan een externe aanvaller netwerkverkeer voor systemen op internet omleiden naar de eigen systemen van de aanvaller. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                           |
| **Gevolgen van het beveiligingslek**      | Spoofing                                                                                                                                                                                                                                                                                                                                                             |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. De computer moet voor deze update opnieuw worden opgestart.                                                                                                                                                                                                |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                            |

| Bulletin-id                               | Microsoft-beveiligingsbulletin MS08-039                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel bulletin**                        | [**Door beveiligingslekken in Outlook Web Access voor Exchange Server is misbruik van bevoegdheden mogelijk (953747)**](http://technet.microsoft.com/security/bulletin/ms08-039)                                                                                                                                                                                                                                                                                         |
| **Samenvatting**                          | Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken in Outlook Web Access (OWA) voor Microsoft Exchange Server opgelost. Een aanvaller die misbruik weet te maken van deze beveiligingslekken, kan toegang krijgen tot de sessiegegevens van een individuele OWA-client, waardoor misbruik van bevoegdheden mogelijk is. De aanvaller kan dan alle handelingen uitvoeren die de gebruiker kan uitvoeren in de OWA-sessie van de individuele client. |
| **Maximaal prioriteitsniveau**            | [Belangrijk](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Gevolgen van het beveiligingslek**      | Misbruik van bevoegdheden                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Detectie**                              | Met Microsoft Baseline Security kan worden vastgesteld of deze update voor uw computersysteem is vereist. Mogelijk moet voor deze update het systeem opnieuw worden gestart.                                                                                                                                                                                                                                                                                             |
| **Software waarin dit probleem optreedt** | **Microsoft Windows.** Zie de sectie Software waarin het probleem optreedt en de sectie Downloadlocaties.                                                                                                                                                                                                                                                                                                                                                                |

Software waarin het probleem optreedt en Downloadlocaties
---------------------------------------------------------

<span></span>
**Gebruik van deze tabel**

In deze tabel vindt u informatie over de beveiligingsupdates die u mogelijk moet installeren. U moet voor elk softwareprogramma of onderdeel in de tabel controleren of er beveiligingsupdates vereist zijn. Indien een softwareprogramma of onderdeel is vermeld, wordt er een hyperlink naar de verkrijgbare software-update weergegeven en wordt ook het prioriteitsniveau van de software-update vermeld.

**Opmerking** voor één beveiligingslek moet u mogelijk verschillende beveiligingsupdates installeren. Bekijk de gehele kolom van elke bulletin-id die wordt weergegeven om te controleren of de te installeren updates zijn gebaseerd op de programma's of onderdelen die u op uw systeem hebt geïnstalleerd.

#### Windows-besturingssysteem

 
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
</tr>
<tr>
<th colspan="4">
Microsoft Windows 2000:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://technet.microsoft.com/security/bulletin/ms08-040)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://technet.microsoft.com/security/bulletin/ms08-038)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://technet.microsoft.com/security/bulletin/ms08-037)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=269c219c-9d6b-4b12-b621-c70cd07cdd22)  
(Belangrijk)  
DNS-serverupdate:  
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=332aa92f-a1ad-42a0-87d0-485d2d41335b)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://technet.microsoft.com/security/bulletin/ms08-040)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://technet.microsoft.com/security/bulletin/ms08-038)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://technet.microsoft.com/security/bulletin/ms08-037)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ed989a33-7a9e-4423-93a8-b38907467cdf)  
(Belangrijk)  
Geen DNS-serverupdate toepasbaar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Windows XP Professional x64 Edition en Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a2b016fa-b108-4e8e-b41b-4ca89002907b)  
(Belangrijk)  
Geen DNS-serverupdate toepasbaar
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://technet.microsoft.com/security/bulletin/ms08-040)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://technet.microsoft.com/security/bulletin/ms08-038)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://technet.microsoft.com/security/bulletin/ms08-037)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Belangrijk)  
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4ef5033c-9843-4e0b-bfad-fcaf05d7dab9)  
(Belangrijk)  
DNS-serverupdate:  
[Windows Server 2003 Service Pack 1 en Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d1fcb794-e6a5-4c28-b3b3-9cd88f468a42)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?familyid=1c0ae18b-1f17-44b3-a337-b36e7de437a7)  
(KB948110)  
(Belangrijk)  
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)  
(KB948109)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=66624a1f-38bf-4af7-936d-3131474ffe1f)  
(Belangrijk)  
DNS-serverupdate:  
[Windows Server 2003 x64 Edition en Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=040a1ba8-21b0-439e-bf21-1acd1c43b162)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
DNS-clientupdate:  
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=facc80da-61d6-49c5-872d-a1980b66ae3e)  
(Belangrijk)  
DNS-serverupdate:  
[Windows Server 2003 met SP1 voor Itanium-systemen en Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=c63e3ee6-6055-4313-b0f1-fec7408886bb)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://technet.microsoft.com/security/bulletin/ms08-040)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://technet.microsoft.com/security/bulletin/ms08-038)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://technet.microsoft.com/security/bulletin/ms08-037)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista en Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista en Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=06739ca6-7368-4acb-bb67-7e8146071a29)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Geen DNS-clientupdate toepasbaar  
Geen DNS-serverupdate toepasbaar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition en Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=74ea0893-7c2f-4fad-ad27-588ad953b046)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Geen DNS-clientupdate toepasbaar  
Geen DNS-serverupdate toepasbaar
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS08-040**](http://technet.microsoft.com/security/bulletin/ms08-040)
</td>
<td style="border:1px solid black;">
[**MS08-038**](http://technet.microsoft.com/security/bulletin/ms08-038)
</td>
<td style="border:1px solid black;">
[**MS08-037**](http://technet.microsoft.com/security/bulletin/ms08-037)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Maximaal prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen
</td>
<td style="border:1px solid black;">
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=189a4170-b495-4904-9cbd-209e7494d303)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Geen DNS-clientupdate toepasbaar  
DNS-serverupdate:  
[Windows Server 2008 voor 32-bits systemen](http://www.microsoft.com/downloads/details.aspx?familyid=1fcea8f4-b233-42e1-b913-c4fcae276c7b)\*  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen
</td>
<td style="border:1px solid black;">
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f6aaa5-49fc-4a16-bc34-8514e214b8cf)\*  
(KB948109)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=85d8701d-f8c7-4079-8a21-a3a9d5ba71ce)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Geen DNS-clientupdate toepasbaar  
DNS-serverupdate:  
[Windows Server 2008 voor x64-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=afac5bbc-71fa-457b-8b0a-f5902d37bfd0)\*  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=b30ee4f0-850f-4ff3-86a4-663603a0a802)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Geen DNS-clientupdate toepasbaar  
Geen DNS-serverupdate toepasbaar
</td>
</tr>
</table>
 
**\*Windows Server 2008 Server Core-installatie is getroffen.** Voor ondersteunde edities van Windows Server 2008 is deze update van toepassing met hetzelfde prioriteitsniveau, ongeacht of Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Server-software

 
<table style="border:1px solid black;">
<caption>Microsoft SQL Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-040"><strong>MS08-040</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 7.0 Service Pack 4</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">SQL Server 7.0 Service Pack 4</a><br />
(KB948113)<br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000 Service Pack 4</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 Service Pack 4</a><br />
(KB948110)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 Service Pack 4</a><br />
(KB948111)<br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2000 Itanium-editie Service Pack 4</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">SQL Server 2000 Itanium-editie Service Pack 4</a><br />
(KB948110)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">SQL Server 2000 Itanium-editie Service Pack 4</a><br />
(KB948111)<br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 Service Pack 2</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 Service Pack 2</a><br />
(KB948109)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 Service Pack 2</a><br />
(KB948108)<br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948109)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 x64 Edition Service Pack 2</a><br />
(KB948108)<br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2005 met SP2 voor Itanium-systemen</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">SQL Server 2005 met SP2 voor Itanium-systemen</a><br />
(KB948109)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">SQL Server 2005 met SP2 voor Itanium-systemen</a><br />
(KB948108)<br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c95b2cb3-51a4-44e4-b9f4-9416e9ce16a0">Microsoft Data Engine (MSDE) 1.0 Service Pack 4</a><br />
(KB948113)<br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4fd1f86a-94a2-43d8-9b0a-774c81426d9e">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948110)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=8316bc5e-8c2d-4710-8acc-b815ccc81cd4">Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4</a><br />
(KB948111)<br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition Service Pack 2</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948109)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition Service Pack 2</a><br />
(KB948108)<br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft SQL Server 2005 Express Edition met Advanced Services Service Pack 2</td>
<td style="border:1px solid black;">GDR-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c9851cc-2c4c-4190-872c-84993a7623b7">Microsoft SQL Server 2005 Express Edition met Advanced Services Service Pack 2</a><br />
(KB948109)<br />
(Belangrijk)<br />
<br />
QFE-update:<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a60bb7e7-ef4e-4cbd-b63a-0ad7bd1402b3">Microsoft SQL Server 2005 Express Edition met Advanced Services Service Pack 2</a><br />
(KB948108)<br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Microsoft Exchange Server</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bulletin-id</strong></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms08-039"><strong>MS08-039</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Maximaal prioriteitsniveau</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Belangrijk</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e099c1d1-5af6-4d6c-b735-9599412b3131">Microsoft Exchange Server 2003 Service Pack 2</a><br />
(Belangrijk)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Exchange Server 2007</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=086a2a13-a1de-4b1d-bd12-b148bfd2dafa">Microsoft Exchange Server 2007</a><br />
(Belangrijk)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Exchange Server 2007 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=63e7f26c-92a8-4264-882d-f96b348c96ab">Microsoft Exchange Server 2007 Service Pack 1</a><br />
(Belangrijk)</td>
</tr>
</tbody>
</table>
 

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging voor thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

Beveiligingsupdates zijn verkrijgbaar via [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) en [Office Update](http://go.microsoft.com/fwlink/?linkid=21135). Beveiligingsupdates zijn ook verkrijgbaar via het [Microsoft Downloadcentrum](http://go.microsoft.com/fwlink/?linkid=21129). U vindt deze updates het snelst door een zoekactie uit te voeren met als trefwoord "security update''.

Ten slotte kunt u beveiligingsupdates downloaden uit de [Microsoft Update-catalogus](http://go.microsoft.com/fwlink/?linkid=96155). In de Microsoft Update-catalogus vindt u een doorzoekbare catalogus met inhoud die beschikbaar is gesteld via Windows Update en Microsoft Update, waaronder beveiligingsupdates, stuurprogramma's en service packs. Door tijdens het zoeken het nummer van het beveiligingsbulletin (bijvoorbeeld “MS07-036”) te gebruiken, kunt u alle beschikbare updates toevoegen aan uw winkelmand (waaronder de verschillende talen voor een update) en de map van uw keuze downloaden. Raadpleeg de [veelgestelde vragen van de Microsoft Windows Update-catalogus](http://go.microsoft.com/fwlink/?linkid=97900) voor meer informatie over de Microsoft Windows Update-catalogus.

**Richtlijnen voor detecteren en implementeren**

Microsoft heeft richtlijnen voor detecteren en implementeren uitgebracht voor de beveiligingsupdates van deze maand. Aan de hand van deze richtlijnen kunnen IT-professionals zien hoe zij met diverse middelen, zoals Windows Update, Microsoft Update, Office Update, de Microsoft Baseline Security Analyzer (MBSA), de Office Detection Tool, Microsoft Systems Management Server (SMS) en de Extended Security Update Inventory Tool (ESUIT) de beveiligingsupdate kunnen implementeren. Zie [Microsoft Knowledge Base-artikel 910723](http://support.microsoft.com/kb/910723) voor meer informatie.

**Microsoft Baseline Security Analyzer**

Met de Microsoft Baseline Security Analyzer (MBSA) kunnen beheerders lokale en externe systemen scannen op ontbrekende beveiligingsupdates en algemene, onjuiste beveiligingsconfiguraties. Ga naar de website [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) voor meer informatie over MBSA.

**Windows Server Update Services:**

Als Windows Server Update Services (WSUS) wordt gebruikt, kunnen beheerders snel en betrouwbaar de nieuwste essentiële updates en beveiligingsupdates implementeren voor Windows-besturingssysteem Windows 2000 en later, Office XP en later, Exchange Server 2003 en SQL Server 2000 en later.

Ga naar de website [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) voor meer informatie over hoe u deze beveiligingsupdate kunt implementeren met behulp van Windows Server Update Services.

**Systems Management Server**

Microsoft Systems Management Server (SMS) is een configureerbare bedrijfsoplossing voor het beheer van updates. Met SMS kunnen beheerders bepalen of beveiligingsupdates nodig zijn voor Windows-systemen, en deze updates in de gehele organisatie gecontroleerd implementeren met minimaal ongemak voor de eindgebruikers. De volgende release van SMS, System Center Configuration Manager 2007, is nu verkrijgbaar; zie ook [System Center Configuration Manager 2007.](http://technet.microsoft.com/en-us/library/bb735860.aspx) Ga naar de website [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939) voor meer informatie over hoe beheerders SMS 2003 kunnen gebruiken om beveiligingsupdates te implementeren. SMS 2.0-gebruikers kunnen ook het [Software Updates Service Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340) gebruiken voor de implementatie van beveiligingsupdates. Ga naar de website [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) voor meer informatie over SMS.

**Opmerking:** SMS maakt gebruik van de Microsoft Baseline Security Analyzer en de Microsoft Office Detection Tool om brede ondersteuning te kunnen bieden voor het zoeken en uitvoeren van beveiligingsupdates. Bepaalde software-updates worden mogelijk niet opgemerkt door deze hulpprogramma's. Beheerders kunnen in deze gevallen de inventarisatiefuncties van SMS gebruiken om de updates op bepaalde systemen uit te voeren. Zie [Software-updates implementeren met de distributiefunctie van de SMS-software](http://go.microsoft.com/fwlink/?linkid=33341) voor meer informatie over deze procedure. Voor bepaalde beveiligingsupdates zijn beheerdersrechten vereist na het opnieuw opstarten van het systeem. Beheerders kunnen voor het installeren van deze updates de Elevated Rights Deployment Tool gebruiken (die deel uitmaakt van het [SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) en het [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161)).

**Update Compatibility Evaluator en Application Compatibility Toolkit**

Updates schrijven vaak naar de bestanden en registerinstellingen die nodig zijn om uw toepassingen te kunnen uitvoeren. Hierdoor kunnen incompatibiliteiten worden veroorzaakt en duurt het langer om beveiligingsupdates te implementeren. U kunt het testen en valideren van Windows Updates ten opzichte van geïnstalleerde toepassingen stroomlijnen met de [Update Compatibiliteit Evaluator](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true)-componenten die onderdeel zijn van [Application Compatibility Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en).

De Application Compatibility Toolkit (ACT) bevat de noodzakelijke hulpprogramma's en documentatie om problemen met de compatibiliteit van toepassingen te evalueren en te verminderen voordat Microsoft Windows Vista, een Windows-update, een Microsoft-beveiligingsupdate of een nieuwe versie van Windows Internet Explorer op uw systeem wordt geïnstalleerd.

### Overige informatie

#### Hulpprogramma voor het verwijderen van schadelijke software uit Microsoft Windows

Microsoft heeft een bijgewerkte versie van het nieuwe Windows-programma voor het verwijderen van schadelijke software op Windows Update, Microsoft Update, Windows Server Update Services en het Downloadcentrum geplaatst.

#### Belangrijke niet-beveiligingsupdates op MU, WU en WSUS:

Voor informatie over releases op Windows Update en Microsoft Update die geen beveiligingsreleases zijn, verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services voor 2008. Heeft betrekking op alle Windows-inhoud.
-   [Nieuwe, herziene en vrijgegeven updates voor Microsoft-producten behalve Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   Dan Kaminsky van [IOActive](http://www.ioactive.com/) voor het melden van een probleem dat wordt beschreven in MS08-037.
-   Michael Jordan van [Context Information Security](http://www.contextis.co.uk/) voor het melden van een probleem dat wordt beschreven in MS08-039.
-   Een anonieme onderzoeker voor het melden van een probleem dat wordt beschreven in MS08-040.
-   Een anonieme onderzoeker voor het melden van een probleem dat wordt beschreven in MS08-040.
-   Brett Moore van [Insomnia Security](http://www.insomniasec.com/), die werkt bij [iDefense VCP](http://labs.idefense.com/), voor het melden van een probleem dat wordt beschreven in MS08-040.
-   Een anonieme onderzoeker voor het melden van een probleem dat wordt beschreven in MS08-040.

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Microsoft Product Support Services](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (8 juli 2008): Samenvatting van de gepubliceerde bulletins.
-   V1.1 (11 februari 2009): Onder MS08-040 foutieve verwijzing naar Microsoft SQL Server 2000 Desktop Engine (WMSDE) op Microsoft Windows 2000 Service Pack 4 verwijderd uit de tabel Software waarin dit probleem optreedt en downloadlocaties voor Windows-besturingssysteem.

*Built at 2014-04-18T01:50:00Z-07:00*
