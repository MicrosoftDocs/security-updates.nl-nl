---
TOCTitle: 'Stap 5: Automatische updates configureren'
Title: 'Stap 5: Automatische updates configureren'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18126817
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720532(v=WS.10)'
---

Stap 5: Automatische updates configureren
=========================================

Op WSUS-clientcomputers moet een compatibele versie van Automatische updates aanwezig zijn. Het installatieprogramma van WSUS configureert IIS automatisch om de meest recente versie van Automatische updates te installeren op elke clientcomputer die verbinding maakt met de WSUS-server.

Wat de beste manier is om Automatische updates te configureren, hangt af van uw netwerkomgeving. In een Active Directory-omgeving kunt u een groepsbeleidsobject in een domein gebruiken. In een omgeving zonder Active Directory kunt u het lokale groepsbeleidsobject gebruiken. Maar of u nu gebruikmaakt van het lokale groepsbeleidsobject of van een groepsbeleidsobject in een domein, u moet de clientcomputers naar de WSUS-server verwijzen en vervolgens Automatische updates configureren.

Bij de volgende instructies wordt aangenomen dat op uw netwerk Active Directory wordt uitgevoerd. Ook wordt aangenomen dat u weet hoe u met groepsbeleid moet werken en groepsbeleid gebruikt voor het beheer van uw netwerk. U moet een nieuw groepsbeleidsobject maken voor WSUS-instellingen en dit groepsbeleidsobject koppelen aan het domein.

Zie de website over groepsbeleid op [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375) voor meer informatie over groepsbeleid.

**Stap 5 omvat de volgende procedures**:

-   De WSUS-beheersjabloon toevoegen
-   Automatische updates configureren
-   De clientcomputer naar de WSUS-server verwijzen
-   Detectie door de WSUS-server handmatig starten

Voer de eerste drie procedures uit voor een groepsbeleidobject in een domein. U moet een nieuw groepsbeleidobject maken of een bestaand groepsbeleidobject gebruiken. Als u GPMC (Group Policy Management Console) voor het beheren van uw groepsbeleidobjecten gebruikt, gaat u naar het groepsbeleidobject dat u wilt wijzigen en klikt u op **Bewerken**.

Om de beleidsinstellingen voor het beheren van WSUS te kunnen zien, moet u ervoor zorgen dat de WSUS-beheersjabloon, wuau.adm, wordt toegevoegd aan de Groepsbeleidsobjecteditor. Aangezien wuau.adm standaard via het besturingssysteem wordt doorgeven, zou het al in de Groepsbeleidsobjecteditor aanwezig moeten zijn.

**De WSUS-beheersjabloon toevoegen**
1.  Klik in de Groepsbeleidsobjecteditor op een van de knooppunten bij **Beheersjablonen**.

2.  Klik in het menu **Actie** op **Sjablonen toevoegen/verwijderen** en klik op **Toevoegen**.

3.  Klik in het dialoogvenster **Beleidssjablonen** op **wuau.adm** en klik vervolgens op **Openen**.

4.  Klik in het dialoogvenster **Sjablonen toevoegen/verwijderen** op **Sluiten**.

**Automatische updates configureren**
1.  Vouw in de Groepsbeleidsobjecteditor achtereenvolgens **Computerconfiguratie**, **Beheersjablonen** en **Windows-onderdelen** uit en klik op **Windows Update**.

2.  Dubbelklik in het detailvenster op **Automatische updates configureren**.

