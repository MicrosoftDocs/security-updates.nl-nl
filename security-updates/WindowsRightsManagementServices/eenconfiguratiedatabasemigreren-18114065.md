---
TOCTitle: Een configuratiedatabase migreren
Title: Een configuratiedatabase migreren
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18114065
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747607(v=WS.10)'
---

Een configuratiedatabase migreren
=================================

Er kunnen zich omstandigheden voordoen waarin een databaseserver buiten bedrijf moet worden gesteld. Een voorbeeld is een hardware-upgrade van een RMS-databaseserver. Voordat de databaseserver buiten bedrijf wordt gesteld, moet de configuratiedatabase worden verplaatst naar een andere databaseserver. Om de gegevens in de configuratiedatabase te beschermen, met inbegrip van de daarin opgenomen sleutelparen, moet u een migratie zorgvuldig plannen en implementeren.

We raden u aan een CNAME-alias te maken voor de RMS-databaseserver en vervolgens RMS te configureren voor het gebruik van deze alias. Daarmee vervalt de noodzaak handmatig de databaseservernaam te wijzigen in de RMS-configuratiedatabase als de naam van de server wordt gewijzigd. Wanneer u een CNAME-alias gebruikt, hoeft u slechts de aliasrecord te wijzigen.

Voordat u begint met de migratie van de configuratiedatabase, moet u over de volgende informatie beschikken:

-   De accountnaam en het accountwachtwoord dat oorspronkelijk werd gebruikt om de servers in te richten in de RMS-cluster die gebruikt maakt van deze database.
-   Als een op software gebaseerde cryptografieprovider (CSP) wordt gebruikt voor het opslaan van de persoonlijke RMS-sleutel: het wachtwoord voor de persoonlijke RMS-sleutel dat oorspronkelijk werd opgegeven tijdens het inrichten. Als een hardwarebeveiligingsmodule (HSM) wordt gebruikt voor het opslaan van het wachtwoord voor de persoonlijke RMS-sleutel, hebt u deze informatie niet nodig.

| ![](/security-updates/images/Cc747607.note(WS.10).gif)Opmerking                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Voor het migreren van de configuratiedatabase is geen nieuw serverlicentieverleningscertificaat of een nieuwe persoonlijke sleutel van de server nodig omdat RMS de instellingen bewaart van de oorspronkelijke configuratiedatabase. |

U moet een back-up maken van de RMS-databases voordat u iets doet op de databaseserver. Als dat geen optie is, moet u ten minste het serverlicentieverleningscertificaat exporteren. Zie [Uw serverlicentieverleningscertificaat exporteren naar een bestand](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af) voor meer informatie over het exporteren van het serverlicentieverleningscertificaat. Als een fout optreedt tijdens het migreren van de databases, kunt u het serverlicentieverleningscertificaat importeren in een nieuwe RMS-installatie en met inhoud werken die met rechten was beveiligd in de oude installatie.

Voer de volgende stappen uit om een configuratiedatabase te migreren:

-   Werk de RMS-configuratiedatabase bij zodat deze de nieuwe databaseservernaam weergeeft.
-   Werk de web.config-bestanden en het register bij van elk van de servers in de RMS-cluster zodat die gebruikmaken van de nieuwe databaseservernaam

| ![](/security-updates/images/Cc747607.Important(WS.10).gif)Belangrijk                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| In dit onderwerp wordt ervan uitgegaan dat de RMS-databases al zijn gekopieerd naar de nieuwe databaseserver die als host fungeert voor de RMS-databases. |

Werk de RMS-configuratiedatabase bij zodat deze gebruikmaakt van de nieuwe databaseservernaam.
----------------------------------------------------------------------------------------------

De naam van de databaseserver die als host optreedt voor de RMS-databases wordt opgeslagen in de RMS-configuratiedatabase. Nadat de databasebestanden zijn gemigreerd naar de nieuwe databaseserver, moet u de RMS-configuratiedatabase bijwerken. U kunt dit doen met het hulpprogramma RMS Config Editor dat onderdeel is van de RMS Administration Toolkit of met SQL Management Studio.

Voer de onderstaande stappen uit om de RMS-databaseservernaam bij te werken met RMS Config Editor:

**De RMS-configuratiedatabase bijwerken met RMS Config Editor**
1.  Meld u aan bij een RMS-server in de cluster in de rol van lid van de systeembeheerdersdatabase.

