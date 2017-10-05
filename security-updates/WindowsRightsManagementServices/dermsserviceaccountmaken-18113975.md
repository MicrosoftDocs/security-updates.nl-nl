---
TOCTitle: 'De RMS-serviceaccount maken'
Title: 'De RMS-serviceaccount maken'
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18113975
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747546(v=WS.10)'
---

De RMS-serviceaccount maken
===========================

Tijdens de installatie van RMS wordt op de lokale computer een beveiligingsgroep, de **RMS-servicegroep** genaamd, gemaakt en worden voor deze groep de benodigde machtigingen ingesteld voor de vereiste bronnen voor RMS.

Als u RMS op een server inricht, geeft u een gebruikersaccount op die moet worden gebruikt als de RMS-serviceaccount. Deze account wordt lid gemaakt van de RMS-servicegroep en aan de account worden de machtigingen toegewezen die horen bij deze groep. Tijdens normale bewerkingen wordt RMS in de meeste gevallen uitgevoerd onder de RMS-serviceaccount.

| ![](images/Cc747546.note(WS.10).gif)Opmerking         |
|------------------------------------------------------------------------------------|
| Gebruik als RMS-serviceaccount niet de domeinaccount waarmee RMS is geïnstalleerd. |

Uit veiligheidsoverwegingen kunt u het beste een speciale gebruikersaccount maken en deze account alleen als RMS-serviceaccount gebruiken. Stel voor deze account geen extra machtigingen in.

| ![](images/Cc747546.Important(WS.10).gif)Belangrijk   |
|------------------------------------------------------------------------------------|
| U moet deze speciale gebruikersaccount maken voordat u RMS installeert en inricht. |

Zie 'Beveiligingsmodel van RMS' in 'Technische referentie van RMS' in deze documentatie voor meer informatie over de machtigingen die worden toegekend aan de RMS-servicegroep en de accounts waaronder RMS wordt uitgevoerd.
