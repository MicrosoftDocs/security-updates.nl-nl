---
TOCTitle: 'Het wachtwoord voor de RMS-serviceaccount wijzigen'
Title: 'Het wachtwoord voor de RMS-serviceaccount wijzigen'
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18113960
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720273(v=WS.10)'
---

Het wachtwoord voor de RMS-serviceaccount wijzigen
==================================================

Afhankelijk van het wachtwoordbeleid dat u opgeeft voor de RMS-servers, verloopt het wachtwoord van de RMS-serviceaccount na een bepaalde periode. Als het wachtwoord is verlopen, werkt RMS niet meer. U dient het wachtwoord daarom te wijzigen voordat het verloopt.

**Eén RMS-serviceaccount gebruiken**

Als u één RMS-serviceaccount gebruikt, kunt u het wachtwoord op elke RMS-server as volgt wijzigen:

1.  Als de server in een cluster is opgenomen, verwijdert u de server uit het cluster.
2.  Meld u op de server aan met de referenties van de RMS-serviceaccount.
3.  Wijzig het wachtwoord voor de RMS-serviceaccount.
    Op de andere servers waarvoor dezelfde RMS-serviceaccount wordt gebruikt, zijn services niet meer beschikbaar omdat de referenties die op deze servers zijn opgeslagen, niet meer geldig zijn nadat het wachtwoord is gewijzigd.
4.  Meld u af bij de server.
5.  Meld u weer als Windows RMS-beheerder bij de server aan.
6.  Als u de gebruikersidentiteit op de server opnieuw wilt configureren, klikt u op de pagina **Algemeen Beheer** op **RMS-serviceaccount wijzigen**. Op de pagina **RMS-serviceaccount wijzigen** geeft u vervolgens het domein, de gebruikersnaam en het wachtwoord op.
7.  Start IIS opnieuw op.
8.  Indien van toepassing neemt u de server weer op in het cluster.
9.  Herhaal stap 6 tot en met 8 voor elke server in het cluster.

Dit is de eenvoudigste manier om het wachtwoord voor de RMS-serviceaccount te wijzigen. RMS kan hierdoor echter enige tijd buiten bedrijf zijn omdat Active Directory wordt bijgewerkt met het nieuwe wachtwoord wanneer u het wachtwoord voor de RMS-serviceaccount op een server wijzigt. In IIS worden de groepen toepassingen regelmatig opnieuw gestart. Groepen van toepassingen die met de oude referenties worden uitgevoerd, kunnen echter pas worden gestart als u het wachtwoord voor de RMS-serviceaccount hebt gewijzigd en IIS opnieuw hebt opgestart op die server. RMS werkt pas weer als de groep van toepassingen weer worden uitgevoerd.

**Twee RMS-serviceaccounts gebruiken**

Bij deze methode maakt u eerst twee RMS-serviceaccounts met een verschillend verloopbeleid of verschillende verloopdatums. Tijdens normale bewerkingen wordt RMS uitgevoerd onder de eerste account. Als u de eerste serviceaccount wilt wijzigen, voert u de volgende handelingen uit op elke RMS-server:

1.  Als de server in een cluster is opgenomen, verwijdert u de server uit het cluster.
2.  Geef de tweede RMS-serviceaccount op als de account waaronder u RMS wilt uitvoeren. Zie '[De RMS-serviceaccount wijzigen](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)' verderop in dit onderwerp voor instructies voor het wijzigen van de account.
3.  Start IIS opnieuw op.
4.  Indien van toepassing neemt u de server weer op in het cluster.

Zodra op alle RMS-servers de tweede RMS-serviceaccount wordt gebruikt, kunt u het wachtwoord van de eerste RMS-serviceaccount wijzigen zonder dat dit invloed op de werking van het RMS-systeem heeft. Op deze manier kunt u tussen de twee accounts schakelen en downtime voor RMS voorkomen.
