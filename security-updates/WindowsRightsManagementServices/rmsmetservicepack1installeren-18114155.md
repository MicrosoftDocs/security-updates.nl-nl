---
TOCTitle: RMS met Service Pack 1 installeren
Title: RMS met Service Pack 1 installeren
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18114155
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747689(v=WS.10)'
---

RMS met Service Pack 1 installeren
==================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

De computer waarop u RMS installeert, moet een lidserver in een domein of een domeincontroller zijn. U kunt RMS niet implementeren op een zelfstandige server in een werkgroep.

| ![](images/Cc747689.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                                                                                                                                                 |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voltooi eerst de inrichting en installatie op de eerste basiscertificeringsserver, voordat u RMS op een andere server inricht. Zie '[De eerste basiscertificeringsserver inrichten](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)', '[Een licentieserver inrichten](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)' of '[Een server toevoegen aan een cluster](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)' voor instructies. |

| ![](images/Cc747689.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS SP1 kan op een server worden geïnstalleerd waarop nu de vorige versie van RMS is geïnstalleerd. Als u RMS uit bedrijf hebt genomen, dient RMS volledig te worden verwijderd. Installeer RMS SP1 alleen als u RMS via het onderdeel Software in het Configuratiescherm hebt verwijderd. |

RMS met Service Pack 1 installeren
----------------------------------

#### RMS met Service Pack 1 installeren

1.  Meld u op de server waarop u RMS SP1 wilt installeren aan met een domeinaccount die lid is van de lokale groep Administrators.

2.  Als het dialoogvenster **Welkom** verschijnt, controleert u de lijst met software die wordt geïnstalleerd en klikt u op **Volgende**.

3.  Lees in het dialoogvenster **Gebruiksrechtovereenkomst** de overeenkomst door, selecteer **Ik ga akkoord** en klik op **Volgende**.

4.  Accepteer bij **Map** de standaardmap of geef een nieuwe map op en klik op **Volgende**.

5.  Klik in het dialoogvenster **Installatie bevestigen** op **Installeren** om de installatie te starten.

6.  Als het dialoogvenster **Installatie voltooid** verschijnt, klikt u op **Sluiten**.

    | ![](images/Cc747689.note(WS.10).gif)Opmerking                                                                        |
    |---------------------------------------------------------------------------------------------------------------------------------------------------|
    | Als het foutbericht verschijnt dat de toepassing opnieuw wordt gestart, vernieuwt u de pagina **Algemeen beheer** in Microsoft Internet Explorer. |

U kunt RMS ook installeren vanaf een opdrachtregel. Zie '[RMS-server installeren vanaf de opdrachtregel](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)' verderop in dit onderwerp voor instructies.
