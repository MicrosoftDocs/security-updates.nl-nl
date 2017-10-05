---
TOCTitle: Clients verifiëren met smartcards
Title: Clients verifiëren met smartcards
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18113999
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747579(v=WS.10)'
---

Clients verifiëren met smartcards
=================================

Als u in uw organisatie smartcards gebruikt voor een betere beveiliging en een beter beheer van gebruikersreferenties, kunt u deze smartcards nu gebruiken om rechtenaccountcertificaten te krijgen en licenties van de RMS-server te gebruiken. U moet Secure Sockets Layer (SSL) inschakelen voor de website waarvoor u RMS hebt ingericht en de verificatiemethode configureren in Internet Information Services (IIS), als u wilt dat clientverificatie vereist is voor de RMS-server. Ga hiervoor als volgt te werk:

1.  Open **Beheer van Internet Information Services**.
2.  Vouw het serveritem uit, klik met de rechtermuisknop op de websitemap en klik vervolgens op **Eigenschappen**.
3.  Klik op het tabblad **Mapbeveiliging** en selecteer vervolgens in het gedeelte **Beveiligde communicatie** het selectievakje **Toewijzingsfunctie Active Directory inschakelen**.
4.  Vouw de websitemap uit, open de virtuele map **\_wmcs** en vouw vervolgens de virtuele map (**Licensing** of **Certification**) uit waarvoor u verificatie wilt configureren.
    -   Als u verificatie wilt configureren als een gebruiker een gebruikerslicentie aanvraagt, klik dan met de rechtermuisknop op het bestand license.asmx en klik vervolgens op **Eigenschappen**.
    -   Als u verificatie wilt configureren als een gebruiker een gebruikerscertificaat aanvraagt, klik dan met de rechtermuisknop op het bestand certification.asmx en klik vervolgens op **Eigenschappen**.
5.  Klik op het tabblad **Bestandsbeveiliging** en klik vervolgens in het gedeelte **Beveiligde communicatie** op **Bewerken** om het dialoogvenster **Beveiligde communicatie** te openen.
6.  Selecteer **Beveiligd kanaal (SSL) vereisen** en klik vervolgens op een van de volgende opties:
    -   **Clientcertificaten vereisen** (als u wilt dat alleen clients met een clientcertificaat zoals een smartcard een verbinding kunnen maken met de service)
    -   **Clientcertificaten accepteren** (als u wilt dat clients verificatiereferenties kunnen opgeven met een smartcardcertificaat of met een gebruikersnaam en wachtwoord)
7.  Selecteer **Clientcertificaattoewijzing inschakelen** en klik vervolgens op **OK**.
8.  Als u clientverificatie wilt gebruiken voor zowel certificering als licentieverlening, moet u de bovenstaande procedure herhalen maar bij stap 2 de andere virtuele map selecteren.

Nadat deze instellingen zijn geconfigureerd, moet een gebruiker die door RMS beveiligde inhoud wil openen die door deze server is uitgegeven, verificatiereferenties opgeven voordat de server een rechtenaccountcertificaat of een gebruikerslicentie afgeeft.
