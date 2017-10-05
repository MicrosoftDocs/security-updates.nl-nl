---
TOCTitle: Intrekkingsbeleid definiëren
Title: Intrekkingsbeleid definiëren
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18114219
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747782(v=WS.10)'
---

Intrekkingsbeleid definiëren
============================

Het definiëren van een intrekkingsbeleid voor een organisatie vereist een zorgvuldige aanpak en een grondige planning omdat u hiermee weliswaar de beveiliging voor beveiligde inhoud kunt verbeteren, maar ook het gebruiksgemak negatief kunt beïnvloeden. Intrekkingsbeleid voor de implementatie van RMS kan worden gedefinieerd via de beheerwebsite.

Intrekking door derden
----------------------

Omdat serverlicentieverleningscertificaten voor de basiscertificeringsserver in uw RMS-implementatie worden uitgegeven met de inschrijvingsservice van Microsoft, kan Microsoft uw serverlicentieverleningscertificaat ook weer intrekken. Microsoft zal een serverlicentieverleningscertificaat echter alleen intrekken wanneer hiertoe opdracht wordt gegeven door een rechtbank.

Naast de inschrijvingsservice van Microsoft kunt u een derde partij opgeven die het serverlicentieverleningscertificaat van een RMS-server kan intrekken. Deze partij kan een externe entiteit zijn of een openbare of persoonlijke sleutel die de beheerder namens de organisatie genereert. Met de persoonlijke sleutel van de opgegeven derde partij kan een intrekkingslijst worden ondertekend waarmee het serverlicentieverleningscertificaat wordt ingetrokken. Deze derde partij wordt tijdens het inrichten van RMS opgegeven met de persoonlijke sleutel van deze partij. De sjablonen voor het rechtenbeleid van de server kunnen ook zo worden geconfigureerd dat derden inhoud, toepassingsmanifesten, licenties en certificaten kunnen intrekken die zijn uitgegeven met uw RMS-installatie. Zie '[Sjablonen voor het rechtenbeleid maken en wijzigen](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)' verderop in dit onderwerp voor meer informatie.

| ![](images/Cc747782.Important(WS.10).gif)Belangrijk                                                                                                                                        |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u een eigen sleutelpaar wilt genereren en gebruiken voor het intrekken van het serverlicentieverleningscertificaat van de basiscertificeringsserver, moet u dit sleutelpaar opslaan op een goed beveiligde locatie. |

Het intrekken van een serverlicentieverleningscertificaat is een ingrijpende maatregel omdat alle certificaten en licenties die met uw RMS-installatie zijn uitgegeven in dat geval ongeldig worden. Zie '[Serverlicentieverleningscertificaten intrekken](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)' verderop in dit onderwerp voor meer informatie over het intrekken van serverlicentieverleningscertificaten.

De effecten van intrekkingslijsten bepalen
------------------------------------------

Zodra intrekking is vereist voor bepaalde beveiligde inhoud, worden alle op clientcomputers geregistreerde intrekkingslijsten gebruikt. Als er aan de opgegeven voorwaarde wordt voldaan, wordt er ingetrokken. Ga daarom zorgvuldig te werk wanneer u intrekking implementeert omdat in dat geval intrekkingslijsten worden geregistreerd op clientcomputers en deze lijsten mogelijk breder worden toegepast dan u wilt. Zie '[Sjablonen voor het rechtenbeleid maken en wijzigen](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)' verderop in dit onderwerp voor meer informatie over het configureren van deze optie.

De balans tussen beveiliging en gebruiksgemak
---------------------------------------------

Als u een intrekkingsbeleid opgeeft in een sjabloon voor het rechtenbeleid, moet u bepalen wat u belangrijker vindt: een betere beveiliging voor documenten of een minder grote kans dat gebruikers problemen ondervinden bij het werken met inhoud. Dit probleem wordt hieronder beschreven.

Als u een intrekkingslijst instelt in een sjabloon voor het rechtenbeleid, moet u ook een vernieuwingsinterval opgeven voor de intrekkingslijst. Wanneer een gebruiker wil werken met inhoud die is uitgegeven met de sjabloon voor het rechtenbeleid, moet op de computer van de gebruiker een intrekkingslijst aanwezig zijn en mag deze lijst niet ouder zijn dan het opgegeven vernieuwingsinterval. Als het vernieuwingsinterval bijvoorbeeld op 10 is ingesteld, moet de intrekkingslijst in de laatste tien dagen zijn gemaakt. Is de intrekkingslijst niet op de clientcomputer aanwezig of ouder dan het opgegeven vernieuwingsinterval, dan kan de nieuwste intrekkingslijst met een toepassing met RMS-ondersteuning worden opgehaald van de locatie die u in de gebruikslicentie hebt opgegeven. Een gebruiker die niet op het netwerk is aangesloten, kan mogelijk geen huidige intrekkingslijst ophalen en als gevolg daarvan niet met de inhoud werken.

Gebruik de volgende suggesties om het effect van dit probleem te beperken:

-   Ga zorgvuldig te werk wanneer u het vernieuwingsinterval voor een intrekkingslijst opgeeft en zorg dat een bijgewerkte intrekkingslijst altijd eenvoudig toegankelijk is voor gebruikers.
-   Sla intrekkingslijsten op als URL's die zowel via het bedrijfsnetwerk als buiten het bedrijfsnetwerk om toegankelijk zijn.
-   Gebruik Microsoft® Systems Management Server (SMS) of een vergelijkbaar programma om bijgewerkte exemplaren van intrekkingslijsten met een bepaald interval, bijvoorbeeld elke avond, te distribueren naar de clientcomputers.
-   Vereis intrekking alleen voor de gevoeligste documenttypen.
