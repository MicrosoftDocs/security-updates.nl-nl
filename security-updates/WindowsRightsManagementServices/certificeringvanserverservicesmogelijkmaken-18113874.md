---
TOCTitle: Certificering van serverservices mogelijk maken
Title: Certificering van serverservices mogelijk maken
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18113874
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720196(v=WS.10)'
---

Certificering van serverservices mogelijk maken
===============================================

Als u deze procedure wilt uitvoeren, moet u lokaal bij de beheerwebsite zijn aangemeld met een domeingebruikersaccount die deel uitmaakt van de groep Administrators. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Deze procedure is alleen van toepassing op het basiscluster.

Met deze procedure wordt u verondersteld een gebruikersgroep te hebben gemaakt met de gebruikersaccounts die de serverservices zullen nabootsen als zij met rechten beveiligde inhoud gebruiken.

Certificering van serverservices mogelijk maken
-----------------------------------------------

#### Certificering van serverservices mogelijk maken

1.  Aanmelden bij de computer als lid van de lokale groep Administrators.

2.  Open een browser voor het bestandssysteem en ga naar de volgende map op het &lt;systeemstation&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification folder.

3.  Klik met de rechtermuisknop op het bestand ServerCertification.asmx en klik vervolgens op **Eigenschappen** als u wilt dat serverservices rechtenaccountcertificaten (RAC's) kunnen ontvangen.

4.  Kies **Toevoegen** op het tabblad **Beveiliging**, en voeg de groep toe die u hebt gemaakt voor deze categorie gebruikers en de **RMS-servicegroep**.

5.  Schakel in de lijsten met **Machtigingen** voor de groepen het selectievakje **Toestaan** in voor de machtigingen **Lezen & Uitvoeren**, en klik vervolgens op **OK**.

6.  Herhaal stap 1 - 4 voor elke server in het cluster.

| ![](images/Cc720196.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voor Microsoft Exchange Server 2007 moet u het Active Directory-computerobject van elke bruggenhoofdserver toevoegen aan de DACL (Discretionary Access Control list) van ServerCertification.asmx. Voeg ook voor Microsoft Office SharePoint Server 2007 het Active Directory-computerobject van de Office SharePoint Server 2007-server toe aan deze DACL. Het wordt aangeraden een beveiligingsgroep aan deze DACL toe te voegen, waaraan u vervolgens de juiste computerobjecten toevoegt. |
