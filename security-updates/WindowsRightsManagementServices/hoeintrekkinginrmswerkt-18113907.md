---
TOCTitle: Hoe intrekking in RMS werkt
Title: Hoe intrekking in RMS werkt
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18113907
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720263(v=WS.10)'
---

Hoe intrekking in RMS werkt
===========================

Bij intrekking wordt voorkomen dat een ingetrokken entiteit die is opgenomen in de bindingsaanvraag wordt gebonden, waardoor de gebruiker niet in staat is met de inhoud te werken. Intrekking wordt geïmplementeerd via intrekkingslijsten die worden gedistribueerd naar clientcomputers. Deze lijsten zijn ondertekende XrML-bestanden waarin wordt opgegeven welke inhoud, toepassingen, gebruikers of andere principals zijn ingetrokken door de principal die de lijst uitgeeft.

Telkens als een gebruiker probeert te werken met beveiligde inhoud, wordt vanuit de bijbehorende toepassing met RMS-ondersteuning in een bindingsaanvraag een aanvraag voor de benodigde rechten naar de RMS-client verstuurd. Wanneer de gebruiker bijvoorbeeld een bestand probeert te openen, wordt vanuit de toepassing een weergaverecht aangevraagd waarmee het bestand kan worden geopend. Als de gebruiker het bestand probeert te bewerken, wordt er een bewerkingsrecht aangevraagd.

Tijdens het verwerken van een bindingsaanvraag worden in de RMS-client de volgende stappen uitgevoerd:

1.  De gebruikslicentie wordt gecontroleerd op vereisten voor intrekkingslijsten.
2.  Als de gebruikslicentie intrekking vereist, wordt in het clientonderdeel op basis van het opgegeven vernieuwingsinterval in de gebruikslicentie gecontroleerd of de opgegeven intrekkingslijst aanwezig, geregistreerd en bijgewerkt is.
3.  Er wordt gecontroleerd of de principal waarmee de intrekkingslijst is ondertekend, in de gebruikslicentie is opgegeven als een principal waarmee de licentie kan worden ingetrokken.
4.  Als deze controles zijn voltooid, wordt in het clientonderdeel vastgesteld of de oorspronkelijke bindingsaanvraag principals bevat die zijn ingetrokken. Is dit het geval, dan wordt de bindingsaanvraag geweigerd.

Intrekkingslijsten kunnen door de beheerder naar clientcomputers worden gedistribueerd of met een toepassing met RMS-ondersteuning naar de computer worden gedownload als de gebruikslicentie dit vereist. Wanneer een intrekkingslijst wordt gebruikt voor het binden van inhoud, wordt deze geregistreerd. Zolang de toepassing geopend blijft, kan deze lijst ook worden gebruikt voor bindingsaanvragen met andere gebruikslicenties. Als de toepassing wordt gesloten, wordt de registratie van de intrekkingslijst ongedaan gemaakt.

In het volgende schema wordt het bindingsproces weergegeven en wordt aangegeven welke rol intrekking in dit proces speelt.

![](images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

Intrekking is optioneel. De RMS-beheerder kan intrekking vereisen door dit op te geven in een of meer sjablonen voor het rechtenbeleid van de organisatie. Als intrekking vereist is, kan een licentie alleen worden gebonden als de vereiste intrekkingslijst aanwezig is, op de computer van de gebruiker is geregistreerd en niet ouder is dan het vernieuwingsinterval dat is opgegeven in de gebruikslicentie.

Intrekking kan echter nog altijd worden uitgevoerd voor bepaalde gebruikslicenties, zelfs wanneer intrekking voor deze licenties niet vereist is. Intrekking wordt uitgevoerd wanneer een uitgever van een certificaat uit een vertrouwensketen die is opgenomen in een bindingsaanvraag, een intrekkingslijst heeft uitgegeven die is geregistreerd op een clientcomputer. In dat geval wordt de intrekkingslijst gebruikt voor het verwerken van koppelingsaanvragen, zelfs wanneer de gebruikte gebruikslicenties geen intrekking vereisen. Als u de toepassing met RMS-ondersteuning sluit, wordt de registratie van de intrekkingslijst ongedaan gemaakt en wordt de intrekkingslijst niet meer gebruikt voor het verwerken van koppelingsaanvragen.

Wanneer een gebruiker bijvoorbeeld probeert te werken met inhoud waarvoor volgens de gebruikslicentie, uitgegeven door entiteit A, een intrekkingslijst vereist is die is uitgegeven door entiteit A, wordt de intrekkingslijst in de toepassing met RMS-ondersteuning opgehaald van de URL die is opgegeven in de gebruikslicentie. Vervolgens wordt de intrekkingslijst geregistreerd. Tijdens het verwerken van de bindingsaanvraag wordt de intrekkingslijst in de RMS-client gecontroleerd op eventuele intrekkingen.

Vervolgens houdt de gebruiker de toepassing met RMS-ondersteuning geopend en probeert te werken met andere inhoud die eveneens is uitgegeven door entiteit A. In dat geval wordt, hoewel in de gebruikslicentie geen intrekkingsvoorwaarde is opgenomen, de intrekkingslijst van entiteit A geregistreerd op de computer van de gebruiker. In het clientonderdeel wordt de intrekkingslijst gecontroleerd voordat de bindingsaanvraag wordt verwerkt.

Vervolgens probeert de gebruiker met inhoud te werken waarvoor de gebruikslicentie is uitgegeven door entiteit C. In de gebruikslicentie is geen intrekkingslijst opgenomen. Omdat de enige geregistreerde intrekkingslijst op de computer de door entiteit A uitgegeven intrekkingslijst is en entiteit A niet in de vertrouwensketen voor de gebruikslicentie is opgenomen, is intrekking niet van toepassing op de koppeling.

Ten slotte sluit de gebruiker de toepassing met RMS-ondersteuning en opent deze de andere inhoud waarop geen intrekkingsvoorwaarde van toepassing is. Omdat de registratie van de door entiteit A uitgegeven intrekkingslijst ongedaan is gemaakt toen de toepassing werd gesloten, wordt de intrekkingslijst in de RMS-client niet gecontroleerd bij de verwerking van de bindingsaanvraag.
