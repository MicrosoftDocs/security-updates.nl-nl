---
TOCTitle: 'MS09-JUN'
Title: 'Samenvatting van de Microsoft-beveiligingsbulletins voor juni 2009'
ms:assetid: 'ms09-jun'
ms:contentKeyID: 61231972
ms:mtpsurl: 'https://technet.microsoft.com/nl-NL/library/ms09-jun(v=Security.10)'
---

Security Bulletin Summary

Samenvatting van de Microsoft-beveiligingsbulletins voor juni 2009
==================================================================

Gepubliceerd: dinsdag 9 juni 2009

**Versie:** 1.0

In dit bulletin wordt een overzicht gegeven van de beveiligingsbulletins voor juni 2009.

Met de release van de bulletins voor juni 2009 vervangt deze samenvatting van de bulletins de vooraankondiging van de bulletins die is uitgegeven op 4 juni 2009. Ga voor meer informatie over de vooraankondiging van de bulletins naar [Vooraankondiging over Microsoft-beveiligingsbulletins](http://technet.microsoft.com/security/bulletin/advance).

Ga naar [de mededelingenservice voor Microsoft-beveiligingsbulletins](http://go.microsoft.com/fwlink/?linkid=21163) voor informatie over hoe u automatisch meldingen ontvangt wanneer Microsoft beveiligingsbulletins uitgeeft.

Op 10 juni 2009 om 11:00 AM Pacific Time (VS en Canada) zal Microsoft op een webcast vragen van gebruikers over deze bulletins beantwoorden. [Schrijf u nu in voor de webcast over de beveiligingsbulletins van juni.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395225) Na deze datum is de webcast op verzoek beschikbaar. Zie [Samenvattingen van de Microsoft-beveiligingsbulletins en webcasts](http://technet.microsoft.com/security/bulletin/summary) voor meer informatie.

Microsoft helpt haar gebruikers bij het vaststellen van het belang voor de maandelijkse beveiligingsupdates van de nieuwste belangrijkste updates die geen verband houden met beveiliging, en die op dezelfde dag als de maandelijkse beveiligingsupdates worden uitgegeven. Zie de sectie **Overige informatie**.

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
<th style="border:1px solid black;" >Software waarin het probleem optreedt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-018">MS09-018</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Active Directory kan externe code worden uitgevoerd (971055)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken opgelost in implementaties van Active Directory op Microsoft Windows 2000 Server en op Windows Server 2003 en Active Directory Application Mode (ADAM) wanneer geïnstalleerd op Windows XP Professional en Windows Server 2003. Door het ernstigste beveiligingslek kan externe code worden uitgevoerd. Een aanvaller die misbruik weet te maken van dit beveiligingslek, kan op afstand volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Met aanbevolen procedures voor firewalls en standaardfirewallconfiguraties kunt u netwerken beveiligen tegen aanvallen die van buiten het bedrijfsnetwerk komen. Het wordt aanbevolen op de systemen die met internet zijn verbonden zo min mogelijk poorten bloot te stellen aan deze aanvallen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-022">MS09-022</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in de Windows-afdrukspooler kan externe code worden uitgevoerd (961501)</strong><br />
<br />
Met deze beveiligingsupdate worden drie privé gemelde beveiligingslekken in de Windows-afdrukspooler opgelost. Door het ernstigste beveiligingslek kan externe code worden uitgevoerd als een server waarin dit probleem optreedt een speciaal ontworpen RPC-aanvraag ontvangt. Met aanbevolen procedures voor firewalls en standaardfirewallconfiguraties kunt u netwerken beveiligen tegen aanvallen die van buiten het bedrijfsnetwerk komen. Het wordt aanbevolen op de systemen die met internet zijn verbonden zo min mogelijk poorten bloot te stellen aan deze aanvallen.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-019">MS09-019</a></td>
<td style="border:1px solid black;"><strong>Cumulatieve beveiligingsupdate voor Internet Explorer (969897)</strong><br />
<br />
Met deze beveiligingsupdate worden zeven privé gemelde beveiligingslekken en een openbaar gemaakt beveiligingslek in Internet Explorer opgelost. In het ergste geval kan er als gevolg van het beveiligingslek externe code worden uitgevoerd als een gebruiker een speciaal ontworpen webpagina weergeeft in Internet Explorer. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-027">MS09-027</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Microsoft Office Word kan externe code worden uitgevoerd (969514)</strong><br />
<br />
Met deze beveiligingsupdate worden twee privé gemelde beveiligingslekken opgelost, waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal vervaardigd Word-bestand opent. Een aanvaller die misbruik weet te maken van deze beveiligingslekken, kan volledige controle krijgen over een systeem waarvoor dit probleem geldt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-021">MS09-021</a></td>
<td style="border:1px solid black;"><strong>Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)</strong><br />
<br />
Met deze beveiligingsupdate worden diverse privé gemelde beveiligingslekken in Microsoft Office Excel opgelost waardoor externe code kan worden uitgevoerd als een gebruiker een speciaal gemaakt Excel-bestand opent dat een verkeerd ingedeeld recordobject bevat. Een aanvaller die de beveiligingslekken weet te misbruiken, kan volledige controle krijgen over een systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-024">MS09-024</a></td>
<td style="border:1px solid black;"><strong>Door een beveiligingslek in de conversieprogramma's van Microsoft Works kan externe code worden uitgevoerd (957632)</strong><br />
<br />
Deze beveiligingsupdate lost een privé gemeld beveiligingslek in de conversieprogramma's van Microsoft Works op. Dit beveiligingslek kan leiden tot het uitvoeren van externe code als een gebruiker een speciaal vervaardigd Works-bestand opent. Een aanvaller die erin slaagt misbruik te maken van dit beveiligingslek, kan dezelfde rechten over het systeem krijgen als de lokale gebruiker. Gebruikers met accounts waarvoor minder gebruikersrechten op het systeem zijn ingesteld, lopen minder risico dan gebruikers die met beheerdersrechten werken.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritiek</a><br />
Uitvoering van externe code mogelijk</td>
<td style="border:1px solid black;">Opnieuw starten mogelijk vereist</td>
<td style="border:1px solid black;">Microsoft Office:</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-026">MS09-026</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in RPC kan leiden tot misbruik van bevoegdheden (970238)</strong><br />
<br />
Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek opgelost op de Windows RPC-locatie waar de RPC Marshalling Engine de interne status niet juist bijwerkt. Een aanvaller kan via dit beveiligingslek willekeurige code uitvoeren en de volledige controle krijgen over een systeem waarin dit probleem optreedt. Ondersteunde edities van Microsoft Windows worden niet geleverd met RPC-servers of -clients waarmee misbruik kan worden gemaakt van dit beveiligingslek. In een standaardconfiguratie kunnen gebruikers niet worden aangevallen door misbruik van dit beveiligingslek. Het beveiligingslek is echter aanwezig in de Microsoft Windows RPC-runtime en kan van invloed zijn op RPC-toepassingen van derden.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-025">MS09-025</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (968537)</strong><br />
<br />
Met deze beveiligingsupdate worden twee openbaar gemaakte en twee privé gemelde beveiligingslekken in de Windows-kernel opgelost die kunnen leiden tot misbruik van bevoegdheden. Een aanvaller die misbruik weet te maken van deze beveiligingslekken, kan willekeurige programmacode uitvoeren en volledige controle krijgen over het systeem waarin dit probleem optreedt. De aanvaller kan vervolgens programma's installeren, gegevens bekijken, wijzigen of wissen, of nieuwe accounts met volledige gebruikersrechten maken. Een aanvaller moet geldige aanmeldingsreferenties hebben en zich lokaal kunnen aanmelden om misbruik te kunnen maken van de beveiligingslekken. De beveiligingslekken kunnen niet vanaf een externe locatie of door anonieme gebruikers worden misbruikt.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-020">MS09-020</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslekken in Internet Information Service (IIS) kunnen leiden tot misbruik van bevoegdheden (970483)</strong><br />
<br />
Met deze beveiligingsupdate wordt een openbaar gemaakt beveiligingslek en een privé gemeld beveiligingslek in Microsoft Internet Information Services (IIS) opgelost. Door de beveiligingslekken kan misbruik van bevoegdheden worden gemaakt als een aanvaller een speciaal ontworpen HTTP-aanvraag verzendt naar een website die verificatie vereist. Deze beveiligingslekken stellen een aanvaller in staat de IIS-configuratie te omzeilen die bepaalt welke soort verificatie is toegestaan, maar niet de controle van de op het bestandssysteem gebaseerde toegangsbeheerlijst (ACL) waarbij wordt gecontroleerd of een bestand voor een gegeven gebruiker toegankelijk is. Misbruik van deze beveiligingslekken zou de aanvaller beperken tot de machtigingen die de bestandssysteem-ACL's aan anonieme gebruikeraccounts toekent.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Belangrijk</a><br />
Misbruik van bevoegdheden</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/security/bulletin/ms09-023">MS09-023</a></td>
<td style="border:1px solid black;"><strong>Beveiligingslek in Windows Search kan leiden tot vrijgeven van informatie (963093)</strong><br />
<br />
Met deze beveiligingsupdate wordt een privé gemeld beveiligingslek in Microsoft Search opgelost. Door het beveiligingslek kan informatie worden vrijgegeven als een gebruiker een zoekopdracht uitvoert waardoor een speciaal ontworpen bestand als het eerste resultaat wordt getoond of als de gebruiker een voorbeeldweergave van een speciaal ontworpen bestand opent in de zoekresultaten. Standaard is Windows Search niet vooraf geïnstalleerd op Windows XP en Windows Server 2003. Dit is een optioneel onderdeel dat kan worden gedownload. In Windows Search geïnstalleerd op ondersteunde edities van Windows Vista en Windows Server 2008 komt dit beveiligingslek niet voor.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Matig</a><br />
Vrijgeven van informatie</td>
<td style="border:1px solid black;">Moet opnieuw worden opgestart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Exploitatie-index  
-----------------
  
<span></span>
In de volgende tabel vindt u een beoordeling van de mate van misbruik van elk beveiligingslek dat deze maand wordt opgelost. De beveiligingslekken worden vermeld volgens bulletin-id en CVE-id.
  
**Gebruik van deze tabel**
  
Raadpleeg deze tabel voor informatie over de kans dat binnen 30 dagen na publicatie van beveiligingsbulletins functionerende exploitatiecode verschijnt voor elk van de beveiligingsupdates die u misschien moet installeren. Bekijk deze beoordelingen overeenkomstig de configuratie van uw computer(s) om de ernst van het probleem te kunnen vaststellen. Zie de [exploitatie-index van Microsoft](http://technet.microsoft.com/en-us/security/cc998259.aspx) voor meer informatie over de betekenis van deze prioriteitsniveaus en hoe die worden vastgesteld.
  
| Bulletin-id                                                         | Titel bulletin                                                                                                      | CVE-id                                                                           | Beoordeling van de exploitatie-index                                                                                 | Belangrijke opmerkingen                                                                                                                                                                                                                                                                               |  
|---------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-018](http://technet.microsoft.com/security/bulletin/ms09-018) | Beveiligingslekken in Active Directory kunnen leiden tot uitvoering van externe code (971055)                       | [CVE-2009-1138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1138) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Op Windows 2000-servers waarop de LDAP-service (standaard tcp/389) voor het netwerk open staat, kan externe code worden uitgevoerd.                                                                                                                                                                   |  
| [MS09-018](http://technet.microsoft.com/security/bulletin/ms09-018) | Beveiligingslekken in Active Directory kunnen leiden tot uitvoering van externe code (971055)                       | [CVE-2009-1139](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1139) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Het gevolg van dit beveiligingslek op de beveiliging is een geheugenlek dat uiteindelijk tot denial of service kan leiden. Uitvoering van code is echter niet mogelijk.                                                                                                                               |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2007-3091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2007-3091) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1140](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1140) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit is een beveiligingslek waarmee toegang tot interdomeingegevens kan worden verkregen en als gevolg waarvan informatie wordt vrijgegeven maar geen code wordt uitgevoerd.                                                                                                                           |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1141](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1141) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1528) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1529) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1531) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-019](http://technet.microsoft.com/security/bulletin/ms09-019) | Cumulatieve beveiligingsupdate voor Internet Explorer (969897)                                                      | [CVE-2009-1532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1532) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-020](http://technet.microsoft.com/security/bulletin/ms09-020) | Beveiligingslekken in Internet Information Service (IIS) kunnen leiden tot misbruik van bevoegdheden (970483)       | [CVE-2009-1122](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1122) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Geringe kans dat er code wordt uitgevoerd, maar een grote kans dat er informatie wordt vrijgegeven omdat de verificatie kan worden omzeild.                                                                                                                                                           |  
| [MS09-020](http://technet.microsoft.com/security/bulletin/ms09-020) | Beveiligingslekken in Internet Information Service (IIS) kunnen leiden tot misbruik van bevoegdheden (970483)       | [CVE-2009-1535](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1535) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Openbare code is beschikbaar voor het vrijgeven van informatie.                                                                                                                                                                                                                                       |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0549) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0559) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Alleen in Office 2000 zou er code kunnen worden uitgevoerd. Aanvallen op latere versies van Office leiden doorgaans niet tot het uitvoeren van code.                                                                                                                                                  |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0560) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-0561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0561) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-021](http://technet.microsoft.com/security/bulletin/ms09-021) | Door beveiligingslekken in Microsoft Office Excel kan externe code worden uitgevoerd (969462)                       | [CVE-2009-1134](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1134) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-022](http://technet.microsoft.com/security/bulletin/ms09-022) | Door beveiligingslekken in de Windows-afdrukspooler kan externe code worden uitgevoerd (961501)                     | [CVE-2009-0228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-022](http://technet.microsoft.com/security/bulletin/ms09-022) | Door beveiligingslekken in de Windows-afdrukspooler kan externe code worden uitgevoerd (961501)                     | [CVE-2009-0229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | Dit is een beveiligingslek waardoor informatie kan worden vrijgegeven maar waarmee geen code kan worden uitgevoerd.                                                                                                                                                                                   |  
| [MS09-022](http://technet.microsoft.com/security/bulletin/ms09-022) | Door beveiligingslekken in de Windows-afdrukspooler kan externe code worden uitgevoerd (961501)                     | [CVE-2009-0230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0230) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-023](http://technet.microsoft.com/security/bulletin/ms09-023) | Beveiligingslek in Windows Search kan leiden tot vrijgeven van informatie (963093)                                  | [CVE-2009-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0239) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Kans op werkende exploitatiecode is gering      | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-024](http://technet.microsoft.com/security/bulletin/ms09-024) | Door een beveiligingslek in de conversieprogramma's van Microsoft Works kan externe code worden uitgevoerd (957632) | [CVE-2009-1533](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1533) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-025](http://technet.microsoft.com/security/bulletin/ms09-025) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (968537)                        | [CVE-2009-1123](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1123) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-025](http://technet.microsoft.com/security/bulletin/ms09-025) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (968537)                        | [CVE-2009-1124](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1124) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-025](http://technet.microsoft.com/security/bulletin/ms09-025) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (968537)                        | [CVE-2009-1125](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1125) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-025](http://technet.microsoft.com/security/bulletin/ms09-025) | Beveiligingslekken in de Windows-kernel kunnen leiden tot misbruik van bevoegdheden (968537)                        | [CVE-2009-1126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1126) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | Consistente exploitatiecode is het meest waarschijnlijk voor Windows 2000. De kans dat er code wordt uitgevoerd via een beveiligingslek met betrekking tot stackbufferoverloop, is dankzij de /GS-bescherming kleiner geworden in Windows XP en Windows Server 2003.                                  |  
| [MS09-026](http://technet.microsoft.com/security/bulletin/ms09-026) | Beveiligingslek in RPC kan leiden tot misbruik van bevoegdheden (970238)                                            | [CVE-2009-0568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0568) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | Dit beveiligingslek heeft geen rechtstreekse gevolgen voor Microsoft-software. Werkstations waarop RPC-services van onafhankelijke softwareleveranciers worden uitgevoerd, kunnen echter wel kwetsbaar zijn voor het uitvoeren van externe code als deze beveiligingsupdate niet wordt geïnstalleerd. |  
| [MS09-027](http://technet.microsoft.com/security/bulletin/ms09-027) | Door beveiligingslekken in Microsoft Office Word kan externe code worden uitgevoerd (969514)                        | [CVE-2009-0563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0563) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Inconsistente exploitatiecode is waarschijnlijk | (Geen)                                                                                                                                                                                                                                                                                                |  
| [MS09-027](http://technet.microsoft.com/security/bulletin/ms09-027) | Door beveiligingslekken in Microsoft Office Word kan externe code worden uitgevoerd (969514)                        | [CVE-2009-0565](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0565) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Consistente exploitatiecode is waarschijnlijk   | (Geen)                                                                                                                                                                                                                                                                                                |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="8">
Microsoft Windows 2000:  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://technet.microsoft.com/security/bulletin/ms09-018)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://technet.microsoft.com/security/bulletin/ms09-022)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://technet.microsoft.com/security/bulletin/ms09-019)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://technet.microsoft.com/security/bulletin/ms09-026)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://technet.microsoft.com/security/bulletin/ms09-025)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://technet.microsoft.com/security/bulletin/ms09-020)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://technet.microsoft.com/security/bulletin/ms09-023)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Active Directory op Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bba6e20a-0345-46ae-a6f1-fd27fdee7c21)  
(KB969805)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=86378753-db24-44c2-a27d-cc0239f40ab8)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d645ad82-13c3-4030-808b-834e86ed3298)  
(Kritiek)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe8b3796-a407-4f41-89eb-35b4bcc24ff6)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=155a79c1-e5e4-4f62-b4b0-53aca59f20ac)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=79b0481d-a3d7-477b-928a-a98cc79374af)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=8515a294-4f25-4dc5-860a-e7ad9b6c1c01)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="8">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://technet.microsoft.com/security/bulletin/ms09-018)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://technet.microsoft.com/security/bulletin/ms09-022)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://technet.microsoft.com/security/bulletin/ms09-019)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://technet.microsoft.com/security/bulletin/ms09-026)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://technet.microsoft.com/security/bulletin/ms09-025)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://technet.microsoft.com/security/bulletin/ms09-020)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://technet.microsoft.com/security/bulletin/ms09-023)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 en Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM) op Windows XP Professional Service Pack 2 en Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cb2c9b76-0c65-4754-9941-d45a7c74a29a)  
(KB970437)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f2119aca-a98e-4810-be52-f38241443baf)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3d7f63ee-d7c3-48a5-902e-60625405e97d)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=827b735c-660b-4723-b688-3297e107153a)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d9e27ce1-4e7c-437f-9477-e7805a33da08)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f033fa78-c451-44f8-aa6c-a49622c37f40)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 en Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6349e046-a3f8-4ae5-b8c3-c9879cc99e8f)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services (IIS) 5.1 op Windows XP Professional Service Pack 2 en Windows XP Professional Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=97da589f-4534-42f6-9f29-967b5a33c542)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=759f22cb-ea7f-49dd-a200-19cb83fffd8d)  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=2ef3aaf0-a2a9-4c17-99ab-a0dc3d3f7e86)  
(KB970437)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22699d09-1e68-456a-8733-bfad6667ebf5)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=088f70eb-c5c5-426a-880a-18ed386d0b56)  
(Kritiek)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e5d2c81e-ffab-4e3b-a59a-a55000597213)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a24aedf0-7a31-4ee8-a9a6-998f1160c700)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=20734b70-37f1-47dd-bc09-d56f93577a55)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3769800e-af93-4a44-8a1e-b30cc54b226f)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8982e6d2-e1f7-4208-88e3-80b159a8e21a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=50c56dd6-c34d-4632-a779-8bcf8fdb341b)  
(Gemiddeld)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://technet.microsoft.com/security/bulletin/ms09-018)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://technet.microsoft.com/security/bulletin/ms09-022)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://technet.microsoft.com/security/bulletin/ms09-019)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://technet.microsoft.com/security/bulletin/ms09-026)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://technet.microsoft.com/security/bulletin/ms09-025)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://technet.microsoft.com/security/bulletin/ms09-020)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://technet.microsoft.com/security/bulletin/ms09-023)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=d814ce65-a193-4027-a6cd-106d388830a6)   
(KB969805)  
(Belangrijk)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f6f99957-f74f-4446-8734-a468283eebae)   
(KB970437)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=865414f8-3f77-4fee-acc6-6684a3dc0aa4)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=72a23752-86fb-4cc9-ab8e-63ffdfae5bec)  
(Gemiddeld)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a980b867-c67f-4c61-b6db-e55c2ca68dc0)  
(Gemiddeld)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=298143f2-f37a-4a2c-86ac-9804d4ff1dad)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62bb9e22-4f4b-4ffc-ba76-f626e94c79d5)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9356404c-d89a-4de0-b9b4-f6e1bdadf745)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=2bd4e410-dbd8-431a-b316-e1e2f1825c3a)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=e72ef31f-5161-4fe6-8ed3-6206e02cef31)  
(Gemiddeld)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=0d1f23c8-06eb-4996-92eb-0eb635fd6a42)  
(KB969805)  
(Belangrijk)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1a2badc7-c0a5-4032-a009-73ebe9d76313)  
(KB970437)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=197a6cc7-4ba3-4d2e-b621-0ef3da645ef2)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a03d3c4-e39d-43a3-8d42-216e9551be96)  
(Gemiddeld)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e7d6372-9c8c-449d-88fd-afd4f92ad9e6)  
(Gemiddeld)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4a5401d7-ca97-4734-a0e9-d7ffe0777e34)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=888b8dd8-d76c-42f5-a377-1f1750d3cf56)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a3123af-173d-49eb-9997-14e82e764aee)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=ea363223-535d-4142-9aba-3890960c6259)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ffc3680-f9bf-423b-96a7-102f4cc9c240)  
(Gemiddeld)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 met SP2 voor Itanium-systemen
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=92e7808b-92ff-449d-bb73-ee8638e9ccd1)  
(KB969805)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=719efd62-fb33-447d-b6dd-2aaafbbad881)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=58efde2c-e0b8-4259-b19e-80564b834882)  
(Gemiddeld)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a2d2907e-67ae-44a4-a805-8670e659ea57)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=3084f46e-02b9-4d99-a7a1-033817f9bd9f)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 met SP2 voor Itanium-systemen](http://www.microsoft.com/downloads/details.aspx?familyid=13b50993-410f-4e7a-a33a-6d9b48dbb4d1)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e6b806eb-e2c4-4436-8964-720db593055d)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://technet.microsoft.com/security/bulletin/ms09-018)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://technet.microsoft.com/security/bulletin/ms09-022)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://technet.microsoft.com/security/bulletin/ms09-019)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://technet.microsoft.com/security/bulletin/ms09-026)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://technet.microsoft.com/security/bulletin/ms09-025)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://technet.microsoft.com/security/bulletin/ms09-020)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://technet.microsoft.com/security/bulletin/ms09-023)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ad8f037-2434-4dea-bfc3-9d3b4008b828)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e60215c3-b8b9-4e45-9d9f-b3fb0b47cce1)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6f2730e9-b4fc-4f20-96cf-73f1be63f374)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ca227c0-f2dd-429c-a542-e08e93527214)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 en Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c31b36f8-330c-4a0c-9a3d-7cbe9a1ab8c8)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85c317cd-2a14-4747-9f50-3af3ddd3ae1b)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88185088-8c2c-4bc6-89b2-87f4d4849cf7)  
(Kritiek)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5edb14f7-11ec-4180-9f0f-b2673f1c8d83)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=188adafe-1feb-46ad-b237-a88d35104dcd)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 en Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d70a65f-07ce-4992-8bec-28fefd7587bc)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://technet.microsoft.com/security/bulletin/ms09-018)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://technet.microsoft.com/security/bulletin/ms09-022)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://technet.microsoft.com/security/bulletin/ms09-019)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://technet.microsoft.com/security/bulletin/ms09-026)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://technet.microsoft.com/security/bulletin/ms09-025)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://technet.microsoft.com/security/bulletin/ms09-020)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://technet.microsoft.com/security/bulletin/ms09-023)
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
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Gemiddeld**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f18356d-9f09-4d24-8361-970c0d1ccac4)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a0e3f975-57da-43fa-ac12-3d14fd6ce939)\*\*  
(Gemiddeld)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=aaad301c-d232-4733-a0df-8e5d41bbfde8)\*\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaa26c6c-5bf7-4099-bb21-1e03de3a25ca)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor 32-bits systemen en Windows Server 2008 voor 32-bits systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98ba52b2-da1a-4939-a10e-d43b3a7e7ed4)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0a6e8d-a31d-4f3d-a7d7-e61215bfebed)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=758edce7-2a82-4b2e-bd71-5b7075cc4b17)\*\*  
(Gemiddeld)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=faac92d4-4a2b-4bb5-8bd1-1519a9fa8147)\*\*  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=447aaa4f-946b-4f23-b151-dcf46ea9f80e)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor x64-systemen en Windows Server 2008 voor x64-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbaa5a72-c267-4907-a207-525c2803d7b9)\*  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bbac3deb-6c93-45aa-832c-02b915ac7f44)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=67d4c189-030d-42eb-98b9-7957ccd92592)  
(Gemiddeld)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f33012b9-5d5b-4f72-8d49-a8e1c8bc1337)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 voor Itanium-systemen en Windows Server 2008 voor Itanium-systemen Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0e3ad56-a363-44ba-af4d-b7f551c88afd)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
</table>
 
