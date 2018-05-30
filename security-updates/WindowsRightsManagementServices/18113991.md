---
TOCTitle: De pagina Algemeen beheer gebruiken
Title: De pagina Algemeen beheer gebruiken
ms:assetid: '57bbf402-2351-4dee-823c-27f4dd32447c'
ms:contentKeyID: 18113991
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747575(v=WS.10)'
---

De pagina Algemeen beheer gebruiken
===================================

Op de pagina **Algemeen beheer** van de beheerwebsite kunt u een RMS-server inrichten en de inrichting van een RMS-server ongedaan maken. Daarnaast kunt u de RMS-serviceaccount wijzigen.

Als u deze webpagina wilt openen vanaf de server die u wilt beheren, gaat u als volgt te werk:

1.  Meld u aan als lokale beheerder.
2.  Klik op **Start**, wijs **Alle programma's** in **Windows RMS** aan en klik op **Windows RMS-beheer**.

U kunt de pagina **Algemeen beheer** niet openen in een browser op een externe computer.

Als u de pagina **Algemeen beheer** opent op een server die u nog niet hebt ingericht, worden de volgende opties weergegeven voor elke website die op de server wordt uitgevoerd:

-   **RMS op deze website inrichten**. Klik op deze koppeling als dit de eerste server is die u wilt inrichten in dit cluster. Hiermee wordt het inrichtingsproces gestart waarin RMS-bronnen, zoals virtuele mappen, worden geïnstalleerd. Daarnaast worden de databases geïnstalleerd op de databaseserver. Zie '[De eerste basiscertificeringsserver inrichten](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)' verderop in dit onderwerp voor meer informatie.
-   **RMS aan een cluster toevoegen**. Klik op deze koppeling als u de server wilt inrichten en wilt toevoegen aan een bestaand cluster. U kunt een server toevoegen aan het basiscertificeringscluster of aan een licentiecluster. RMS-bronnen, zoals virtuele mappen, worden geïnstalleerd. Er worden echter geen databases gemaakt, omdat voor deze server de clusterdatabases worden gebruikt. Zie '[Een server toevoegen aan een cluster](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)' verderop in dit onderwerp voor meer informatie.

Als u de pagina **Algemeen beheer** opent op een server die al is ingericht, worden de volgende opties weergegeven:

-   **RMS op deze website beheren.** Klik op deze koppeling als u de pagina Clusterbeheer wilt openen. Zie '[De introductiepagina van de beheerwebsite gebruiken](https://technet.microsoft.com/6c155977-bd0e-47d6-ac65-1746cddb505e)' verderop in dit onderwerp voor meer informatie.
-   **RMS-serviceaccount wijzigen.** Klik op deze koppeling als u RMS onder een andere RMS-serviceaccount wilt uitvoeren. Zie '[De RMS-serviceaccount wijzigen](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)' verderop in dit onderwerp voor meer informatie.
-   **RMS van deze website verwijderen.**Klik op deze koppeling als u de inrichting van RMS ongedaan wilt maken. Als u de inrichting van RMS ongedaan maakt, worden de virtuele mappen en toepassingen voor RMS van deze server verwijderd. RMS wordt niet verwijderd. Zie '[De installatie van RMS ongedaan maken](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)' verderop in dit onderwerp voor meer informatie.

| ![](/security-updates/images/Cc747575.note(WS.10).gif)Opmerking                                                                                                                                                                                    |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| De beheerwebsite van RMS gebruikt pop-upvensters voor de configuratie van sommige functies. Als u pop-upblokkering gebruikt in uw webbrowser, moet u uw browserinstellingen dusdanig configureren dat pop-ups van de beheerwebsite van RMS worden toegestaan. |