2.  Installeer de RMS Administration Toolkit van het Microsoft Downloadcentrum ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)).

3.  Navigeer naar %SystemDrive%:\\Program Files\\RMS SP2 Administration Toolkit\\RMSConfigEditor en dubbelklik vervolgens op **RMSCONFIGEDITOR.EXE**.

4.  Voer in het vak **Server** de naam in van de nieuwe server die als host optreedt voor de RMS-configuratiedatabase en klik vervolgens op **Go**.

5.  Klik in het vak **Database** op **DRMS\_Config\_***&lt;RMS-clusternaam&gt;***\_***&lt;Poort&gt;*, waarbij *&lt;RMS-clusternaam&gt;* de naam is van de RMS-cluster en *&lt;Poort&gt;* de TCP-poort is die RMS gebruikt om te communiceren en klik vervolgens op **Go**.

6.  Klik op **DRMS\_ClusterPolicies**.

7.  Wijzig in het resultaatvenster de waarde in de kolom **PolicyData** van de rij **LoggingDatabaseServer** in de naam van de nieuwe RMS-databaseserver.

8.  Klik op **Persist**.

9.  Wijzig de waarde in de kolom **PolicyData** van de rij **CertificationUserKeyStorageConnectionString** zo dat de nieuwe databaseserver wordt weergegeven. De waarde moet zijn **data source=***&lt;naam nieuwe databaseserver&gt;***;integrated** waarbij *&lt;naam nieuwe databaseserver&gt;* de naam is van de nieuwe databaseserver.

10. Klik op **Persist**.

11. Herhaal de stappen 9 en 10 voor de waarde in de kolom **PolicyData** van de rij **DirectoryServicesCacheDatabase**.

12. Klik in het linkerdeelvenster op **DRMS\_PluginProperties**.

13. Wijzig bij **PropertyID** 101, met de naam **PERSISTENT\_STORAGE**, de kolom **PropertyValue** zo dat de nieuwe databaseserver wordt weergegeven. De waarde moet zijn **data source=***&lt;naam nieuwe databaseserver&gt;***;integrated** waarbij *&lt;naam nieuwe databaseserver&gt;* de naam is van de nieuwe databaseserver.

14. Klik op **Persist**.

15. Sluit RMS Config Editor af.

Als u de RMS-configuratiedatabase wilt bijwerken met SQL Server Management Studio, voert u de volgende stappen uit:

**De RMS-configuratiedatabase bijwerken met SQL Server Management Studio**
1.  Meld u aan bij de RMS-configuratiedatabaseserver als lokale beheerder of bij een andere gebruikersaccount die lid is van de groep lokale beheerders.

2.  Klik op **Start**, wijs **Alle programma's** aan, wijs **Microsoft SQL Server 2005** aan en klik op **SQL Server Management Studio**.

3.  Zorg ervoor dat op de pagina **Connect to Server** de naam van de nieuwe databaseserver wordt weergegeven in het vak **Server name** en klik vervolgens op **Connect**.

4.  Vouw databases uit **Databases**, vouw **DRMS\_Config\_***&lt;RMS cluster name&gt;***\_***&lt;Port&gt;* uit en vouw vervolgens **Tables** uit.

5.  Klik met de rechtermuisknop op **DRMS\_ClusterPolicies** en klik vervolgens op **Open Table**.

6.  Wijzig in het resultaatvenster de waarde in de kolom **PolicyData** van de rij **LoggingDatabaseServer** in de naam van de nieuwe RMS-databaseserver.

7.  Wijzig de waarde in de kolom **PolicyData** van de rij **CertificationUserKeyStorageConnectionString** zo dat de nieuwe databaseserver wordt weergegeven. De waarde moet zijn **data source=***&lt;naam nieuwe databaseserver&gt;***;integrated** waarbij *&lt;naam nieuwe databaseserver&gt;* de naam is van de nieuwe databaseserver.

8.  Herhaal de stappen 6 en 7 voor de waarde in de kolom **PolicyData** van de rij **DirectoryServicesCacheDatabase**.

9.  Klik met de rechtermuisknop in het deelvenster Object Explorer op **DRMS\_PluginProperties** en klik vervolgens op **Open Table**.

