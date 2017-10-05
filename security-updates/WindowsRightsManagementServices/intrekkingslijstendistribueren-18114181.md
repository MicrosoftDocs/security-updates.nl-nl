---
TOCTitle: Intrekkingslijsten distribueren
Title: Intrekkingslijsten distribueren
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18114181
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747702(v=WS.10)'
---

Intrekkingslijsten distribueren
===============================

Als u intrekking wilt implementeren, moet u intrekkingslijsten distribueren. In intrekkingslijsten wordt opgegeven welke inhoud, toepassingen, gebruikers of andere principals zijn ingetrokken. U kunt zowel intrekkingslijsten van een organisatie als intrekkingslijsten van Microsoft distribueren.

Intrekkingslijsten van de organisatie distribueren
--------------------------------------------------

Als u een sjabloon voor het rechtenbeleid met een intrekkingslijst wilt gebruiken, moet u de intrekkingslijst beschikbaar stellen aan de clientcomputers in de organisatie. Zie 'Intrekking implementeren' eerder in dit onderwerp voor meer informatie over het maken van intrekkingslijsten.

Als u een intrekkingslijst van een organisatie wilt distribueren, gaat u als volgt te werk:

1.  Kopieer het intrekkingslijstbestand naar een algemeen toegankelijke webserver. Omdat gebruikers mogelijk buiten de organisatie met de inhoud willen werken, moet de opgegeven locatie toegankelijk zijn voor alle gebruikers, zowel via het netwerk als buiten het netwerk om.
    De distributie van het intrekkingslijstbestand naar de clientcomputers kan enige tijd in beslag nemen. Als gevolg daarvan kan het gebeuren dat een gebruiker nog niet over de intrekkingslijst beschikt wanneer deze probeert een document te openen waarvoor een intrekkingslijst vereist is. Als de intrekkingslijst niet op de clientcomputer aanwezig is, kan deze met een toepassing met RMS-ondersteuning worden gedownload vanaf de locatie die in de gebruikslicentie is opgegeven.
    U kunt het beste een script maken waarmee de intrekkingslijst elke dag automatisch wordt ondertekend en naar de website wordt gekopieerd. Zo voorkomt u dat gebruikers niet met inhoud kunnen werken omdat ze over een vervallen intrekkingslijst beschikken. Zie 'Het hulpprogramma Revocation List Signing gebruiken' voor een voorbeeldscript.
2.  Geef in de sjabloon voor het rechtenbeleid een vernieuwingsinterval voor de intrekkingslijst van de organisatie op dat groter is dan nul. Zo voorkomt u dat de intrekkingslijst optioneel is. Als u de lijst niet vaak bijwerkt, bijvoorbeeld alleen in geval van een beveiligingsprobleem, kunt u voor de vernieuwingsvoorwaarde een lang interval instellen. Vervolgens kunt u scripts maken en beleidsinstellingen opgeven waarmee de intrekkingslijst naar de clientcomputers wordt gedistribueerd wanneer dit nodig is. Zie 'Intrekkingsbeleid definiëren' eerder in dit onderwerp voor informatie over het instellen van vernieuwingsintervallen. Zie 'Sjablonen voor het rechtenbeleid maken en wijzigen' verderop in dit onderwerp voor meer informatie over het configureren van sjablonen voor het rechtenbeleid.
3.  In de sjabloon voor het rechtenbeleid geeft u de URL naar de locatie van de intrekkingslijst op.
4.  Desgewenst kunt u de intrekkingslijst naar clientcomputers distribueren via Groepsbeleid of SMS (Systems Management Server).

Intrekkingslijsten van Microsoft distribueren
---------------------------------------------

Als u wilt dat een Rights Management Services-client een intrekkingslijst van Microsoft gebruikt, dient u de lijst te distribueren naar de clientcomputers. In dit onderwerp wordt beschreven hoe u een intrekkingslijst van Microsoft in de volgende gevallen kunt distribueren:

-   Uw organisatie wil een eigen intrekkingslijst en de intrekkingslijst van Microsoft distribueren.
-   Uw organisatie wil alleen de intrekkingslijst van Microsoft distribueren.

Intrekkingslijsten van Microsoft kunt u downloaden vanaf de volgende locaties:

