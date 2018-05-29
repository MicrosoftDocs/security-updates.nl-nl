---
TOCTitle: Softwarevereisten voor RMS
Title: Softwarevereisten voor RMS
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18113844
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720201(v=WS.10)'
---

Softwarevereisten voor RMS
==========================

In de volgende tabel staan de softwarevereisten voor RMS-servers.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Software</th>
<th style="border:1px solid black;" >Vereist</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Besturingssysteem</td>
<td style="border:1px solid black;">Elke versie van Microsoft Windows Server® 2003, behalve Web Edition.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bestandssysteem</td>
<td style="border:1px solid black;">Het NTFS-bestandssysteem wordt aanbevolen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Onderdelen van het besturingssysteem</td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (ofwel MSMQ) met Active Directory® Directory Service-integratie ingeschakeld.<br />
<br />
</li>
<li>Internet Information Services (IIS) met ASP.NET ingeschakeld.<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Active Directory®-directoryservices</td>
<td style="border:1px solid black;">RMS moet worden geïnstalleerd in een Active Directory-domein waarin alle domeincontrollers Windows 2000 met Service Pack 3 (SP3) of hoger uitvoeren. Alle gebruikers en groepen die met RMS inhoud gebruiken en publiceren, moeten over een e-mailadres beschikken dat in Active Directory is geconfigureerd.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Databaseserver</td>
<td style="border:1px solid black;">RMS vereist een database en opgeslagen procedures om bewerkingen te kunnen uitvoeren. U kunt Microsoft SQL Server 2000 met SP3a of later gebruiken, of Microsoft SQL Server 2005. Voor testdoeleinden of andere toepassingen voor één computer, kan Microsoft SQL Server Desktop Engine (MSDE 2000) met SP3 of Microsoft SQL Server 2005 Express Edition worden gebruikt.</td>
</tr>
</tbody>
</table>
  
Als u RMS implementeert in een omgeving waarin meerdere Active Directory-forests aanwezig zijn, moet u de universele groep van Active Directory gebruiken. Het groepslidmaatschap wordt dan naar alle globale catalogussen gekopieerd. Als u universele groepen wilt maken, moet het functionaliteitsniveau van het domein worden ingesteld op ten minste Windows 2000 (native modus) en het functionaliteitsniveau van het forest moet worden verhoogd tot Windows Server 2003.
  
MSDE 2000 of Microsoft SQL Server 2005 Express Edition kunt u het beste alleen gebruiken voor het ondersteunen van RMS-databases in een testomgeving, omdat netwerkinterfaces niet door MSDE 2000 of Microsoft SQL Server 2005 Express Edition worden ondersteund. Bovendien wordt in de gebruiksvoorwaarden voor MSDE 2000 of Microsoft SQL Server 2005 Express Edition aangegeven dat u hulpprogramma's voor SQL Server-clients niet kunt gebruiken voor het bewerken van een MSDE 2000- of Microsoft SQL Server 2005 Express Edition-database. Door deze beperking kunt u geen logboekgegevens weergeven of opgeslagen gegevens in de configuratiedatabase wijzigen.
  
Als ASP.NET-versie 1.1 niet op uw server is geïnstalleerd, hebben de 32-bits versie en de 64-bits versie van Windows Server 2003 elk een verschillend installatieproces.
  
Volg de volgende stappen om ASP.NET versie 1.1 te installeren en in te schakelen, als u de 32-bits versie van Windows Server 2003 uitvoert:
  
1.  Open **Software** in het **Configuratiescherm** en klik vervolgens op **Windows-onderdelen toevoegen of verwijderen**.  
2.  Klik op **Toepassingsserver** en klik vervolgens op **Details**.  
3.  Selecteer **ASP.NET** in de wizard Windows-onderdelen.  
4.  Als ASP.NET 1.1 is geïnstalleerd, maar niet wordt toegestaan als een extensie van de IIS-webservice:  
    -   Open Beheer van Internet Information Services.  
    -   Klik op **IIS Web service extension**, selecteer ASP.NET v1.1.4322 en klik vervolgens op **Toestaan**.
  
Volg de volgende stappen om ASP.NET versie 1.1 te installeren en in te schakelen, als u de 64-bits versie van Windows Server 2003 uitvoert:
  
1.  Installeer .NET Framework 1.1. Hiermee wordt gelijk ASP.NET 1.1 geïnstalleerd. U kunt het Herdistribueerbaar pakket voor .NET Framework versie 1.1 downloaden via het Microsoft Downloadcentrum ([http://go.microsoft.com/fwlink/?LinkId=69985](http://go.microsoft.com/fwlink/?linkid=69985)).  
2.  Open Beheer van Internet Information Services.  
3.  Klik op IIS Web-service-extensie, selecteer ASP.NET v1.1.4322 en klik vervolgens op Toestaan.
  
Volg om IIS te laten samenwerken met RMS de volgende stappen als u RMS uitvoert op een 64-bits versie van Windows Server 2003:
  
1.  Klik op **Start** en vervolgens op **Uitvoeren**.  
2.  Typ de volgende opdracht in het vak **Openen** en druk op ENTER:
  
**"cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
RMS is niet ontworpen voor .NET Framework versie 2.0. Hoewel een gecombineerde installatie wel wordt ondersteund, moet u ervoor zorgen dat ASP.NET geconfigureerd is voor gebruik van ASP.NET v1.1.4322. Voor een geslaagde gecombineerde installatie hebt u twee mogelijkheden:
  
-   Zorg ervoor dat u .NET Framework versie 2.0 installeert voordat u de RMS-server installeert.  
-   Zet de ASP.NET-versie terug naar versie 1.1.4322 op de standaardwebsite in IIS door de volgende opdracht uit te voeren:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Raadpleeg Help en ondersteuning van Windows Server 2003 voor meer informatie over Active Directory, Message Queuing en IIS.
  
| ![](/security-updates/images/Cc720201.Caution(WS.10).gif)Waarschuwing                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| U kunt de RMS-server inrichten op de standaardwebsite of op elke site die u eerder hebt gedefinieerd in IIS. Uit veiligheidsoverwegingen mag u deze server niet gebruiken voor het uitvoeren van andere sites of services. Doet u dit toch, dan zouden meerdere toepassingen en services kunnen worden uitgevoerd onder dezelfde account als RMS, met name de lokale systeemaccount, waardoor de persoonlijke sleutels aan ontoelaatbare bewerkingen kunnen worden blootgesteld. U kunt de RMS-server niet op dezelfde website inrichten als Microsoft Office SharePoint Server 2007. U kunt RMS niet gebruiken in combinatie met Kerberos-verificatie. Het inrichten van de RMS-server op een website schakelt Kerberos-verificatie voor die server uit. Als RMS niet is geconfigureerd voor gebruik van ASP.NET v1.1.4322, wordt er geen informatie geregistreerd in het logboekbestand. Dit leidt tot gegevensverlies. |
  
Zie ook  
-------
  
####  
  
[De infrastructuur van de databaseserver plannen](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
