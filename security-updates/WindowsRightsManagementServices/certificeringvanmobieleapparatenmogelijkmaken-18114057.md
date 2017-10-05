---
TOCTitle: Certificering van mobiele apparaten mogelijk maken
Title: Certificering van mobiele apparaten mogelijk maken
ms:assetid: '93ec088e-9056-4c3c-bd97-1173fb194578'
ms:contentKeyID: 18114057
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747603(v=WS.10)'
---

Certificering van mobiele apparaten mogelijk maken
==================================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Deze procedure is alleen van toepassing op het basiscertificeringscluster.

Er wordt bij deze procedure van uitgegaan dat u een gebruikersgroep hebt gemaakt met de gebruikersaccounts van mobiele-apparaatgebruikers die door RMS beveiligde inhoud gebruiken.

Certificering van mobiele apparaten mogelijk maken
--------------------------------------------------

#### Certificering van mobiele apparaten mogelijk maken

1.  Open een browser voor het bestandssysteem op uw basiscertificeringsserver en ga naar de volgende map op het &lt;systeemstation&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification.

2.  Klik met de rechtermuisknop op het bestand MobileDeviceCertification.asmx en klik vervolgens op **Eigenschappen** als u wilt dat mobiele apparaten rechtenaccountcertificaten (RAC's) kunnen ontvangen.

3.  Kies **Toevoegen** op het tabblad **Beveiliging**, en voeg de groep toe die u hebt gemaakt voor deze categorie gebruikers en de **RMS-servicegroep**.

4.  Schakel in de lijst met **Machtigingen** voor de groepen het selectievakje **Toestaan** in voor zowel de machtigingen **Lezen** als **Lezen & Uitvoeren**, en klik vervolgens op **OK**.
