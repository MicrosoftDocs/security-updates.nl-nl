---
TOCTitle: 'De RMS-client distribueren'
Title: 'De RMS-client distribueren'
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18113913
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720266(v=WS.10)'
---

De RMS-client distribueren
==========================

De RMS-client vormt een onderdeel van het Windows Vista®-besturingssysteem. De RMS-client kan niet langer meer afzonderlijk worden geiïnstalleerd. Voor besturingssystemen die vóór Windows Vista op de markt zijn gebracht, dient u de RMS-clientsoftware te installeren en vervolgens te activeren.

Bij het activeringsproces worden een lockbox en een computercertificaat voor de aangemelde gebruiker ingesteld. De activering wordt lokaal uitgevoerd. Daarvoor is dus geen netwerkverbinding nodig. Nadat RMS is geactiveerd, wordt bij het eerste verzoek om een gebruikerslicentie door een RMS-toepassing er een gebruikerscertificaat voor de gebruiker gemaakt. De RMS-client kan op elke clientcomputer in de organisatie met behulp van Groepsbeleid, Windows Update of een beheerscript worden geïnstalleerd.

| ![](/security-updates/images/Cc720266.note(WS.10).gif)Opmerking                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ongeacht de methode waarmee de client is gedistribueerd, gebruikt de RMS-client een poort (standaard is dit poort 80 of poort 443) voor communicatie met de RMS-server. U moet controleren of de clientcomputer via deze poorten aanvragen naar de RMS-basis- en licentieclusters kan verzenden. |

**Groepbeleid gebruiken**

Als binnen uw organisatie software via Groepsbeleid wordt gedistribueerd, kunt u deze methode ook gebruiken om met uitgebreide machtigingen de RMS-client te distribueren. Wordt de RMS-client op deze manier gedistribueerd, dan heeft de gebruiker geen beheerdersbevoegdheden nodig en kan de RMS-client worden geïnstalleerd via **Software** in het **Configuratiescherm** of door inhoud die door rechten wordt beveiligd, in een toepassing met RMS-ondersteuning te openen.

**Windows Update gebruiken**

Windows Update is de eenvoudigste manier om de RMS-client op een computer te installeren. Het voordeel van deze methode is dat een mechanisme wordt gebruikt waarmee gebruikers bekend zijn. Dit vereist echter wel dat de gebruiker die de RMS-client installeert over lokale beheerdersrechten op de computer moet beschikken.

**Installeren met een script**

Als u de clientinstallatie zoveel mogelijk wilt beheren, kunt u de software ophalen en vervolgens een script uitvoeren om de integriteit van de software bij elke stap van het installatieproces te controleren. Dit script kan worden geschreven en toegevoegd aan een groepsbeleidsobject als een opstartscript. Met deze methode hoeft de gebruiker geen lokale systeembeheerder op de computer te zijn en wordt de RMS-client automatisch geïnstalleerd na het opnieuw opstarten.

Hier ziet u een voorbeeld van een script:

`Set objShell = Wscript.CreateObject("Wscript.Shell")`  
`objShell.run "WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q"`  

Zie [SMS of Groepsbeleid instellen voor de implementatie van clients](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) verderop in dit onderwerp voor informatie over het distribueren van de RMS-client met behulp van Groepsbeleid.

Zie [Procedures voor het implementeren van de RMS-client](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) verderop in dit onderwerp voor procedures voor het implementeren van de RMS-client.