3.  Klik op **Ingeschakeld** en klik vervolgens op een van de volgende opties:

    -   **Downloaden en installeren melden**: Als u deze optie selecteert, krijgt een lid van de groep Administrators dat zich heeft aangemeld, een melding voordat de updates worden gedownload of geïnstalleerd.
    -   **Automatisch en installeren melden**: Als u deze optie selecteert, worden de updates automatisch gedownload en krijgt vervolgens een lid van de groep Administrators dat zich heeft aangemeld, een melding voordat de updates worden geïnstalleerd.
    -   **Automatisch en installatie plannen**: Als Automatische updates is geconfigureerd om een geplande installatie uit te voeren, moet u ook de dag en het tijdstip voor de terugkerende geplande installatie opgeven.
    -   **Locale beheerder toestaan om instelling te kiezen**: Als u deze optie selecteert, kunnen lokale beheerders het item Automatische updates in het Configuratiescherm gebruiken om zelf een optie voor de configuratie te selecteren. Ze kunnen bijvoorbeeld voor de terugkerende geplande installatie een tijdstip kiezen dat hun het beste uitkomt. Het is lokale beheerders niet toegestaan Automatische updates uit te schakelen.

4.  Klik op **OK**.

| ![](/security-updates/images/Cc720532.note(WS.10).gif)Opmerking                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| De optie **Locale beheerder toestaan om instelling te kiezen** wordt alleen weergegeven als Automatische updates zichzelf heeft bijgewerkt naar de versie die compatibel is met WSUS. |

**De clientcomputer naar de WSUS-server verwijzen**
1.  Vouw in de Groepsbeleidsobjecteditor achtereenvolgens **Computerconfiguratie**, **Beheersjablonen** en **Windows-onderdelen** uit en klik op **Windows Update**.

2.  Dubbelklik in het detailvenster op **Locatie van Microsoft-updateservice in intranet**.

3.  Klik op **Ingeschakeld** en typ zowel in het vak **Stel de updateservice in het intranet in voor het detecteren van updates** als in het vak **Intranetserver voor statistische gegevens** de HTTP-URL van dezelfde WSUS-server. Typ bijvoorbeeld *http://servernaam* in beide vakken en klik op **OK**.

| ![](/security-updates/images/Cc720532.note(WS.10).gif)Opmerking                                                                                                                                                                                                                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u het lokale groepsbeleidsobject gebruikt om deze computer naar de WSUS-server te verwijzen, wordt deze instelling onmiddellijk van kracht en wordt deze computer na korte tijd in de WSUS-beheerconsole weergegeven. U kunt dit proces nog versnellen door handmatig een detectiecyclus te starten. |

Nadat u een clientcomputer hebt geconfigureerd, duurt het enkele minuten voordat deze computer op de pagina **Computers** in de WSUS-console wordt weergegeven. Voor clientcomputers die zijn geconfigureerd met een groepsbeleidsobject in een domein, is dat ongeveer 20 minuten nadat het groepsbeleid is vernieuwd (dat wil zeggen, nadat de nieuwe beleidsinstellingen op de clientcomputer zijn geconfigureerd). Het groepsbeleid wordt standaard elke 90 minuten (met een marge van 0 tot -30 minuten) op de achtergrond vernieuwd. Als u het groepsbeleid eerder wilt vernieuwen, geeft u op de clientcomputer de opdrachtprompt weer en typt u de volgende tekst: **gpupdate /force**.

Voor clientcomputers die zijn geconfigureerd met het lokale groepsbeleidsobject, wordt groepsbeleid onmiddellijk toegepast en duurt het vernieuwen ongeveer 20 minuten.

Als het groepsbeleid eenmaal is toegepast, kunt u het detecteren handmatig starten. Als u het detecteren handmatig start, hoeft u niet 20 minuten te wachten voordat de clientcomputer verbinding maakt met de WSUS-server.

**Detectie door de WSUS-server handmatig starten**
1.  Klik op de clientcomputer op **Start** en klik op **Uitvoeren**.

2.  Typ **cmd** in het vak **Openen** en klik op **OK**.

3.  Typ **wuauclt.exe /detectnow** achter de opdrachtprompt. Met deze opdrachtregeloptie geeft u Automatische updates de opdracht onmiddellijk verbinding te maken met de WSUS-server.
