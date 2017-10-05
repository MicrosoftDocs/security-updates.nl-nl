---
TOCTitle: 'Een gedistribueerde RMS-topologie plannen'
Title: 'Een gedistribueerde RMS-topologie plannen'
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18114058
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747657(v=WS.10)'
---

Een gedistribueerde RMS-topologie plannen
=========================================

In bepaalde omstandigheden kan het nodig zijn een of meer licentieservers in te zetten die geen lid zijn van het basiscertificeringscluster. Dit wordt meestal gedaan ter ondersteuning van afdelingen die rechtstreeks controle moeten uitoefenen over het uitgeven van uitgifte- en gebruikslicenties, zoals een juridische afdeling met beveiligingseisen die controle op afdelingsniveau noodzakelijk maken. Het basiscertificeringscluster verleent de accountcertificeringsservice voor de licentieservers. De combinatie van een basiscertificeringscluster en een of meer licentieserverinstallaties wordt een gedistribueerde topologie genoemd.

Houd er rekening mee dat, net als de basiscertificeringsserver, licentieservers eveneens in een cluster kunnen worden ingezet. Tevens maakt het licentiecluster, net als het basiscertificeringscluster, gebruik van een eigen taakverdelingsservice. Elke licentieserver of licentiecluster maakt gebruik van een afzonderlijke SQL Server-instantie die voorziet in de configuratie- en logboekdatabases voor die bepaalde server of dat cluster.

Hoewel u de RMS-installatie zo kunt instellen dat uitsluitend de certificeringsservices vanuit de basisinstallatie worden uitgevoerd en de volledige licentieverleningsservice vanuit een of meer licentieservers of -clusters wordt uitgevoerd, is dat niet de gangbare configuratie. Over het algemeen vergroot u het aantal fysieke servers in het basiscertificeringscluster om aan de prestatie- en redundantie-eisen te voldoen, in plaats van het inzetten van afzonderlijke licentieservers (tenzij het verlenen van licenties op afdelingsniveau moet worden ondersteund). Deze implementatie wordt in het volgende diagram geïllustreerd.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

Het bouwen van een gedistribueerde topologie kan meer beheerkosten betekenen voor uw organisatie, omdat een gedistribueerde topologie per definitie complexer is. Als uw organisatie meervoudige licentieclusters en meervoudige forests heeft, kan het nodig zijn het register van de RMS-clientcomputers handmatig te wijzigen zodat u zeker weet dat de licenties bij de juiste RMS-server worden aangevraagd. Bovendien kunnen zich vertrouwensproblemen voordoen tussen domeinen. Het is dan noodzakelijk de domeinen verder te configureren om de consumptie van door RMS beveiligde inhoud mogelijk te maken.

Serviceverbindingspunten in een gedistribueerde topologie
---------------------------------------------------------

Wanneer u een RMS-server inricht, wordt een cluster-URL toegevoegd aan het Active Directory-forest in een serviceverbindingspunt. Er is een serviceverbindingspunt voor het basiscertificeringscluster en voor elk licentiecluster dat in het forest is ingericht. Het serviceverbindingspunt voor het basiscertificeringscluster moet worden geregistreerd voordat u een licentiecluster inricht. Wanneer u het licentiecluster inricht, wordt voor de subinschrijving gebruikgemaakt van die URL om het basiscertificeringscluster op het netwerk te vinden en een serverlicentieverleningscertificaat te verkrijgen.

Als u een basiscertificeringscluster inzet in plaats van een enkele basiscertificeringsserver, moet elke server die onderdeel is van dat cluster virtueel kunnen worden geadresseerd achter een gedeelde URL.

Er zijn een aantal implementaties van virtuele adressering zoals Round Robin-DNS, de Windows Load Balancing-service, hardwareoplossingen, enzovoort. Virtuele adressering voorziet in taakverdeling over de servers en elimineert tevens de afhankelijkheid van een enkele server voor licentieverlening en uitgifte.

RMS gebruikt de gedeelde URL als de URL voor het verkrijgen van licenties en als de gepubliceerde waarde die door de computers van de eindgebruikers wordt gebruikt bij het opzoeken van het RMS-cluster in Active Directory of in het register. Geen enkele computer van een eindgebruiker hoeft dus rechtstreeks toegang te hebben tot welke server dan ook die zich binnen een cluster bevindt.
