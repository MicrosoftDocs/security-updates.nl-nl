---
TOCTitle: 'RMS: Mogelijke problemen met beveiliging'
Title: 'RMS: Mogelijke problemen met beveiliging'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18114224
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747757(v=WS.10)'
---

RMS: Mogelijke problemen met beveiliging
========================================

Beveiliging met RMS
-------------------

-   [Wat is de account van de supergebruiker?](#bkmk_43)
-   [Is RMS een beveiligingsprogramma?](#bkmk_44)
-   [Welke mechanismen worden gebruikt om te voorkomen dat gebruikers de tijd op hun computers kunnen terugzetten, zodat zij een met rechten beveiligd document ook na het verlopen van de gebruikslicentie kunnen blijven gebruiken?](#bkmk_45)
-   [Kunnen leden van de groep Domeinadministrators documenten lezen die voor iemand anders in het domein zijn bedoeld?](#bkmk_46)
-   [Ik begrijp dat de certificaten of licenties die in het systeem worden gegenereerd, door elke lockbox kunnen worden geverifieerd alsof die certificaten of licenties afkomstig zijn van een service die bij Microsoft is geregistreerd. Welk gevaar wordt hiermee ingedamd?](#bkmk_47)
-   [Als het iemand door 'bruut geweld' lukt een document te openen, kunnen met die sleutel dan ook andere documenten worden geopend?](#bkmk_48)
-   [Zijn vanwege de exportbeperkingen op coderingstechnologieën delen van de sleutels bekend buiten de onderneming waar deze sleutels worden gebruikt?](#bkmk_49)
-   [Hoe kunt u voorkomen dat kwaadwillende gebruikers de functie voor het uit bedrijf nemen op afstand kunnen inschakelen?](#bkmk_50)
-   [Kan een gebruiker de schermuitvoer van met rechten beveiligde inhoud vastleggen?](#bkmk_51)
-   [Kunnen beheerders die back-ups maken van bestanden die betrekking hebben op RMS, met rechten beveiligde inhoud openen?](#bkmk_52)
-   [Staat in het wisselbestand dat in Windows wordt gebruikt de ongecodeerde inhoud zodat in feite de inhoud niet is beveiligd en door iedereen kan worden bekeken?](#bkmk_53)
-   [Is het mogelijk te bepalen welke beheerders welke beheerfuncties van RMS kunnen gebruiken?](#bkmk_54)
-   [Kunnen met RMS documenten direct na te zijn gemaakt, afzonderlijk worden beveiligd op de computer van een gebruiker of in een gedeelde map?](#bkmk_55)
-   [Zijn bij het openen van een bestand de automatisch opgeslagen bestanden en tijdelijke bestanden gecodeerd?](#bkmk_56)
-   [Wanneer ik een met rechten beveiligd e-mailbericht ontvang, lijkt het alsof het e-mailbericht een bijlage bevat. Ik kan die bijlage opslaan, terwijl het e-mailbericht klaarblijkelijk niet kan worden opgeslagen. Werkt RMS niet meer?](#bkmk_562)

<span id="BKMK_43"></span>
#### Wat is de account van de supergebruiker?

RMS ondersteunt de speciale groep Supergebruikers. Leden van deze groep hebben volledig beheer over alle met rechten beveiligde inhoud. Aan de leden van de groep Supergebruikers worden volledige eigenaarsrechten toegewezen voor alle gebruikslicenties die aan hen worden uitgegeven door de RMS-cluster waarvoor de groep Supergebruikers is geconfigureerd. Dit betekent dat leden van deze groep alle beveiligde bestanden kunnen decoderen en de beveiliging kunnen opheffen. Een lid van deze groep kan bijvoorbeeld de beveiliging opheffen voor bestanden die zijn uitgegeven door een ontslagen medewerker, zodat een nieuwe eigenaar de bestanden kan uitgeven en beheren.

<span id="BKMK_44"></span>
#### Is RMS een beveiligingsprogramma?

Nee, RMS is geen beveiligingsprogramma. Wanneer RMS bij een toepassing met RMS-ondersteuning zoals Office 2007 wordt gebruikt, kan RMS worden beschouwd als een programma waarmee beleid wordt opgelegd. Als de gebruiker niet is gemachtigd om de gegevens te bekijken, kan hij of zij met 'bruut geweld' proberen de codering te kraken. De codering is veilig maar kan net als alle andere softwarecoderingen worden gekraakt. Mag de gebruiker de gegevens bekijken, dan kan hij of zij die gegevens doorspelen aan gebruikers die de gegevens niet mogen bekijken, door er een kopie of schermafdruk van te maken.

<span id="BKMK_45"></span>
#### Welke mechanismen worden gebruikt om te voorkomen dat gebruikers de tijd op hun computers kunnen terugzetten, zodat zij een met rechten beveiligd document ook na het verlopen van de gebruikslicentie kunnen blijven gebruiken?

RMS merkt of de tijd op het clientsysteem vooruit of achteruit is gezet en zorgt ervoor dat de gebruiker de inhoud niet kan gebruiken. Ook worden door RMS meetbare tijdsverschillen tussen de RMS-server en -client opgemerkt.

<span id="BKMK_46"></span>
#### Kunnen leden van de groep Domeinadministrators documenten lezen die voor iemand anders in het domein zijn bedoeld?

Leden van de groep Domeinadministrators kunnen inhoud lezen die voor een gebruikersaccount is beveiligd, als zij lid van de RMS-groep Supergebruikers zijn of als de gebruikersaccount van hen is. Omdat leden van de groep Domeinadministrators controle hebben over de gebruikersaccounts in het domein, is er geen scenario om het gevaar van een onbetrouwbaar lid van de groep Domeinadministrators uit te sluiten.

Voeg daarom uitsluitend leden uit de groep Domeinadministrators aan de groep Supergebruikers toe als zij toegang tot met rechten beveiligde inhoud moeten hebben. Wanneer een licentie wordt verleend aan een lid van de groep Supergebruikers, wordt gebeurtenis-id 49 in het gebeurtenislogboek voor toepassingen op de RMS-server vastgelegd. Gebeurtenis-id 49 houdt het volgende in: **'Er is een licentie verleend aan een lid van de groep Supergebruikers. De gebruiker heeft het volgende e-mailadres: &lt;Gebruikersalias&gt;”** waarbij **Gebruikersalias** wordt vervangen door de e-mailaccount van de gebruiker.

Net zoals bij andere groepen waarmee de toegang tot bronnen wordt beperkt, moet u waarschuwingen definiëren en beveiligingscontroles uitvoeren om te voorkomen dat iemand zonder te zijn gevalideerd, aan de groep Supergebruikers wordt toegevoegd.

<span id="BKMK_47"></span>
#### Ik begrijp dat de certificaten of licenties die in het systeem worden gegenereerd, door elke lockbox kunnen worden geverifieerd alsof die certificaten of licenties afkomstig zijn van een service die bij Microsoft is geregistreerd. Welk gevaar wordt hiermee ingedamd?

Zonder de integriteit van certificaten te kunnen verifiëren kan een gebruiker het rechtenaccountcertificaat dat aan een andere gebruiker is toegekend, vervalsen en een gebruikslicentie voor inhoud bemachtigen of een toepassing maken waarmee de beveiliging van een document kan worden opgeheven.

<span id="BKMK_48"></span>
#### Als het iemand door 'bruut geweld' lukt een document te openen, kunnen met die sleutel dan ook andere documenten worden geopend?

Alle met rechten beveiligde inhoud is gecodeerd met een andere, willekeurig gegenereerde symmetrische sleutel. Daarom heeft elk document een unieke sleutel waarmee andere documenten niet kunnen geworden gedecodeerd.

<span id="BKMK_49"></span>
#### Zijn vanwege de exportbeperkingen op coderingstechnologieën delen van de sleutels bekend buiten de onderneming waar deze sleutels worden gebruikt?

Toepassingen die zijn ondertekend met de hoofdsleutel van Microsoft, voldoen aan de hoofdhandtekeningssleutel van Microsoft, maar verder worden er geen andere sleutels door Microsoft of als gevolg van een implementatie bij een klant openbaar gemaakt.

<span id="BKMK_50"></span>
#### Hoe kunt u voorkomen dat kwaadwillende gebruikers de functie voor het uit bedrijf nemen op afstand kunnen inschakelen?

De aanvaller heeft de referenties van een gebruikersaccount met beheerdersrechten voor de RMS-cluster nodig. Standaard is de RMS-beheerinterface alleen lokaal op de RMS-server beschikbaar. U verkleint het risico door ervoor te zorgen dat die interface alleen op de RMS-server beschikbaar is, dat Remote Desktop Protocol (RDP) is uitgeschakeld en dat de server is beveiligd.

<span id="BKMK_51"></span>
#### Kan een gebruiker de schermuitvoer van met rechten beveiligde inhoud vastleggen?

Als de kopieerfunctie in de RMS-rechten is uitgeschakeld, is de toetsencombinatie ALT + PRINT SCRN van Windows door RMS uitgeschakeld. In een omgeving waarin de desktops niet worden beheerd, kan een gebruiker deze beveiliging altijd omzeilen door met een product van een andere leverancier dan Microsoft een schermafdruk van inhoud te maken.

<span id="BKMK_52"></span>
#### Kunnen beheerders die back-ups maken van bestanden die betrekking hebben op RMS, met rechten beveiligde inhoud openen?

Nee. Zij kunnen wel de back-up maken maar hebben geen toegang tot de inhoud.

<span id="BKMK_53"></span>
#### Staat in het wisselbestand dat in Windows wordt gebruikt de ongecodeerde inhoud zodat in feite de inhoud niet is beveiligd en door iedereen kan worden bekeken?

Nadat gedecodeerde inhoud door de RMS-client weer naar de toepassing is gestuurd, kan de inhoud in het wisselbestand komen te staan. Een deel van de aanbevelingen voor de ontwikkeling van de RMS-toepassingen uit de Rights Management Services (RMS) Software Development Kit (SDK) zijn de stappen om dit te voorkomen, maar de toepassing met RMS-ondersteuning neemt toch het leeuwendeel hiervan voor zijn rekening.

<span id="BKMK_54"></span>
#### Is het mogelijk te bepalen welke beheerders welke beheerfuncties van RMS kunnen gebruiken?

Ja. U kunt een andere RMS-beheerdersgroep in Active Directory maken, gebruikers toevoegen en vervolgens de betreffende toegangscontrolelijst (ACL) voor de beheerpagina's maken. In de standaardconfiguratie voor de toegangscontrolelijsten van de webpagina voor RMS-beheer kan zijn ingesteld, dat de pagina met de beveiligingsinstellingen alleen kan worden geopend door de gebruiker die de server heeft ingericht.

<span id="BKMK_55"></span>
#### Kunnen met RMS documenten direct na te zijn gemaakt, afzonderlijk worden beveiligd op de computer van een gebruiker of in een gedeelde map?

Alhoewel documenten op de lokale computer van gebruikers met RMS kunnen worden beveiligd, wordt toch de voorkeur gegeven aan Encrypting File System (EFS). EFS beveiligt documenten transparant, terwijl bij RMS de gebruiker enkele handelingen (klikken met de muis) moet uitvoeren om een document te beveiligen.

<span id="BKMK_56"></span>
#### Zijn bij het openen van een bestand de automatisch opgeslagen bestanden en tijdelijke bestanden gecodeerd?

Ja, alle tijdelijke bestanden zijn gecodeerd.

<span id="BKMK_562"></span>
#### Wanneer ik een met rechten beveiligd e-mailbericht ontvang, lijkt het alsof het e-mailbericht een bijlage bevat. Ik kan die bijlage opslaan, terwijl het e-mailbericht klaarblijkelijk niet kan worden opgeslagen. Werkt RMS niet meer?

Nee. Dit is normaal. De bijlage die u ziet, is het gecodeerde bericht voordat de RMS-client het bericht heeft gedecodeerd. Het bericht wordt nog steeds met rechten beveiligd en kan niet worden opgeslagen als het is gedecodeerd.