**Opmerkingen voor Windows Server 2008**

**\*Windows Server 2008 Server Core-installatie is getroffen.** Voor ondersteunde edities van Windows Server 2008 is deze update van toepassing met hetzelfde prioriteitsniveau, ongeacht of Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 Server Core-installatie is niet getroffen.** De beveiligingslekken die in deze update worden beschreven, hebben geen invloed op ondersteunde edities van Windows Server 2008 als Windows Server 2008 is geïnstalleerd met behulp van de Server Core-installatieoptie. Zie [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) voor meer informatie over deze installatieoptie. De Server Core-installatieoptie kan niet worden toegepast op bepaalde edities van Windows Server 2008. Zie hiervoor [Server Core-installatieopties vergelijken](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Office-pakketen en -software

 
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
Microsoft Office-pakketten, -systemen en -onderdelen
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://technet.microsoft.com/security/bulletin/ms09-027)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://technet.microsoft.com/security/bulletin/ms09-021)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://technet.microsoft.com/security/bulletin/ms09-024)
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
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritiek**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3663e9f2-a952-4238-b902-90b5b09feb38)  
(KB969600)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd16e243-b8e2-4afb-86b6-4d60214598eb)  
(KB969683)  
(Kritiek)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf95806-3d32-411b-9779-a81aebad45e9)  
(KB957838)  
(Kritiek)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1323be1-15f2-491b-abae-c03ba1394398)  
(KB969602)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd80ce95-0aec-4493-b9d1-c3dad95c3415)  
(KB969680)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0ba8c9e-75ee-46bd-9e92-d4e6599309ad)  
(KB957646)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cbc2587-2c8c-49b4-9f40-e4cdccb61ecd)  
(KB969603)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=10156044-a5a4-4312-98a7-1b1ced625ddb)  
(KB969681)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3 met het bestandsconversieprogramma van Microsoft Works 6–9](http://www.microsoft.com/downloads/details.aspx?familyid=a7ba3ea7-d06a-4c14-9107-9b92ef68fcae)\*\*\*  
(KB968326)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office System Service Pack 1 en 2007 Microsoft Office System Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1 en Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e205108-4c28-4cab-a4d0-4ed3fd696473)  
(KB969604)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 en Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2bcd565a-6acb-407d-80da-0398526ddf99)\*  
(KB969682)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bd47e1e5-cd2e-4c08-9864-471e97f38ca3)  
(KB969559)  
(Belangrijk)
</td>
</tr>
<tr>
<th colspan="4">
Microsoft Office voor Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://technet.microsoft.com/security/bulletin/ms09-027)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://technet.microsoft.com/security/bulletin/ms09-021)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://technet.microsoft.com/security/bulletin/ms09-024)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Prioriteitsniveau**
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Belangrijk**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Geen
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 voor Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 voor Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Conversieprogramma voor Open XML-bestandsindeling voor Mac
</td>
<td style="border:1px solid black;">
[Conversieprogramma voor Open XML-bestandsindeling voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Conversieprogramma voor Open XML-bestandsindeling voor Mac](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<th colspan="4">
Overige Office-software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bulletin-id**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://technet.microsoft.com/security/bulletin/ms09-027)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://technet.microsoft.com/security/bulletin/ms09-021)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://technet.microsoft.com/security/bulletin/ms09-024)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Prioriteitsniveau**
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
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20e6933d-85f8-4cec-9534-893789cd053e)  
(KB969685)  
(Belangrijk)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=ac0530dc-7f63-4ad0-85c1-784ad28156cf)  
(KB969686)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Belangrijk)  
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 en Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63bd8f14-e736-46ce-af66-d30f17461e5a)  
(KB969613)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
[Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 en Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2)  
(KB969679)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Belangrijk)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Belangrijk)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 en Microsoft Office SharePoint Server 2007 Service Pack 2 (32-bits edities)](http://www.microsoft.com/downloads/details.aspx?familyid=862e6ad1-8124-4060-93b1-2b882ef5ce3d)\*\*  
(KB969737)  
(Belangrijk)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 en Microsoft Office SharePoint Server 2007 Service Pack 2 (64-bits edities)](http://www.microsoft.com/downloads/details.aspx?familyid=b7b6e611-2c5d-4639-add9-972055789ecd)\*\*  
(KB969737)  
(Belangrijk)
</td>
<td style="border:1px solid black;">
Niet van toepassing
</td>
</tr>
</table>
 
**Opmerkingen voor MS09-021**

\*Behalve beveiligingsupdatepakket KB969682 moet ook voor Microsoft Office Excel 2007 Service Pack 1 en Microsoft Office Excel 2007 Service Pack 2 de beveiligingsupdate voor [Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 1 en Microsoft Office-compatibiliteitspakket voor de bestandsindelingen van Word, Excel en PowerPoint 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2) (KB969679) worden geïnstalleerd om beschermd te zijn tegen de beveiligingslekken die in dit bulletin worden beschreven.

\*Deze update geldt voor servers waarop Excel Services is geïnstalleerd, zoals de standaardconfiguratie van Microsoft Office SharePoint Server 2007 Enterprise en Microsoft Office SharePoint Server 2007 voor internetsites. Microsoft Office SharePoint Server 2007 Standard wordt zonder Excel Services geleverd.

**Opmerking voor MS09-024**

\*\*\*Microsoft Office Word 2003 wordt getroffen als een kwetsbaar Works-conversieprogramma is geïnstalleerd. Works-conversieprogramma's zijn verkrijgbaar voor Microsoft Office Word 2003 als een download via het [bestandsconversieprogramma voor Microsoft Works 6–9](http://www.microsoft.com/downloads/details.aspx?familyid=bf41401e-70fa-465d-ae2e-cf44dbf05297&displaylang=en).

Hulpmiddelen en richtlijnen voor detecteren en implementeren
------------------------------------------------------------

<span></span>
**Beveiligingscentrum**

De software- en beveiligingsupdate beheren waarmee u de servers, desktops en draagbare computers binnen uw organisatie kunt implementeren. Zie het [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903) voor meer informatie. Op de website [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171) staat aanvullende informatie over beveiliging in Microsoft-producten. Consumenten kunnen op de website [Beveiliging thuis](http://go.microsoft.com/fwlink/?linkid=85102) deze informatie ook ophalen door te klikken op "De nieuwste beveiligingsupdates".

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

Voor informatie over andere releases voor Windows Update en Microsoft Update (geen beveiligingsreleases), verwijzen wij u naar:

-   [Microsoft Knowledge Base-artikel 894199](http://support.microsoft.com/kb/894199): Beschrijving van wijzigingen in de inhoud van Software Update Services en Windows Server Update Services. Heeft betrekking op alle Windows-inhoud.
-   [Nieuwe, herziene en vrijgegeven updates voor Microsoft-producten behalve Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Om de beveiliging voor klanten te verbeteren, verstrekt Microsoft bij elke maandelijkse uitgifte van beveiligingsupdates informatie over beveiligingslekken aan de grote producenten van beveiligingsprogramma's. Deze producenten kunnen dan die informatie over beveiligingslekken gebruiken om hun klanten een betere beveiliging te bieden door hun software of apparatuur aan te passen, zoals antivirusprogramma's, inbraakdetectiesystemen voor netwerken of inbraakpreventiesystemen voor hosts. Op de websites van de programmapartners (zie [Microsoft Active Protections Program (MAPP)-partners](http://www.microsoft.com/security/msrc/mapp/partners.mspx)) kunt u nagaan of de leveranciers van beveiligingsprogramma's hun producten steeds aanpassen.

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

-   Joshua J. Drake van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-018
-   Justin Wyatt van het [Beaverton School District](http://www.beaverton.k12.or.us/home/) voor het melden van een probleem dat wordt beschreven in MS09-018
-   David Bloom van [Google Inc.](http://www.google.com/) voor de samenwerking bij het oplossen van een probleem dat wordt beschreven in MS09-019
-   Jorge Luis Alvarez Medina van [Core Security Technologies](http://www.coresecurity.com/) voor het melden van een probleem dat wordt beschreven in MS09-019
-   Haifei Li van [Fortinet](http://www.fortinet.com/) voor het melden van een probleem dat wordt beschreven in MS09-019
-   [Tippingpoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS09-019
-   Peter Vreugdenhil, die bij [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) werkt, voor het melden van een probleem dat wordt beschreven in MS09-019
-   Wushi, die bij [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) werkt, voor het melden van twee problemen die worden beschreven in MS09-019
-   Nils, die bij [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) werkt, voor het melden van een probleem dat wordt beschreven in MS09-019
-   Yamata Li van [Palo Alto Networks](http://www.paloaltonetworks.com/) voor het melden van een probleem dat wordt beschreven in MS09-020
-   Bing Liu van [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) van Fortinet voor het melden van drie problemen die worden beschreven in MS09-021
-   Carsten H. Eiram van [Secunia](http://secunia.com/) voor het melden van twee problemen die worden beschreven in MS09-021
-   [TELUS Security Labs Vulnerability Research Team](http://telussecuritylabs.com/) voor het melden van een probleem dat wordt beschreven in MS09-021
-   Sean Larsson en Joshua Drake van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-021
-   [TippingPoint](http://www.tippingpoint.com/) en [Zero Day Initiative](http://www.zerodayinitiative.com/) voor het melden van een probleem dat wordt beschreven in MS09-021
-   Jun Mao van [VeriSign iDefense Labs](http://labs.idefense.com/) voor het melden van een probleem dat wordt beschreven in MS09-022
-   Yair Amit van [IBM Rational Application Security](http://blog.watchfire.com/) voor het melden van een probleem dat wordt beschreven in MS09-023
-   Shaun Colley van [NGS Software](http://www.ngssoftware.com/) voor het melden van een probleem dat wordt beschreven in MS09-024
-   Thomas Garnier voor het melden van twee problemen die worden beschreven in MS09-025
-   Wushi van [team509](http://www.team509.com/), die samenwerkt met [Zero Day Initiative](http://www.zerodayinitiative.com/), voor het melden van een probleem dat wordt beschreven in MS09-027
-   Nicolas Joly van [VUPEN Security](http://www.vupen.com/) voor het melden van een probleem dat wordt beschreven in MS09-027

#### Ondersteuning

-   De software waarin het probleem optreedt, is getest om te controleren of het probleem bij deze versies optreedt. Andere versies hebben het einde van hun ondersteuningscyclus bereikt. Ga naar [Microsoft Support Lifecycle](http://go.microsoft.com/fwlink/?linkid=21742) om de ondersteuningscyclus voor uw softwareversie te bepalen.
-   Technische ondersteuning van [Security Support](http://support.microsoft.com/?ln=nl) is beschikbaar via 020-500 1005. Voor ondersteuningsverzoeken in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Zie [Hulp en ondersteuning van Microsoft](http://support.microsoft.com/?ln=nl) voor meer informatie over de beschikbare ondersteuningsopties.
-   Voor internationale klanten is ondersteuning verkrijgbaar bij de Microsoft-vestiging in hun land. Voor ondersteuning in verband met beveiligingsupdates worden geen kosten in rekening gebracht. Ga naar de [website voor internationale ondersteuning](http://go.microsoft.com/fwlink/?linkid=21155) voor meer informatie over hoe u contact kunt opnemen met Microsoft voor ondersteuning.

#### Uitsluiting van aansprakelijkheid

De informatie die wordt geboden in de Microsoft Knowledge Base, wordt geleverd 'in de huidige staat' zonder enige garantie. Microsoft wijst hierbij alle expliciete of impliciete garanties van de hand, met inbegrip van alle garanties betreffende de verhandelbaarheid en geschiktheid voor een bepaald doel. Voorzover maximaal is toegestaan op grond van toepasselijk recht zijn Microsoft Corporation en/of haar leveranciers in geen geval aansprakelijk voor enige directe, indirecte of incidentele schade, bijzondere schade, gevolgschade of schade ten gevolge van het verlies van winsten, zelfs als Microsoft Corporation of haar leveranciers van de mogelijkheid van dergelijke schade op de hoogte is gesteld. Aangezien sommige staten/rechtssystemen uitsluiting of beperking van aansprakelijkheid voor gevolgschade of incidentele schade niet toestaan, is de voorgaande beperking wellicht niet op u van toepassing.

#### Revisies

-   V1.0 (9 juni 2009): Samenvatting van de gepubliceerde bulletins.

*Built at 2014-04-18T01:50:00Z-07:00*
