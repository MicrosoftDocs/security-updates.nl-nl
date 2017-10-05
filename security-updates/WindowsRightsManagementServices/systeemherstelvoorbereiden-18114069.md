---
TOCTitle: Systeemherstel voorbereiden
Title: Systeemherstel voorbereiden
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18114069
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747659(v=WS.10)'
---

Systeemherstel voorbereiden
===========================

Het uitvallen van een onderdeel van het RMS-systeem, waaronder de internet- en intranetverbindingen die door de RMS-server worden gebruikt, de RMS-certificeringsserver, ingeschreven RMS-licentieservers of de databaseservers die als host optreden voor de RMS-configuratiedatabases, kunnen leiden tot onverwachte onderbreking van de service. Wanneer u een RMS-systeem installeert, moet u zich terdege realiseren wat de gevolgen van een uitval van een RMS-service voor uw IT-systemen kunnen zijn en moet u het uitgevallen onderdeel zo snel mogelijk herstellen.

Het uitvallen van de databaseservers die als host fungeren voor de RMS-configuratiedatabases, kan er de oorzaak van zijn dat gebruikers geen toegang meer hebben tot door RMS beveiligde gegevens. In dit gedeelte krijgt u een overzicht van de belangrijke overwegingen en factoren waarmee u rekening dient te houden wanneer u een RMS-systeem gaat herstellen:

