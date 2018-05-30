---
TOCTitle: Machtigingen voor virtuele mappen instellen
Title: Machtigingen voor virtuele mappen instellen
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18113964
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747549(v=WS.10)'
---

Machtigingen voor virtuele mappen instellen
===========================================

Nadat het uit bedrijf nemen is ingeschakeld, is deze optie als een service beschikbaar. De service Uit bedrijf nemen is een virtuele map in IIS met bijbehorende toegangsmachtigingen. Gebruikers kunnen deze service gebruiken als u machtigingen voor de virtuele map en het bestand decommission.asmx instelt.

Standaard is de optie Geïntegreerde Windows-verificatie ingeschakeld voor de virtuele map, maar alleen systeem- en beheerdersaccounts hebben toegang tot het eigenlijke bestand. Wanneer u de machtigingen voor de DACL van het bestand decommission.asmx opgeeft, kunt u toegang verlenen aan een bepaalde groep gebruikers die de eigenlijke RMS-beveiliging mogen verwijderen, of iedereen toegang tot de service verlenen.

Voordat gebruikers de service Uit bedrijf nemen kunnen gebruiken, moet eerst de toepassing van de gebruikers worden aangepast, zodat aanvragen voor een gebruikslicentie naar de nieuwe pipeline voor uit bedrijf nemen kunnen worden gestuurd. Voor Microsoft Office System 2003 wordt dit gedaan door een vermelding aan het register op de computer van de gebruiker toe te voegen. Als u met Office 2003 werkt, kunt u deze stap als volgt uitvoeren:

1.  Open de Register-editor.
2.  Ga naar `HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM` en voeg een sleutel genaamd `Uit bedrijf nemen` toe.
3.  Voeg onder de sleutel Uit bedrijf nemen de volgende nieuwe vermelding **Tekenreekswaarde** toe en vervang *uw licentieserver* door de naam van uw RMS-server:
    `http://`*uw licentieserver*`/_wmcs/licensing`
4.  Klik vervolgens met de rechtermuisknop op de vermelding, selecteer **Wijzigen** en geef de waarde op die verwijst naar de service Uit bedrijf nemen:
    `http://`*uw licentieserver*`/_wmcs/decommission`

| ![](/security-updates/images/Cc747549.note(WS.10).gif)Opmerking                                                                           |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| Onder deze sleutel kunnen meerdere vermeldingen staan als er zich meerdere RMS-servers binnen de organisatie in de modus Uit bedrijf nemen bevinden. |
