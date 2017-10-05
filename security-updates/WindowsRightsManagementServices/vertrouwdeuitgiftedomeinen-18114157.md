---
TOCTitle: Vertrouwde uitgiftedomeinen
Title: Vertrouwde uitgiftedomeinen
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18114157
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747738(v=WS.10)'
---

Vertrouwde uitgiftedomeinen
===========================

Standaard worden met RMS-servers geen gebruikslicenties verleend die zijn gebaseerd op uitgiftelicenties die worden uitgegeven met een RMS-server uit een ander cluster. In bepaalde gevallen kan één server of cluster echter niet zowel een uitgiftelicentie als een gebruikslicentie uitgeven voor bepaalde beveiligde inhoud. Dit is bijvoorbeeld het geval wanneer een bepaald RMS-cluster uit gebruik is genomen en is vervangen door een ander cluster, zoals bij een fusie van twee bedrijven kan gebeuren. In deze situatie moeten met een RMS-cluster gebruikslicenties kunnen worden verleend die zijn gebaseerd op uitgiftelicenties die met een ander RMS-cluster zijn gemaakt.

U kunt een RMS-cluster zo configureren dat deze de uitgiftelicenties vertrouwt die met een ander RMS-cluster worden uitgegeven. Daarnaast kunt u een vertrouwd uitgiftedomein implementeren zodat er gebruikslicenties kunnen worden uitgegeven die zijn gebaseerd op deze uitgiftelicenties. Hiertoe importeert u het serverlicentiecertificaat en de persoonlijke sleutel van de andere server en voegt u deze toe aan de lijst met vertrouwde uitgiftedomeinen. De persoonlijke sleutels die worden geïmporteerd, worden alleen gebruikt voor het decoderen van ondertekende uitgiftelicenties, niet voor het ondertekenen van nieuwe licenties.

Zie 'Vertrouwde uitgiftedomeinen toevoegen en verwijderen' en 'Vertrouwensbeleid inschakelen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over vertrouwde gebruikersdomeinen en stapsgewijze instructies.
