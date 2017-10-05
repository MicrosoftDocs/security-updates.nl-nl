---
TOCTitle: Compliantieproblemen van FIPS voor RMS
Title: Compliantieproblemen van FIPS voor RMS
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18113986
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747551(v=WS.10)'
---

Compliantieproblemen van FIPS voor RMS
======================================

Rights Management Services (RMS) versie 1.0 Service Pack 1 (SP1) is ontworpen voor organisaties die de door FIPS geëvalueerde cryptografische functionaliteit moeten gebruiken.

Federal Information Processing Standard 140-1 (FIPS 140-1) en de opvolger FIPS 140-2 zijn normen van de Amerikaanse overheid die een benchmark bieden voor het implementeren van cryptografische software. Deze normen geven aanbevolen richtlijnen voor het implementeren van cryptografische algoritmen, het verwerken van belangrijk materiaal en gegevensbuffers en het gebruik van het besturingssysteem.

RMS kan worden geïmplementeerd als onderdeel van een met FIPS compatibel systeem voor het beveiligen van vertrouwelijke gegevens.

-   De door FIPS geëvalueerde cryptografieproviders beperken de functionaliteit tot: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. Door deze beperking wordt de beveiligingskanaalprovider gedwongen alleen over het krachtigere Transport Layer Security (TLS) 1.0-protocol te onderhandelen. Misschien moet Internet Explorer voor ondersteuning van TLS worden geconfigureerd, maar veel webservers van derden ondersteunen TLS niet. Zie artikel 811834 in de Knowledge Base op de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=43614) voor meer informatie over dit onderwerp.

Beveilig de persoonlijke sleutel van RMS met een van de twee standaard cryptografieproviders van Microsoft (CSP's) als u een softwarematige persoonlijke sleutel voor de beveiliging gaat gebruiken. Deze cryptografieproviders hebben het evaluatieproces FIPS 140-1 of FIPS 140-2 (afhankelijk van welke toepassing is) van de Amerikaanse overheid uitgevoerd. Alhoewel het niet is vereist, wordt klanten die veel waarde hechten aan beveiliging, aangeraden hardwarebeveiligingsmodules (zoals van nCipher of IBM) te gebruiken voor het hoogste beveiligingsniveau van persoonlijke sleutels van de RMS-server. Als hardwarebeveiligingsmodules worden gebruikt, moet de juiste CSP worden geselecteerd om de hardwarebeveiligingsmodule te kunnen gebruiken. Hiervoor moet het systeem waarschijnlijk opnieuw worden opgestart. Zie Knowledge Base-artikel 830690 op de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=44138) voor meer informatie over dit onderwerp.

Wanneer u uw RMS-systeem gaat implementeren, moet u de volgende keuzen maken:

-   Volg de NSA-richtlijnen voor met FIPS compatibele cryptografie in Windows.
-   Schakel Lokaal beveiligingsbeleid voor met FIPS compatibele cryptografie in.
-   Implementeer RMS SP1-clients en -servers in de bovenstaande omgeving.
-   Schakel het TLS-protocol (Transport Layer Security) in Internet Information Services op de RMS-server in.
-   Schakel in Internet Explorer het TLS-protocol (Transport Layer Security) voor de clients in.
-   Schakel het SQL TDS-protocol (Tabular Data Stream) in dat wordt gebruikt bij de Windows TLS/SSL-beveiligingsprovider tussen SQL-clients en SQL Server op de databaseserver.
-   Configureer SQL voor TSL/SSL
