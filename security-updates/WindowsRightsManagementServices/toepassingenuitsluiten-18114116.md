---
TOCTitle: Toepassingen uitsluiten
Title: Toepassingen uitsluiten
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18114116
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747644(v=WS.10)'
---

Toepassingen uitsluiten
=======================

U kunt de versie van een toepassing met RMS-ondersteuning opgeven op basis waarvan alle licentieaanvragen moeten worden gecontroleerd. Bij de uitsluiting van een toepassing wordt in elke gebruikslicentie een voorwaarde opgenomen dat de licentie alleen van toepassing is op de door RMS beveiligde inhoud waarvoor de licentie is uitgegeven. Dit geldt niet wanneer de toepassing waarmee de licentie wordt aangevraagd, is opgenomen in de lijst met uitgesloten toepassingen.

Dit kan bijvoorbeeld nuttig zijn wanneer in een onderneming een beveiligingsupdate voor een toepassing wordt geïmplementeerd. Systeembeheerders kunnen de update op de gebruikelijke wijze installeren. Ze kunnen vervolgens een uitsluitingsbeleid voor toepassingen instellen op basis van de versiegegevens van de toepassing die gebruikmaakt van de beheerwebsite. Met dit uitsluitingsbeleid wordt voorkomen dat door RMS licenties worden uitgegeven aan clients waarop eerdere versies van de software worden uitgevoerd.

Toepassingen met RMS-ondersteuning worden uitgesloten op basis van de bestandsnaam en het versienummer. U kunt een toepassing met RM-ondersteuning uitsluiten om ervoor te zorgen dat gebruikers een nieuwere en veiligere versie van een toepassing installeren wanneer deze beschikbaar is. In uw organisatie is bijvoorbeeld versie 1.0.4.2315 van een toepassing met RMS-ondersteuning geïmplementeerd. De ontwikkelaar van de toepassing ontdekt dan een beveiligingsprobleem en deze kan dan versie 1.0.4.4200 uitgeven om het probleem te verhelpen. Wanneer u vervolgens de nieuwe versie van de toepassing implementeert, kunt u tevens voorkomen dat gebruikers nog met de vorige versie van de toepassing met beveiligde inhoud kunnen werken door een uitsluitingsbeleid in te stellen.

Zoals bij andere soorten uitsluitingen moet u de uitsluiting van een toepassing configureren in elk cluster waarvoor de uitsluiting moet gelden.

Wanneer u dit uitsluitingsbeleid toepast op de server, kunnen de uitgesloten toepassingen niet meer worden gebruikt voor het aanvragen van nieuwe gebruikslicenties en het koppelen van nieuwe licenties aan door RMS beveiligde inhoud. De uitgesloten toepassing kan nog wel worden gebruikt voor bestanden waarvoor eerder een licentie is verleend.

| ![](images/Cc747644.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                    |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| De toepassingsversie moet in RMS worden weergegeven in een viercijferige indeling met punten (\#.\#.\#.\# ). Bij sommige toepassingen wordt de versie echter weergegeven in een tweecijferige of driecijferige indeling met punten. In dat geval moet u een of twee nullen toevoegen zodat de indeling van het versienummer voldoet aan de vereisten van RMS. |
