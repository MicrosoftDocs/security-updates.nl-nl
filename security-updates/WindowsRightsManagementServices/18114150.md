---
TOCTitle: 'RMS-server installeren vanaf de opdrachtregel'
Title: 'RMS-server installeren vanaf de opdrachtregel'
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18114150
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747733(v=WS.10)'
---

RMS-server installeren vanaf de opdrachtregel
=============================================

U kunt via een opdrachtprompt RMS Service Pack 2 (SP2) automatisch installeren. U kunt de installatie op twee verschillende manieren automatiseren: een installatie zonder toezicht uitvoeren met behulp van de EXE-client die u hebt gedownload of de uitgepakte MSI-bestanden uit de gedownloade EXE gebruiken om de RMS-client te installeren. Als u de installatie wilt uitvoeren met behulp van het EXE-bestand dat u hebt gedownload, gebruikt u de volgende syntax:

**WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Als u de installatie wilt uitvoeren met de Windows® Installer-bestanden (.msi), pakt u eerst de msi-bestanden van het uitvoerbare bestand RMS SP2 uit. Voor het uitpakken van de bestanden msdrmclient.msi en RmClientBackCompat.msi kunt u via de opdrachtprompt de volgende opdracht uitvoeren:

**WindowsRightsManagementServiceSP2-KB917275-Server-ENU.exe /X:C:\\***Installatielocatie*

Nadat de .msi-bestanden zijn uitgepakt, kunt u via de volgende opdrachten RMS installeren:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Installatielocatie*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Installatielocatie*

In de volgende tabel wordt de syntaxis van elke opdracht beschreven.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parameter</th>
<th style="border:1px solid black;" >Definitie</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/I MSDrmClient.msi</strong> of <strong>/I RMClientBackCompat.msi</strong></td>
<td style="border:1px solid black;">Vereist. Geeft het product aan dat wordt geïnstalleerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/qn</strong></td>
<td style="border:1px solid black;">Optioneel. Geeft een stille installatie zonder gebruikerinteracties aan.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/lei</strong> <em>logboekbestand.log</em></td>
<td style="border:1px solid black;">Optioneel. Geeft het bestand aan waarin fout- en statusberichten worden geregistreerd.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>DISPLAYPAGE=&quot;NEE&quot;</strong></td>
<td style="border:1px solid black;">Optioneel. Geeft aan dat de pagina <strong>Algemene beheer</strong> niet wordt weergegeven na de installatie.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>TARGETDIR=c:\</strong><em>Installatielocatie</em></td>
<td style="border:1px solid black;">Optioneel. Geeft aan in welke map RMS met Service Pack 2 moet worden geïnstalleerd. Als u geen speciale locatie opgeeft, wordt de standaardinstallatielocatie gebruikt.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747733.note(WS.10).gif)Opmerking                                                                                                                                                                                                                   |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| U moet er altijd voor zorgen dat de twee MSI-bestanden goed zijn geïnstalleerd, ongeacht de installatiemethode die u gebruikt. Als er zich een fout voordoet waardoor het bestand MSDrmClient.msi niet kan worden geïnstalleerd, moet u het bestand RMClientBackCompat.msi niet installeren. |