-   [Internetconnectiviteit](#bkmk_1)
-   [Intranetconnectiviteit](#bkmk_2)
-   [Certificerings- en licentieservices](#bkmk_3)
-   [Databaseservers](#bkmk_4)
-   [Active Directory](#bkmk_5)

<span id="BKMK_1"></span>
Internetconnectiviteit
----------------------

Als u servers on line inschrijft, moet de RMS-server tijdens de inrichting verbinding met internet hebben om een serverlicentieverleningscertificaat te kunnen ophalen en dat elk jaar te kunnen vernieuwen. Wanneer het certificaat bijna is verlopen, ontvangt u van de certificeringsserver een bericht om het certificaat te vernieuwen door gebeurtenissen in het logboek voor systeemgebeurtenissen te registreren. Gebeurtenissen worden geregistreerd één maand voor de vervaldatum van het serverlicentieverleningscertificaat (gebeurtenis-id 16), één week voor de vervaldatum van het serverlicentieverleningscertificaat (gebeurtenis-id 17) en wanneer het serverlicentieverleningscertificaat verloopt (gebeurtenis-id 18). De RMS-webpagina Algemeen beheer van de website RMS-beheer waarschuwt ook wanneer de vervaldatum van het serverlicentieverleningscertificaat nadert. Als u het RMS-beheerpakket voor Microsoft Operations Manager (MOM) gebruikt, wordt er een waarschuwing door de vervalgebeurtenissen gegeven. Als er vanaf de RMS-server geen verbinding met internet is, kan het serverlicentieverleningscertificaat niet via de knop **Vernieuwen** op de RMS-beheerwebsite worden vernieuwd en moet er via het off line inschrijvingsproces een aanvraag voor een bijgewerkt certificaat worden ingediend.

Vernieuw het serverlicentieverleningscertificaat ruim voor de vervaldatum om problemen te voorkomen als de internetverbinding op de vervaldatum om de een of andere reden niet beschikbaar is. De RMS-server kan zonder geldig serverlicentieverleningscertificaat geen RMS-services verlenen. Dat betekent dat gebruikers geen door RMS beveiligde gegevens kunnen publiceren of geen gebruikslicenties en rechtenaccountcertificaten kunnen krijgen die nodig zijn om door RMS beveiligde inhoud te kunnen lezen. Gebruikers die reeds gebruikslicenties en rechtenaccountcertificaten voor gedeelten van de door RMS beveiligde inhoud hebben, kunnen de gegevens blijven openen zolang hun gebruikslicenties en rechtenaccountcertificaten geldig zijn.

<span id="BKMK_2"></span>
Intranetconnectiviteit
----------------------

RMS is een client/server-technologie op basis van een verbonden infrastructuur. Zonder een werkend intranetnetwerk kunnen RMS-servers geen verbinding maken met de vereiste services in het bedrijf of services aan de gebruikers verlenen. Zonder intranetverbinding kunnen gebruikers geen rechtenaccountcertificaten (RAC's), clientlicentieverleningscertificaten (CLC's) en gebruikslicenties van de RMS-servers ontvangen.

Het is het overwegen waard binnen organisaties redundante routingarchitecturen en overnamekoppelingen van externe sites naar de sites met de RMS-server te implementeren.

Nadat een gebruiker een clientlicentiecertificaat voor de computer heeft ontvangen, kan die gebruiker door RMS beveiligde gegevens off line publiceren als op dat moment een RMS-server niet kan worden bereikt. Sommige e-mailtoepassingen met RMS-ondersteuning zijn ingesteld voor het automatisch downloaden van gebruikslicenties voor de betreffende door RMS beveiligde e-mailberichten tijdens het synchroniseren van een postbus. De gebruiker kan dan toch door RMS beveiligde e-mailberichten lezen, ook als er geen verbinding met het intranet is.

<span id="BKMK_3"></span>
Certificerings- en licentieservices
-----------------------------------

Het RMS-systeem maakt veelvuldig gebruik van twee virtuele mappen in Internet Information Services (IIS) 6.0, namelijk de certificerings- en licentieservices. Met deze services kunnen gebruikers en hun computers worden ingeschreven in de RMS-omgeving en kunnen toepassingen met RMS-ondersteuning door RMS beveiligde gegevens publiceren en openen. Als deze services niet beschikbaar zijn, hebben de gebruikers waarschijnlijk pas weer toegang als de beschikbaarheid van deze services is hersteld.

Om de mogelijke uitval van services te voorkomen zou u clusters met certificeringsservers en ingeschreven licentieservers kunnen maken, zodat bij uitval van een knooppunt in een cluster de beschikbaarheid van een service niet in gevaar komt.

U kunt het beste voor overcapaciteit in de clusters zorgen. Hiermee voorkomt u problemen wanneer er zich een storing op een van de knooppunten voordoet. Wanneer u de eerste certificeringsserver en elke ingeschreven licentieserver of de eerste ingeschreven licentieserver in een cluster installeert, moet u de configuratieopties en de gegevens noteren die tijdens de inrichting worden ingevoerd.

<span id="BKMK_4"></span>
Databaseservers
---------------

De belangrijkste onderdelen in het RMS-systeem zijn de databaseservers met de configuratiedatabases. Op elke RMS-server of in elk cluster met servers worden de configuratie- en logboekgegevens in databases opgeslagen. De configuratie is van essentieel belang voor het functioneren van RMS. In deze databases staan het serverlicentieverleningscertificaat, de gemaakte RMS-beleidssjablonen, een lijst met gebruikers die in het RMS-systeem zijn ingeschreven, en de persoonlijke en openbare sleutels van de RMS-server als er bij deze server geen hardwarebeveiligingsmodule is gebruikt. U kunt een vorige installatie van RMS met een back-up van de RMS-databases op een nieuw systeem herstellen en vervolgens een RMS-systeem maken. De gevolgen van het verlies van een database zijn per database anders. In de volgende tabel worden de gevolgen van een fout met de volgende databases beschreven:

-   **Configuratiedatabase**. Als deze database niet meer beschikbaar is tijdens de werking van de RMS-server, kunnen de RMS-services gewoon blijven doorwerken omdat de vereiste gegevens lokaal door RMS worden opgeslagen. Als er zich echter een gebeurtenis voordoet waarbij de RMS-service moet communiceren met de configuratiedatabase, zoals bij de inschrijving van een nieuwe gebruiker, doet er zich een fout voor bij de RMS-service en kan de nieuwe gebruiker niet met door RMS beveiligde inhoud werken. Wordt er een bewerking uitgevoerd en de RMS-server moet daardoor de opgeslagen gegevens verwijderen, bijvoorbeeld door het opnieuw starten van de IIS-service of een geplande vernieuwing van de lokale cache, dan stopt de RMS-service. De RMS-server kan de normale service pas hervatten als de configuratiedatabase beschikbaar is.
    Als de configuratiedatabase beschadigd raakt of helemaal niet meer beschikbaar is, stoppen de RMS-servers.
-   **Database met directoryservices**. In deze database staan groepsnamen en gegevens over hun lidmaatschappen die van een globale-catalogusserver afkomstig zijn. Als deze database enige tijd niet beschikbaar is, heeft dit geen merkbare gevolgen voor de RMS-services. Het voornaamste doel van deze database is het bieden van redundantie en het verminderen van de servicebelasting voor de globale-catalogusserver.
-   **Logboekdatabase**. Als logboekregistratie op de RMS-server is ingeschakeld, wordt het logboek in deze database opgeslagen. Is de database niet beschikbaar, dan worden de logboekvermeldingen opgeslagen in de Message Queuing-service (ook wel genoemd MSMQ) op de RMS-server en wordt alle beschikbare schijfruimte gebruikt, tenzij dit anders is ingesteld in de configuratie.

Wij raden u aan uit veiligheidsoverwegingen de databaseservers te clusteren, zodat bij storing een andere server de taken kan overnemen. Maak ook regelmatig een back-up van de databases voor de RMS-certificeringsservers en -clusters en voor de licentieservers en -clusters.

U kunt ook met een transactielogboek een back-updatabase onderhouden. Hiervoor is wel extra hardware nodig, maar het grote voordeel is dat databases sneller kunnen worden hersteld. Microsoft IT heeft deze methode voor het herstellen van RMS-configuratiedatabases toegevoegd. U voert dit uit door de virtuele SQL-naam tijdens het inrichten van RMS te selecteren. Met de virtuele SQL-naam kunt u met behulp van het DNS (Domain Name System) de echte SQL-naam toewijzen. Mocht de SQL-server ermee ophouden, dan kunt u gemakkelijk overschakelen naar de reserve SQL Server door de DNS-naamtoewijzing van de originele server in de reserveserver te wijzigen. Zie de case-study van Microsoft Corporation op de [website van Microsoft](http://go.microsoft.com/fwlink/?linkid=42070) (http://go.microsoft.com/fwlink/?LinkId=42070) voor meer informatie over de interne implementatie van deze oplossing bij Microsoft.

<span id="BKMK_5"></span>
Active Directory
----------------

RMS gebruikt Active Directory voor twee belangrijke services: verificatie van gebruikers en de globale-catalogusservice. Als Active Directory niet beschikbaar is, kunnen gebruikers niet worden geverifieerd en kunnen gebruikers en hun computers niet in het RMS-systeem worden ingeschreven. De verificatiepijplijn is nodig om een rechtenaccountcertificaat te kunnen krijgen. Deze pijplijn moet worden geverifieerd. Zodra een gebruiker een rechtenaccountcertificaat heeft, kan die persoon zonder verdere verificatie gebruikslicenties krijgen, omdat de licentiepijplijn standaard anoniem is.

Bedrijfsentiteiten kunnen met groepslidmaatschappen in Active Directory aangeven wie toegang heeft tot door RMS beveiligde gegevens. Bij uitval van Active Directory kunnen er geen gebruikslicenties meer aan gebruikers worden verstrekt. Standaard worden de gegevens van groepslidmaatschappen 15 minuten op de RMS-server bewaard, zodat een tijdelijke uitval van de globale-catalogusservice niet voor problemen zorgt. U wijzigt de registersleutel voor de geldigheidsduur als u de tijd tussen de updates van de cache langer of korter wilt maken. Zie 'Cache-instellingen voor Active Directory wijzigen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.
