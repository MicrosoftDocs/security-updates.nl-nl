---
TOCTitle: 'RMS-servers uit bedrijf nemen'
Title: 'RMS-servers uit bedrijf nemen'
ms:assetid: '11badb02-62c1-455c-96b7-935bbcb496bc'
ms:contentKeyID: 18113943
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720200(v=WS.10)'
---

RMS-servers uit bedrijf nemen
=============================

Als u RMS uit bedrijf neemt, kunt u met een serversleutel de door RMS beveiligde inhoud decoderen die eerder met deze server is uitgegeven. Zo kan de inhoud zonder RMS-beveiliging worden opgeslagen. Dit kan nuttig zijn wanneer u geen RMS-beveiliging meer wilt gebruiken binnen uw organisatie.

Voer de server lang genoeg in deze modus uit om gebruikers de kans te geven hun inhoud zonder RMS-beveiliging op te slaan en netwerk- en systeembeheerders de mogelijkheid te bieden clients met RMS-ondersteuning uit te sluiten van deze service.

U kunt de service voor uit bedrijf nemen inschakelen via de pagina **Beveiligingsinstellingen** van de beheerwebsite. Als u deze service inschakelt, kunt u de standaardconfiguratie van de RMS-server niet meer herstellen. Bevat deze installatie vertrouwde uitgiftedomeinen, dan worden deze eveneens uit bedrijf genomen.

Als u de service voor uit bedrijf nemen hebt ingeschakeld, is op de beheerwebsite alleen de pagina **Informatie over uit bedrijf genomen server** beschikbaar. Er worden geen beheertaken ondersteund. Als u de server uit bedrijf wilt nemen, gaat u als volgt te werk:

1.  Gebruik IIS Manager om lees- en uitvoermachtigingen voor **RMS Service Group** toe te wijzen aan de uit bedrijf genomen virtuele hoofdmap.
2.  Voeg de groep **Iedereen** toe aan de DACL van het bestand decommissioning.asmx en geef iedereen leesbevoegdheden.
3.  Stel gebruikers op de hoogte dat u de RMS-installatie uit bedrijf neemt en adviseer ze verbinding te maken met de server om hun inhoud op te slaan zonder RMS-beveiliging.
4.  Configureer alle toepassingen met RMS-ondersteuning in uw onderneming zodanig dat verbinding wordt gemaakt met de pagina decommissioning.asmx. Afhankelijk van de toepassing met RMS-ondersteuning wordt deze mogelijk beheerd door een registersleutel of groepsbeleidsinstelling.
5.  Worden in uw organisatie toepassingen met RMS-ondersteuning gebruikt waarmee voor uitgifte automatisch gebruik wordt gemaakt van de installatie, dan moet u op deze computers in Groepsbeleid een registeringang instellen die zorgt dat in deze toepassingen de service voor uit bedrijf nemen wordt gebruikt.
6.  Wanneer de beveiliging voor alle inhoud is opgeheven, maakt u een back-up van de persoonlijke sleutel van de server en verwijdert u RMS van de server.
