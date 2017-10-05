---
TOCTitle: Vereisten voor sleutelbeheer definiëren
Title: Vereisten voor sleutelbeheer definiëren
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18114236
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747797(v=WS.10)'
---

Vereisten voor sleutelbeheer definiëren
=======================================

In RMS worden cryptografiesleutels gebruikt voor inhoudsbeveiliging en rechtenbeheer. Deze sleutels bevatten de essentiële informatie die het systeem in staat stelt naadloos en veilig te werken. Beheerders moeten deze sleutels zorgvuldig beveiligen tegen gegevensverlies, systeemfouten en diefstal.

In de standaardconfiguratie van RMS worden het serversleutelpaar en de bijbehorende GUID opgeslagen in een tabel in de configuratiedatabase. Het serversleutelpaar is gecodeerd door het wachtwoord dat u tijdens de inrichting hebt geselecteerd.

Als u het serversleutelpaar en de GUID wilt beveiligen, slaat u een back-up van de configuratiedatabase op een opslagmedium op (zoals een cd-rom) en bewaart u het medium op een veilige locatie (bijvoorbeeld in een kluis op een andere locatie). Hoe vaak u back-ups moet maken, is afhankelijk van de frequentie waarmee u wijzigingen in de beheerinstellingen doorvoert en het acceptabele risiconiveau voor gegevensverlies als gevolg van mediumbeschadiging of andere risico's. Onthoud wel het wachtwoord van de persoonlijke sleutel dat bij het maken van een back-up van de configuratiedatabase is gebruikt. Zonder dat wachtwoord zult u de back-up niet naar de RMS-server kunnen herstellen.

Als u SQL Server als databaseserver gebruikt, kunt u met SQL Server Enterprise Manager de waarde van de gecodeerde persoonlijke-sleutelgegevens en GUID rechtstreeks naar een beveiligde diskette of een ander medium kopiëren. Omdat de persoonlijke sleutel is beveiligd, moet de RMS-installatie onder dezelfde RMS-serviceaccount als de back-up worden uitgevoerd als u de RMS-installatie hiermee wilt herstellen.

Als u de persoonlijke sleutel van de server beveiligt met een software- of hardwarecryptografieprovider, moet u handmatig een back-up van de sleutelcontainer en sleutel maken. Het gebruik van een HSM komt de beveiliging van persoonlijke sleutels ten goede omdat ze in dat geval in hardware worden opgeslagen en nooit in aanraking komen met software. Gegevens die moeten worden gedecodeerd of ondertekend, worden naar de HSM gestuurd en weer gedecodeerd of ondertekend teruggestuurd.

Voor elke cryptografieprovider (software of hardware) zijn er specifieke procedures voor het veilig maken van een back-up van de sleutel. Raadpleeg indien nodig de documentatie van de cryptografieprovider voor meer informatie over de te volgen procedure.
