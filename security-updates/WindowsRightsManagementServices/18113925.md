---
TOCTitle: De contactgegevens van de beheerder opgeven
Title: De contactgegevens van de beheerder opgeven
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18113925
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720237(v=WS.10)'
---

De contactgegevens van de beheerder opgeven
===========================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

De in deze procedure aangegeven beheerder moet een lokale beheerder zijn op de basiscertificeringsserver. De aangemelde gebruiker moet de rechten hebben voor het bestand SubEnrollService.asmx op de basiscertificeringsserver, zodat de gebruiker een licentieserver kan inrichten. Als een gebruiker probeert een licentieserver in te richten zonder machtiging voor dit bestand, kan de gebruiker een aanvraag verzenden naar de beheerder die is aangewezen voor het verlenen van de benodigde machtigingen. Zie '[Machtigingen instellen voor het bestand van de subinschrijvingsservice](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)' eerder in dit onderwerp voor meer informatie.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

De contactgegevens van de beheerder opgeven
-------------------------------------------

#### De contactgegevens van de beheerder opgeven

1.  Open de pagina **Algemeen beheer** en klik naast de website waarop u de contactgegevens van de beheerder wilt opgeven op **RMS op deze website beheren**.

2.  Klik in het gedeelte **Beheerkoppelingen** op **Certificeringsinstellingen**.

3.  Typ in het gedeelte '**Contactgegevens van de beheerder**' het e-mailadres van de beheerder waarmee contact moet worden opgenomen in geval van problemen met de subinschrijving tijdens het inrichten van een licentieserver (in de indeling *gebruikersnaam*@*domeinnaam*.com).

4.  Klik onder aan de pagina op **Verzenden**.
