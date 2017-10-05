---
TOCTitle: Sjablonen voor het rechtenbeleid uit gebruik nemen
Title: Sjablonen voor het rechtenbeleid uit gebruik nemen
ms:assetid: '32bf98c7-edda-4507-a4b8-4c11bddd6e60'
ms:contentKeyID: 18113927
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720239(v=WS.10)'
---

Sjablonen voor het rechtenbeleid uit gebruik nemen
==================================================

Als u een sjabloon voor het rechtenbeleid uit gebruik wilt nemen, verwijdert u deze. Deze procedure wordt beschreven in '[Een sjabloon voor het rechtenbeleid verwijderen](https://technet.microsoft.com/9c9a1496-cf55-4c65-a4c6-9fe245edce00)' verderop in dit onderwerp. Doorgaans kunt u deze sjablonen echter beter niet verwijderen. Als u een sjabloon voor het rechtenbeleid uit gebruik wilt nemen, moet u ook de kopieën van deze sjabloon verwijderen van de computers van gebruikers. U moet dit doen omdat de RMS-server een aanvraag ontvangt wanneer een auteur voor het uitgeven van inhoud gebruikmaakt van een sjabloon voor het rechtenbeleid. In RMS wordt een kopie van de sjabloon die in de database is opgeslagen, gebruikt om de aanvraag te beantwoorden. Als de sjabloon niet in de database aanwezig is, mislukt de aanvraag.

| ![](images/Cc720239.note(WS.10).gif)Opmerking                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wanneer u een sjabloon voor het rechtenbeleid uit gebruik neemt, kunt u een script maken om deze sjabloon te verwijderen van alle gebruikerscomputers. |