10. Wijzig bij **PropertyID** 101, met de naam **PERSISTENT\_STORAGE**, de kolom **PropertyValue** zo dat de nieuwe databaseserver wordt weergegeven. De waarde moet zijn **data source=***&lt;naam nieuwe databaseserver&gt;***;integrated** waarbij *&lt;naam nieuwe databaseserver&gt;* de naam is van de nieuwe databaseserver.

11. Sluit Microsoft SQL Server Management Studio af.

Configureer alle servers in de RMS-cluster zo dat deze gebruikmaken van de nieuwe databaseservernaam
----------------------------------------------------------------------------------------------------

Om elke server in de RMS-cluster gebruik te laten maken van de nieuwe databaseservernaam, moet u de web.config-bestanden en drie registervermeldingen bijwerken. Wanneer u dit hebt voltooid, moet u Internet Information Services (IIS) opnieuw starten om de wijzigingen door te voeren.

U werkt als volgt de web.config-bestanden bij op alle servers in de RMS-cluster:

**De web.config-bestanden bijwerken op alle servers in de RMS-cluster:**
1.  Meld u aan bij een server in de RMS-cluster als lid van de groep lokale Administrators.

2.  Navigeer naar %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin.

3.  Dubbelklik op **web.config**, selecteer de optie **Een programma in een lijst met geïnstalleerde programma's selecteren** en klik vervolgens op **OK**.

4.  Klik op **Kladblok**, schakel de optie **Dit type bestand altijd met dit programma openen** uit en klik vervolgens op **OK**.

5.  Klik op **Bewerken**en klik vervolgens op **Vervangen**.

6.  Voer in het vak **Zoeken naar** de naam in van de uit bedrijf te nemen databaseserver die als host fungeert voor de RMS-databases.

7.  Voer in het vak **Vervangen door** de naam in van de nieuwe databaseserver die als host gaat optreden voor de RMS-databases.

8.  Klik op **Alles vervangen** en klik vervolgens op **Annuleren**.

9.  Klik op **Bestand** en klik vervolgens op **Opslaan**.

10. Sluit Kladblok.

11. Herhaal de stappen 2 tot en met 9 voor de web.config-bestanden in de mappen %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification en %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing.

12. Herhaal de stappen 1 tot en met 11 voor elke server in de RMS-cluster.

Werk tot slot het register van elk van de servers in de RMS-cluster bij met de nieuwe databaseservernaam:

| ![](/security-updates/images/Cc747607.Caution(WS.10).gif)Waarschuwing                                                                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Het onoordeelkundig bewerken van het register kan ernstige gevolgen hebben voor uw systeem. Maak een back-up van alle belangrijke gegevens op de computer voordat u het register wijzigt. |

**Het register bijwerken van elk van de servers in de RMS-cluster**
1.  Meld u aan bij een server in de RMS-cluster als lid van de groep lokale Administrators.

2.  Klik achtereenvolgens op **Start** en **Uitvoeren**.

3.  Typ **regedit.exe** en klik op **OK**.

4.  Navigeer naar **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**.

5.  Wijzig de registervermelding PASSWORDDERIVEDKEY\_*&lt;naam oude databaseserver&gt;*\_DRMS\_CONFIG\_*&lt;naam RMS-cluster&gt;*\_*&lt;poort&gt;* in:

    PASSWORDDERIVEDKEY\_*&lt;naam nieuwe databaseserver&gt;*\_DRMS\_CONFIG\_*&lt;naam RMS-cluster&gt;*\_*&lt;poort&gt;*

    Hierbij geldt het volgende:

    -   *&lt;naam oude databaseserver&gt;* is de naam van de oude databaseserver.
    -   *&lt;naam RMS-cluster&gt;* is de naam van de RMS-cluster.
    -   *&lt;poort&gt;* is de TCP-poort die RMS gebruikt om te communiceren.
    -   *&lt;naam nieuwe databaseserver&gt;* is de naam van de nieuwe databaseserver.

6.  Navigeer naar **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;RMS cluster name&gt;\_&lt;port&gt;\\Params**.

7.  Wijzig de registervermelding **ConnectionString** zo dat de waarde van de gegevensbron overeenkomt met de naam van de nieuwe databaseserver.

8.  Herhaal stap 6 en 7 voor **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;naam RMS-cluster&gt;\_&lt;poort&gt;\\Params**.

9.  Typ **IISRESET** achter de opdrachtprompt en druk op ENTER.

10. Herhaal de stappen 1 tot en met 9 voor elke server in de RMS-cluster.
