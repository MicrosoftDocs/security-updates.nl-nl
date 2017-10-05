---
TOCTitle: Servers toevoegen ter ondersteuning van certificering en licenties
Title: Servers toevoegen ter ondersteuning van certificering en licenties
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18113864
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720189(v=WS.10)'
---

Servers toevoegen ter ondersteuning van certificering en licenties
==================================================================

Als u de eerste server hebt geïnstalleerd en ingericht om de basisinstallatie van RMS tot stand te brengen, kunt u meer servers instellen om de ondersteuning voor certificerings- en licentieservices uit te breiden. U kunt bijvoorbeeld:

-   een server aan een basiscertificeringscluster toevoegen voor een betere certificerings- en licentieondersteuning. Een server die aan dit cluster wordt toegevoegd, heeft dezelfde configuratie en gebruikt dezelfde databases als de basiscertificeringsserver.
-   Een licentieserver instellen als een aparte server of als een lid van een cluster met licentieservers. Deze wordt ingeschreven in het basiscertificeringscluster en ontvangt het serverlicentieverleningscertificaat (SLC) via de certificeringsservices van de basiscertificeringsserver. Clientaanvragen voor certificeringsservices worden doorgestuurd naar de certificeringsserver. Met de licentieserver kunnen gebruiks- en uitgiftelicenties worden uitgegeven. Aanvragen voor deze services worden niet doorgestuurd naar de basiscertificeringsserver.

Welke implementatie voor u het meest geschikt is, hangt af van de grootte van uw organisatie en van uw wensen op het gebied van redundantie, schaalbaarheid, taakverdelingsondersteuning en beveiliging. Als u extra RMS-servers implementeert om het groeiende aantal certificerings-, licentie- en uitgifteaanvragen te kunnen verwerken, moet u RMS-servers als onderdeel van het basiscertificeringscluster implementeren zodat u redundantie en taakverdeling kunt instellen voor alle servers. U kunt certificeringsservers clusteren en de verwerking overnemen voor licentie- en uitgifteservices door licentieservers in te schrijven (die ook voor taakverdeling mogen worden geclusterd), maar u kunt de taakverdeling van een subingeschreven licentieserver met een basiscertificeringscluster niet instellen.

In de volgende onderwerpen vindt u richtlijnen voor deze taak:

