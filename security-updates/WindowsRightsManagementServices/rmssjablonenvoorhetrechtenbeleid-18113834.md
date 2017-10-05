---
TOCTitle: 'RMS: Sjablonen voor het rechtenbeleid'
Title: 'RMS: Sjablonen voor het rechtenbeleid'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18113834
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720175(v=WS.10)'
---

RMS: Sjablonen voor het rechtenbeleid
=====================================

RMS-sjablonen
-------------

-   [Kan ik op alle inhoud die in een organisatie wordt gemaakt, een standaard RMS-sjabloon toepassen zodat er maar een minimale set met rechten nodig is?](#bkmk_57)
-   [Waar zijn de sjablonen voor het beleid van RMS opgeslagen?](#bkmk_58)
-   [Aan nieuwe sjablonen worden gebruikersaliassen en distributielijsten gekoppeld. Hoe kunnen binnen een organisatie sjablonen met dezelfde basisrechten aan afdelingen worden geleverd en hoe kunnen die rechten afhankelijk van de inhoud aan verschillende groepen worden toegekend?](#bkmk_59)
-   [Zijn de rechten die op een document worden toegepast, statische rechten? Kunnen na het verzenden van een bestand de rechten worden gewijzigd, ondanks het feit dat de uitgiftelicentie in het bestand is ingesloten en niet op de RMS-beleidsserver staat?](#bkmk_60)

<span id="BKMK_57"></span>
#### Kan ik op alle inhoud die in een organisatie wordt gemaakt, een standaard RMS-sjabloon toepassen zodat er maar een minimale set met rechten nodig is?

Ja. Met de Rights Management Services SDK kan een aangepaste toepassing worden ontwikkeld waarmee elke benodigde sjabloon kan worden toegepast. De implementatie van Information Rights Management in Office 2003 en later ondersteunt echter niet de toepassing van sjablonen op inhoud.

<span id="BKMK_58"></span>
#### Waar zijn de sjablonen voor het beleid van RMS opgeslagen?

De locatie van deze sjablonen wordt bepaald door de toepassing met RMS-ondersteuning. Voor Office 2003 en later wordt deze locatie als een gebruikersinstelling op de volgende plaats in het register opgeslagen:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

- of -

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12.0\\Common\\DRM\\AdminTemplatePath** voor Microsoft Office 2007.

| ![](images/Cc720175.note(WS.10).gif)Opmerking                                                                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als deze vermelding naar een lokale map op de client verwijst, moeten de sjabloonbestanden op de client worden opgeslagen. Verwijst deze vermelding daarentegen naar een gedeelde map in het netwerk, dan is deze map niet beschikbaar wanneer de gebruiker offline is. |

<span id="BKMK_59"></span>
#### Aan nieuwe sjablonen worden gebruikersaliassen en distributielijsten gekoppeld. Hoe kunnen binnen een organisatie sjablonen met dezelfde basisrechten aan afdelingen worden geleverd en hoe kunnen die rechten afhankelijk van de inhoud aan verschillende groepen worden toegekend?

Hiervoor zijn twee oplossingen:

-   Maak een sjabloon met de naam Vertrouwelijk die in licentie wordt gegeven aan alle werknemers in uw vestiging, gebruik die sjabloon in een e-mailbericht en verstuur dat bericht naar de desbetreffende personen. Het voordeel hiervan is, dat er voor de e-mail binnen de vestiging maar één sjabloon nodig is en dat die kan worden beperkt tot de gebruikers naar wie u de sjabloon stuurt. Het nadeel is dat iedere persoon die het e-mailbericht ooit heeft ontvangen en die niet meer bij het bedrijf werkt, het e-mailbericht nog kan lezen.
-   U kunt ook meerdere sjablonen maken, waaronder één voor elke distributielijst. Hoewel u hierdoor meer controle hebt, houdt dit ook in dat de IT-afdeling meerdere sjablonen moet ondersteunen.

<span id="BKMK_60"></span>
#### Zijn de rechten die op een document worden toegepast, statische rechten? Kunnen na het verzenden van een bestand de rechten worden gewijzigd, ondanks het feit dat de uitgiftelicentie in het bestand is ingesloten en niet op de RMS-beleidsserver staat?

Ja, dit is mogelijk als er een RMS-beleidssjabloon wordt gebruikt: Wanneer met behulp van een RMS-beleidssjabloon inhoud wordt gepubliceerd, blijft de definitie van het beleid op de server staan. Deze definitie kan na het publiceren van de inhoud door een beheerder worden gewijzigd. Vraagt een gebruiker een licentie voor de inhoud aan, dan worden de rechten van de licentie toegewezen conform het huidige beleid dat op de server is gedefinieerd. Als er rechten worden gewijzigd nadat een gebruikslicentie is toegewezen aan een gebruiker, krijgt de gebruiker de rechten zoals die golden op het moment dat de licentie werd uitgegeven. U kunt na het publiceren van de inhoud een nieuwe sjabloon voor het rechtenbeleid toepassen door een verloopbeleid voor de sjabloon in te schakelen en vervolgens de optie **Gebruikslicenties voor inhoud moeten worden vernieuwd elke: n dagen**. Geef voor x het aantal dagen op waarna een gebruiker een nieuwe gebruikslicentie moet aanvragen.
