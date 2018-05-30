---
TOCTitle: De persoonlijke sleutel van RMS wijzigen
Title: De persoonlijke sleutel van RMS wijzigen
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18114204
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747765(v=WS.10)'
---

De persoonlijke sleutel van RMS wijzigen
========================================

Tijdens het inrichten maakt RMS een persoonlijke sleutel voor de server. De persoonlijke sleutel van RMS is gecodeerd en wordt opgeslagen in de configuratiedatabase. U kunt het beste op een veilige plaats een back-up maken van de persoonlijke sleutel en deze opslaan. U kunt bovendien een hardwarebeveiligingsmodule gebruiken om de persoonlijke sleutel van RMS te beveiligen, omdat deze sleutel in het coderingsschema wordt gebruikt voor de gehele inhoud van de RMS-server. Als de beveiliging van de persoonlijke sleutel van RMS op de een of andere manier in gevaar komt, dient u de inrichting van RMS op de server ongedaan te maken en RMS vervolgens opnieuw in te richten om een nieuwe persoonlijke sleutel te krijgen.

Als de inhoud werd beveiligd door de server, dienen alle eigenaren van inhoud op de hoogte te worden gesteld en dient de inhoud opnieuw te worden gepubliceerd door de RMS-server met de nieuwe persoonlijke sleutel te gebruiken. Kopieën van inhoud die door de in gevaar gebrachte persoonlijke sleutel is beveiligd dienen te worden vernietigd, omdat deze wellicht niet voldoende zijn beveiligd.

| ![](/security-updates/images/Cc747765.Important(WS.10).gif)Belangrijk                                                                                                                                                                                                                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| De server moet het inrichtingsproces herhalen om een nieuwe persoonlijke sleutel te krijgen, ongeacht of de server staat ingeschreven bij de inschrijvingsservice van Microsoft (Microsoft Enrollment Service). Als u alleen probeert een RMS-server opnieuw in te schrijven, zal de vorige persoonlijke sleutel van RMS worden gebruikt. |
