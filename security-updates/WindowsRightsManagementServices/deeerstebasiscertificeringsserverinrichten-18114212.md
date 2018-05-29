---
TOCTitle: De eerste basiscertificeringsserver inrichten
Title: De eerste basiscertificeringsserver inrichten
ms:assetid: 'debc42f3-74ff-4c99-b7a4-4921fccdabc2'
ms:contentKeyID: 18114212
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747768(v=WS.10)'
---

De eerste basiscertificeringsserver inrichten
=============================================

Als u deze procedure wilt uitvoeren, moet u lokaal zijn aangemeld bij de beheerwebsite met een domeingebruikersaccount die lid is van de groep Administrators op de computer die u benadert. Ook leden van de groep Domeinbeheerders kunnen deze procedure uitvoeren. Als u gebruikmaakt van een externe SQL Server-database, moet deze account ook de rol van databasemaker op de SQL-server hebben. Uit veiligheidsoverwegingen kunt u het beste **Uitvoeren als** gebruiken om deze procedure uit te voeren.

Als u de pagina **Algemeen beheer** wilt openen, klikt u op **Start**, wijst u **Alle programma's** en **Windows RMS** aan en klikt u op **Windows RMS-beheer**.

Op elke server kunt u RMS slechts op één website inrichten. Als u RMS wilt inrichten op een andere website dan de standaardwebsite, gebruikt u Internet Information Services Manager om de website toe te voegen voordat u deze inrichtingsprocedure start. Als de website die u wilt inrichten niet voorkomt in de lijst met websites, sluit u de pagina **Algemeen beheer**. Voeg de website toe en begin opnieuw met de inrichtingsprocedure.

Als u RMS implementeert in een omgeving waarin het functieniveau van het Active Directory-domein de native modus van Microsoft Windows 2000 gebruikt, is RMS mogelijk niet in staat om het kenmerk **memberOf** op Active Directory-objecten te lezen bij een poging om het groepslidmaatschap uit te breiden. RMS kan het kenmerk **memberOf** alleen lezen wanneer de RMS-serviceaccount een domeinaccount gebruikt die lid is van de Pre-Windows 2000-compatibele toegangsgroep in uw forest.

Als u een aangepaste URL voor het cluster typt, registreert u deze in uw DNS (Domain Name System) en controleert u of de URL werkt. Als het een implementatie betreft waarbij internet moet zijn ingeschakeld, controleert u of de URL zowel vanaf internet als vanuit uw organisatie beschikbaar is. Als u SSL hebt ingeschakeld voor de webservicesbestanden, moet u HTTPS opgeven voor de cluster-URL.

De eerste basiscertificeringsserver inrichten
---------------------------------------------

#### De eerste basiscertificeringsserver inrichten

1.  Nadat RMS is geïnstalleerd op een server die als eerste basiscertificeringsserver moet gaan fungeren in een Active Directory-forest, opent u de pagina **Algemeen beheer**.