-   [Vereiste rollen, machtigingen en rechten voor installatie en inrichting](#bkmk_1)
-   [Het inrichtingsproces voor extra certificerings- en licentieservers](#bkmk_2)
-   [Clusters en taakverdeling instellen](#bkmk_3)

<span id="BKMK_1"></span>
Vereiste rollen, machtigingen en rechten voor installatie en inrichting
-----------------------------------------------------------------------

Voor het installeren en inrichten van extra servers hebt u dezelfde rollen, machtigingen en rechten nodig als voor het instellen van de eerste server. Daarnaast hebt u machtigingen van de basiscertificeringsserver nodig om een aparte licentieserver in te stellen. Dit proces wordt subinschrijving genoemd. De basiscertificeringsserver wordt beheerd via de DACL van het bestand SubEnrollService.asmx. Leden van de RMS-servicegroep, waaronder de RMS-serviceaccount die u tijdens het inrichten van de basiscertificeringsserver hebt opgegeven, hebben toestemming om subinschrijving uit te voeren. Zie '[Certificerings- en licentieservices instellen op de eerste server](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b)' in dit onderwerp voor meer informatie.

<span id="BKMK_2"></span>
Het inrichtingsproces voor extra certificerings- en licentieservers
-------------------------------------------------------------------

Als u servers aan certificerings- en licentieclusters toevoegt, moet het inrichtingsproces worden voltooid door de server. Welke taken tijdens het inrichtingsproces moeten worden uitgevoerd, is afhankelijk van het type server dat u inricht.

-   Als u een aparte licentieserver inricht, geeft u op dezelfde wijze als voor een basiscertificeringsserver een configuratiedatabase, RMS-serviceaccount en cluster-URL op en stelt u in hoe u de persoonlijke sleutels wilt beveiligen. U hoeft echter geen intrekkingsbeleid voor serverlicentiecertificaten op te geven omdat dit beleid wordt beheerd via de basiscertificeringsserver.
-   Als u een server inricht als een clusterlid, hoeft u tijdens het inrichten alleen maar de RMS-serviceaccount, de configuratiedatabase en het wachtwoord voor de beveiliging van persoonlijke sleutels op te geven. Desgewenst kunt u ook opgeven dat u dezelfde cryptografieprovider en persoonlijke sleutel als van het bestaande cluster wilt gebruiken. Voor alle servers in een cluster worden hetzelfde serverlicentiecertificaat en serversleutelpaar gebruikt.

| ![](images/Cc720189.Important(WS.10).gif)Belangrijk                                       |
|------------------------------------------------------------------------------------------------------------------------|
| Installeer RMS pas op andere servers wanneer u de inrichting en installatie van RMS op de eerste server hebt voltooid. |

Wanneer u een extra server hebt geïnstalleerd en ingericht, wordt deze automatisch geconfigureerd als een clusterlid. Hebt u taakverdeling geïmplementeerd, dan moet u de taakverdelingssoftware echter configureren om met de nieuwe server te werken.

<span id="BKMK_3"></span>
Clusters en taakverdeling instellen
-----------------------------------

RMS ondersteunt serverclusters. Als u clusters van RMS-servers maakt, komt dit ten goede aan de schaalbaarheid en betrouwbaarheid van en taakverdeling binnen uw RMS-implementatie.

**Clusters maken**

Als u een cluster wilt instellen, begint u met een basiscertificeringsserver of licentieserver. Vervolgens installeert u RMS op de overige servers in het cluster. Ga naar de pagina **Algemeen beheer** en klik op **Deze server aan een cluster toevoegen** om de benodigde bronnen in te stellen en de server aan het basiscertificerings- of licentiecluster toe te voegen.

Geef de databasenaam op van het cluster waaraan u de server wilt toevoegen.

**Taakverdelingsclusters**

In RMS wordt taakverdeling niet automatisch geïmplementeerd. U kunt hardware- of softwaretaakverdeling gebruiken, zoals Network Load Balancing, om de taken over de RMS-servers te verdelen.

De volgende onderwerpen bevatten meer informatie over dit onderwerp:

-   Zie 'RMS-systeem: overzicht' in 'Technische referentie van RMS' in deze documentatie voor meer informatie over de verschillen tussen certificerings- en licentieservices.
-   Zie 'Redundantie en taakverdeling verzorgen' in 'Een RMS-implementatie plannen' in deze documentatie voor meer informatie over de wijze waarop u serverimplementaties afstemt op de vereisten voor beschikbaarheid en prestaties van uw organisatie.
-   Zie 'Schaalbaarheidsvereisten evalueren' in 'Een RMS-implementatie plannen' in deze documentatie voor meer informatie over de wijze waarop u bepaalt hoeveel servers vereist zijn voor de implementatie van RMS in uw organisatie.
-   Zie '[De RMS-implementatie beveiligen](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14)' verderop in dit onderwerp voor meer informatie over het implementeren van IT-beveiliging in uw RMS-implementatie.
-   Zie 'RMS met Service Pack 1 installeren' in 'Een RMS-server beheren' in deze documentatie voor informatie over het installeren van RMS.
    U kunt RMS ook installeren vanaf een opdrachtregel. Zie 'RMS installeren vanaf de opdrachtregel' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.
-   Zie 'Een licentieserver inrichten' in 'Een RMS-server beheren' in deze documentatie voor informatie over het inrichten van een licentieserver.
-   Zie 'Een server toevoegen aan een cluster' in 'Een RMS-server beheren' voor informatie over het inrichten van extra servers in een clusters.
