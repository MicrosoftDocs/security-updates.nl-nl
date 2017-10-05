---
TOCTitle: 'De RMS-serviceaccount wijzigen'
Title: 'De RMS-serviceaccount wijzigen'
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18114210
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747736(v=WS.10)'
---

De RMS-serviceaccount wijzigen
==============================

Tijdens de installatie van RMS wordt op de lokale computer de RMS-servicegroep gemaakt en worden aan deze groep de benodigde machtigingen toegewezen voor de bronnen die vereist zijn voor RMS. Als u RMS inricht op een server, geeft u de RMS-serviceaccount op met een domeinaccount. Gebruik als RMS-serviceaccount niet de domeinaccount waarmee u RMS met Service Pack 1 hebt geïnstalleerd. Deze account wordt lid gemaakt van de RMS-servicegroep en krijgt de machtigingen toegekend die horen bij deze groep. Tijdens normale bewerkingen wordt RMS uitgevoerd onder de RMS-serviceaccount.

U kunt de RMS-serviceaccount op elk moment wijzigen. Wanneer u dit doet, wordt de vorige account automatisch uit de RMS-servicegroep verwijderd en wordt de nieuwe account toegevoegd aan deze groep.

| ![](images/Cc747736.Important(WS.10).gif)Belangrijk                                                                                                              |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uit veiligheidsoverwegingen kunt u het beste een speciale gebruikersaccount maken en deze account alleen als RMS-serviceaccount gebruiken. Stel voor deze account geen extra machtigingen in. |

| ![](images/Cc747736.note(WS.10).gif)Opmerking                                |
|-----------------------------------------------------------------------------------------------------------|
| Gebruik als RMS-serviceaccount niet de domeinaccount waarmee u RMS met Service Pack 1 hebt geïnstalleerd. |