2.  Klik naast de website waarop u RMS wilt inrichten op **RMS op deze website inrichten**. U kunt de standaardwebsite of een andere website die u in Internet Information Services (IIS) voor dit doel hebt gemaakt, selecteren.

    | ![](/security-updates/images/Cc747768.Warning(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                    |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | De uitvoering van andere websites of diensten op dezelfde server als RMS wordt niet ondersteund. Doet u dit toch, dan zouden meerdere toepassingen en services kunnen worden uitgevoerd onder dezelfde account als RMS. Hierdoor kunnen de persoonlijke sleutels worden blootgesteld aan ontoelaatbare bewerkingen. |

3.  In het gedeelte **Configuratiedatabase** is het maken van de configuratiedatabase op de lokale server de standaardoptie. U kunt een databaseserver zoals SQL Server™ 2000 met SP3 of Microsoft SQL Server 2000 Desktop Engine (MSDE) als lokale database gebruiken. Als u een externe database gebruikt of als u een databaseserver op de lokale server hebt maar de instantie van de databaseserver een andere naam heeft dan de naam van deze server, dient u **Externe database** te selecteren en de naam van de databaseserver op te geven.

    | ![](/security-updates/images/Cc747768.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | U wordt aangeraden Microsoft SQL Server Desktop Engine alleen in testomgevingen te gebruiken ter ondersteuning van RMS-databases, omdat Microsoft SQL Server Desktop Engine geen ondersteuning biedt voor netwerkinterfaces. Bovendien wordt in de gebruiksvoorwaarden voor Microsoft SQL Server Desktop Engine aangegeven dat u hulpprogramma's voor SQL Server-clients niet kunt gebruiken voor het bewerken van een Microsoft SQL Server Desktop Engine-database. Door deze beperking kunt u geen logboekgegevens weergeven of opgeslagen gegevens in de configuratiedatabase wijzigen. |

4.  Geef in het gedeelte **RMS-serviceaccount** de RMS-serviceaccount op waaronder RMS actief moet zijn voor de meeste normale bewerkingen. Bij installatie op één server kunt u de lokale systeemaccount opgeven of een domeinaccount. Voor alle overige installaties moet u een domeinaccount opgeven. Bij een domeinaccount geeft u de accountnaam op, met de indeling *domeinnaam*\\*gebruikersnaam*, en het wachtwoord.

    | ![](/security-updates/images/Cc747768.Warning(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                        |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | De lokale systeemaccount heeft toegang tot vrijwel alle bronnen van het besturingssysteem en misbruik hiervan heeft dus ernstige gevolgen voor de beveiliging. Gebruik als het even kan dus niet de lokale systeemaccount als RMS-serviceaccount. U kunt in plaats daarvan het beste als RMS-serviceaccount een speciale domeingebruikersaccount zonder speciale machtigingen maken. Gebruik als RMS-serviceaccount niet de domeinaccount waarmee RMS is geïnstalleerd. |

    | ![](/security-updates/images/Cc747768.Important(WS.10).gif)Belangrijk                                                                                                                                                                                      |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Uit veiligheidsoverwegingen kunt u het beste een speciale domeingebruikersaccount zonder speciale machtigingen maken die wordt gebruikt als RMS-serviceaccount. Gebruik als RMS-serviceaccount niet de domeinaccount waarmee RMS met Service Pack 1 is geïnstalleerd. |

5.  Typ in het gedeelte **Cluster-URL** de URL voor de server die of voor het cluster dat voor clients wordt gebruikt in het interne netwerk. Standaard wordt hiervoor de servernaam gebruikt, bijvoorbeeld Contoso-cert. U kunt deze zo nodig bewerken, bijvoorbeeld om een URL te configureren voor het cluster of een taakverdeler die het cluster bedient. Daarnaast kunt u HTTP of HTTPS selecteren. Zie het gedeelte **Opmerkingen** aan het einde van deze procedure voor meer informatie over het configureren van een URL voor een cluster. Na het inrichten kunt u een externe cluster-URL van de beheerwebpagina's configureren zodat deze kan worden gebruikt door clients die geen toegang hebben tot het interne netwerk.

6.  Selecteer in het gedeelte **Persoonlijke-sleutelbeveiliging en inschrijving** het mechanisme ter beveiliging van de persoonlijke sleutel voor de server door een van de volgende opties te kiezen:

    -   **De standaardsoftwarebeveiliging voor persoonlijke sleutels gebruiken**. Als u deze optie selecteert, wordt de persoonlijke sleutel opgeslagen in de RMS-configuratiedatabase. U moet een sterk wachtwoord opgeven om de sleutel in de database te coderen.

    | ![](/security-updates/images/Cc747768.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                                                                                                                                                                 |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Bewaar dit wachtwoord in een veilig archief voor toekomstig gebruik. Sla een back-up van de configuratiedatabase (eveneens beveiligd met dit wachtwoord) op in het veilige archief. Zo beschikt u over een mechanisme om RMS te herstellen als de SQL Server-database beschadigd raakt. Als u het wachtwoord ooit wijzigt, maakt u een nieuwe back-up van de configuratiedatabase waarvan de sleutel aan dat wachtwoord is gekoppeld en slaat u beide op in het veilige archief. |

    -   **Gebruik een cryptografieprovider**. Als u een cryptografieprovider of een hardwarebeveiligingsmodule wilt gebruiken, schakelt u het selectievakje **De standaardsoftwarebeveiliging voor persoonlijke sleutels gebruiken** uit. Selecteer in de lijst **Selecteer de cryptografieprovider** de cryptografieprovider of hardwarebeveiligingsmodule die u hebt geïnstalleerd.

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                                                |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Voor RMS is een volledige RSA-provider (Rivest-Shamir-Adleman) vereist. Alleen dergelijke providers zijn opgenomen in de lijst met cryptografieproviders. |

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                       |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | U kunt het beste gebruikmaken van de standaardsoftwarebeveiliging voor persoonlijke sleutels of van een hardwarebeveiligingsmodule. Als u gebruikmaakt van een andere softwarecryptografieprovider, zorgt u dat in uw organisatie praktijken voor sleutelbeheer (zoals back-up- en herstelprocedures) zijn geregeld voor die cryptografieprovider voordat u deze gebruikt in combinatie met RMS. |

7.  Deze stap is alleen van toepassing als u een cryptografieprovider hebt geselecteerd. Kies een van de volgende mogelijkheden om het serversleutelpaar op te geven dat u wilt gebruiken:

    -   Voor een nieuwe installatie selecteert u **Een nieuw openbaar/persoonlijk sleutelpaar maken**.
    -   Als het gaat om herstel of een upgrade van een bestaande RMS-server, dient u **Een bestaand openbaar/persoonlijk sleutelpaar gebruiken** te selecteren. Klik onder **Bestaande sleutelcontainer** op **Bladeren** en selecteer de sleutelcontainer voor het serversleutelpaar.

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                |
    |---------------------------------------------------------------------------------------------------------------------------|
    | De Microsoft Base, Enhanced en Strong CSP's (cryptografieproviders) hebben allemaal dezelfde opslaglocatie voor sleutels. |

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Als u geen bestaand sleutelpaar hebt als u een bestaande RMS-server terugzet of een upgrade ervan uitvoert, moeten alle licentiearchieven van bestaande RMS-clients worden leeggemaakt (gebruikslicenties en rechtenaccountcertificaten worden daarbij verwijderd) en dienen zij nieuwe licenties van de server te krijgen om inhoud te kunnen verwerken. |

8.  Geef in het gedeelte over serverconnectiviteit met internet op of deze server via internet verbinding maakt om een serverlicentieverleningscertificaat op tehalen.

    -   Selecteer **On line** als u automatisch verbinding met de inschrijvingsservice van Microsoft wilt maken om tijdens het inrichtingsproces een serverlicentieverleningscertificaat te verkrijgen.
    -   Selecteer **Off line** als de RMS-server geen internetverbinding heeft of als u handmatig het serverlicentieverleningscertificaat wilt verkrijgen en dit na inrichting op de RMS-server wilt importeren.

9.  Typ bij **Naam van het serverlicentieverleningscertificaat** de naam die moet worden gebruikt in het serverlicentieverleningscertificaat. Standaard is dit de naam van de server.

10. Als uw organisatie een proxyserver gebruikt voor verbinding met internet, schakelt u het selectievakje **Deze computer maakt via een proxyserver verbinding met internet** in. Typ vervolgens het adres en de poort van de proxyserver.

    Als de proxyserver verificatie vereist, selecteert u het verificatietype en geeft u een gebruikersnaam en wachtwoord op die kunnen worden geverifieerd door de proxyserver. Gebruikt u de optie Geïntegreerde Windows-verificatie, dan moet u ook een domein opgeven.

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Deze instelling kan na inrichting worden aangepast op de pagina **Beveiligingsinstellingen** van de beheerwebsite van RMS. Deze pagina is echter niet beschikbaar tot nadat de server bij de inschrijvingsservice van Microsoft is ingeschreven. Als in uw organisatie via een proxyserver verbinding met internet wordt gemaakt en u geen proxyserver configureert omdat u **Off line** hebt geselecteerd voor **Internet-verbinding van server**, kunt u uw instellingen voor het inschrijvingsproces of de proxyserver pas wijzigen nadat u de handmatige inschrijving hebt voltooid of RMS opnieuw hebt ingericht. |

11. Typ bij **Contactgegevens van de beheerder** het e-mailadres van de beheerder waarmee contact moet worden opgenomen als zich problemen voordoen met de inrichting van andere servers. Na de inrichting kunt u dit e-mailadres wijzigen.

12. Geef bij **Intrekken** aan of u wilt toestaan dat een andere (derde) entiteit het serverlicentieverleningscertificaat van deze server kan intrekken. Als u deze optie selecteert, typt u het pad en de bestandsnaam van het openbare-sleutelbestand van de betreffende entiteit.

13. Klik op **Verzenden**.

    Door op **Verzenden** te klikken wordt de service ingericht. Als u kiest voor on line inschrijving, wordt ook de inschrijving voor de basiscertificeringsserver uitgevoerd. RMS genereert een openbaar/persoonlijk sleutelpaar en verzendt de openbare sleutel naar de inschrijvingsservice van Microsoft. De inschrijvingsservice van Microsoft maakt een serverlicentieverleningscertificaat en stuurt dit binnen enkele minuten terug naar de configuratiedatabase. Als u kiest voor off line inschrijven, moet u de taak in '[Handmatig een basiscertificeringsserver inschrijven](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643)' verderop in dit onderwerp voltooien alvorens u de RMS-server configureert.

    | ![](/security-updates/images/Cc747768.note(WS.10).gif)Opmerking                                                                                                                                                                                                                         |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Deze server kan pas worden gebruikt als het RMS-serviceverbindingspunt is geregistreerd in Active Directory. Gebruik de procedure in '[Een serviceverbindingspunt registreren](https://technet.microsoft.com/630cc3c3-9ed9-4423-8874-cbaceb43b353)' verderop in dit onderwerp als u dit wilt doen. |

Zie '[Een server toevoegen aan een cluster](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)' verderop in dit onderwerp voor instructies over het inrichten van extra basiscertificeringsservers en het toevoegen ervan aan een cluster.
