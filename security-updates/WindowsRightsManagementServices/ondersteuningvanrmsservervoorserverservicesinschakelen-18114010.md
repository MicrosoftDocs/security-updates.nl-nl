---
TOCTitle: 'Ondersteuning van RMS-server voor serverservices inschakelen'
Title: 'Ondersteuning van RMS-server voor serverservices inschakelen'
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18114010
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747593(v=WS.10)'
---

Ondersteuning van RMS-server voor serverservices inschakelen
============================================================

RMS kan ook rechtenaccountcertificaten en gebruikslicenties leveren aan servertoepassingen met RMS-ondersteuning. Er zijn enkele zaken waarvan u zich bewust moet zijn bij het configureren van serverservices:

-   Voor DACL's (Discretionary Access Control Lists) op de RMS-pipelines worden standaard de veiligste instellingen gebruikt. Wanneer u RMS-serverservices gebruikt, moet u de DACL wijzigen.
-   Als de RMS-client is geïnstalleerd op een Windows Server 2003-server en de verbeterde beveiliging van Internet Explorer wordt ingeschakeld, moet u de RMS-cluster-URL toevoegen aan de Zone Vertrouwde websites van Internet Explorer.
-   Vele serverservices maken gebruik van de geavanceerde functionaliteit van de Active Directory-services die alleen beschikbaar is als op alle Active Directory-domeincontrollers Windows Server 2003 wordt uitgevoerd. Als u met bepaalde serverservices werkt (zoals Microsoft Office SharePoint Server 2007 of Microsoft Exchange Server 2007), wordt aanbevolen dat op alle domeincontrollers Windows Server 2003 wordt uitgevoerd en dat de functionele domein- en forestniveaus van Active Directory zich op het niveau van Windows Server 2003 bevinden.

Standaard-DACL (Discretionary Access Control List) op servercertificeringspipeline
----------------------------------------------------------------------------------

Toepassingen zoals Microsoft Office SharePoint Server 2007 of Microsoft Exchange Server 2007 zijn voorzien van RMS-ondersteuning zodat namens gebruikers gebruikslicenties kunnen worden aangevraagd. In een standaard-RMS-installatie is de DACL van de RMS-servercertificeringspipeline beperkt. Dit houdt in dat door een toepassing geen certificaten en licenties voor de gebruikers van die toepassing kunnen worden bemachtigd. Als u voor deze computers echter een toepassing met RMS-ondersteuning hebt, kunt u deze computers wel in staat stellen deel te nemen aan uw RMS-systeem door de DACL's op de RMS-servercertificeringspipeline te configureren.

Servertoepassingen met RMS-ondersteuning kunnen met behulp van het bestand ServerCertification.asmx met de RMS-certificeringsservice worden verbonden.

Wanneer RMS deze bestanden maakt, worden de DACL's van de bestanden zodanig ingesteld dat ze alleen via systeemprocessen toegang bieden. Het wordt aanbevolen dat u een Active Directory -beveiligingsgroep voor serverservices maakt en deze groep vervolgens vult met de Active Directory-objecten van de computers die namens hun gebruikers gebruikslicenties aanvragen.

Nadat u de groep hebt gemaakt, kunt u de DACL voor het bestand ServerCertification.asmx aanpassen zodat de groep over de machtiging Lezen & Uitvoeren voor deze service beschikt. Ook moet u de RMS-servicegroep aan de DACL toevoegen met de machtiging Lezen & Uitvoeren.

| ![](/security-updates/images/Cc747593.note(WS.10).gif)Opmerking                                                                                    |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als zich meerdere RMS-servers in het cluster bevinden, moet de DACL voor het bestand ServerCertification.asmx op elke server in het cluster worden aangepast. |

Voor Microsoft Exchange Server 2007 moet het Active Directory-computerobject van elke Exchange-bruggenhoofdserver aan de serverservicesgroep worden toegevoegd. Als u dit niet doet, is de Exchange-bruggenhoofdserver niet in staat licenties aan te vragen namens de gebruikers die het e-mailbericht ontvingen.

Voor Office SharePoint Server 2007 moet u het Active Directory-computerobject van de server met Office SharePoint Server 2007 toevoegen aan de serverservicesgroep. Als uw Office SharePoint Server 2007-server is geconfigureerd voor gebruik van de standaardserver in Active Directory, moet u de RMS-servicegroep en de groep die gemaakt is voor serverservices toevoegen aan het bestand ServiceLocater.asmx en de machtiging voor Lezen & Uitvoeren toestaan.

| ![](/security-updates/images/Cc747593.Important(WS.10).gif)Belangrijk                                                                                                                                                                   |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Internet Information Services (IIS) moet opnieuw worden gestart nadat u de DACL hebt gewijzigd in ServerCertification.asmx en ServiceLocater.asmx. Als u IIS opnieuw wilt instellen, voert u de opdracht **iisreset** vanaf een opdrachtregel uit. |