-   RMS-servers kunnen de intrekkingslijsten downloaden met Windows Update.
-   Als uw RMS-server geen verbinding heeft met internet, kunt u de lijst ook downloaden vanuit het Microsoft Downloadcentrum.

Als u het pakket met de intrekkingslijst naar een RMS-server downloadt, wordt het pakket opgeslagen in de map %systemdrive%\\Program Files\\Windows Rights Management Services Revocation List. Downloadt u het pakket naar een ander type computer, dan kunt u zelf opgeven waar u het pakket wilt opslaan. Het pakket bevat het bestand CRL\_Update.exe dat u kunt uitvoeren om de clientintrekkingslijsten in het clientlicentiearchief op te slaan, en het intrekkingslijstbestand Msrl.xml dat u naar een website of een algemeen gedeelde map kunt kopiëren.

**De intrekkingslijst van een organisatie en de intrekkingslijst van Microsoft distribueren**
1.  Zie de instructies in '[Intrekkingslijsten distribueren](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)' eerder in dit onderwerp als u de intrekkingslijst van een organisatie wilt distribueren.

2.  Download het pakket met de intrekkingslijst van Microsoft en distribueer het via Groepsbeleid of Systems Management Server (SMS) naar alle clientcomputers in de organisatie. U kunt ook vermeldingen van de intrekkingslijst van Microsoft naar de intrekkingslijst van de organisatie kopiëren en alleen deze laatste lijst distribueren.

| ![](images/Cc747702.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft is een principal in de vertrouwensketen voor alle certificaten en licenties die worden uitgegeven door RMS. Daarom geldt een intrekkingslijst van Microsoft voor alle koppelingsaanvragen waarvoor de gebruikslicentie is verkregen op basis van een sjabloon voor het rechtenbeleid dat de intrekkingslijst van de organisatie vereist. Daarnaast wordt de intrekkingslijst van Microsoft geregistreerd op de clientcomputer. |

**Alleen een intrekkingslijst van Microsoft distribueren**
1.  Download het pakket met de intrekkingslijst van Microsoft.

2.  Wijzig de bestaande sjablonen voor het rechtenbeleid zodat intrekking is vereist. Als er nog geen sjablonen voor het rechtenbeleid aanwezig zijn, maakt u er een en stelt u intrekking in als voorwaarde. Gebruik de openbare sleutel van Microsoft als u de intrekkingsvoorwaarde opgeeft.

3.  Geef voor het vernieuwingsinterval een waarde van 50.000 op. Zo voorkomt u dat een intrekkingslijst van Microsoft ooit verloopt. In dat geval hoeft u voor het distribueren van gebruikslicenties geen nieuwe versie van de intrekkingslijst van Microsoft te gebruiken als deze niet beschikbaar is.

4.  Kopieer het intrekkingslijstbestand naar een algemeen toegankelijke webserver. Omdat gebruikers mogelijk ook buiten de organisatie met de inhoud willen werken, moet de opgegeven locatie toegankelijk zijn voor alle gebruikers, zowel via het netwerk als buiten het netwerk om.

5.  U moet de intrekkingslijst beschikbaar stellen omdat de distributie van het intrekkingslijstbestand naar clientcomputers enige tijd in beslag kan nemen. Als gevolg daarvan kan het gebeuren dat een gebruiker lokaal nog niet over de intrekkingslijst beschikt wanneer deze probeert een document te openen met een uitgiftelicentie waarvoor een intrekkingslijst vereist is. Als de intrekkingslijst niet op de clientcomputer aanwezig is, kan deze met een toepassing met RMS-ondersteuning worden gedownload vanaf de opgegeven locatie.

6.  In de sjabloon voor het rechtenbeleid geeft u de URL naar de locatie van de intrekkingslijst op. Zie '[Sjablonen voor het rechtenbeleid maken en wijzigen](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)' verderop in dit onderwerp voor meer informatie over het configureren van sjablonen voor het rechtenbeleid.

7.  Desgewenst kunt u het pakket met de intrekkingslijst naar clientcomputers distribueren via Groepsbeleid of SMS. Gebruikers kunnen dan ook buiten het netwerk om door RMS beveiligde inhoud openen waarvoor intrekkingslijsten vereist zijn.
