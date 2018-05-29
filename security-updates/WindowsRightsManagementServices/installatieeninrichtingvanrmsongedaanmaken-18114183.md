---
TOCTitle: Installatie en inrichting van RMS ongedaan maken
Title: Installatie en inrichting van RMS ongedaan maken
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18114183
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747753(v=WS.10)'
---

Installatie en inrichting van RMS ongedaan maken
================================================

Mogelijk wilt u om de een of andere reden RMS van een server verwijderen. Op een basiscertificeringsserver moet u in dat geval eerst de inrichting van RMS ongedaan maken. Open de pagina **Algemeen beheer** op de server waarop u de inrichting ongedaan wilt maken en klik op **RMS van deze website verwijderen**. Op een licentieserver hoeft u de inrichting niet ongedaan te maken voordat u RMS verwijdert.

| ![](/security-updates/images/Cc747753.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wanneer u de inrichting van de laatste basiscertificeringsserver in een Active Directory-forest ongedaan maakt, wordt het object voor het serviceverbindingspunt verwijderd uit Active Directory. Als u de inrichting van RMS op deze server niet ongedaan maakt voordat u RMS verwijdert, kunt u pas een nieuwe basiscertificeringsserver in dit forest inrichten als u het object voor het serviceverbindingspunt handmatig hebt verwijderd. |

Verwijder RMS vervolgens.

Als u de inrichting en installatie van RMS ongedaan maakt op een zelfstandige server of de laatste server in een cluster, wordt ook de database met de directoryservice verwijderd. De configuratie- en logboekdatabase worden niet verwijderd. Als u RMS bijwerkt of opnieuw installeert op de server, wordt de logboekdatabase echter overschreven door een nieuwe logboekdatabase.

Wanneer u de inrichting en installatie van RMS ongedaan maakt op een server in een cluster, worden de configuratiedatabase, logboekdatabase en database met de directoryservices voor het cluster niet verwijderd. De tabel DRMS\_ClusterServer in de configuratiedatabase wordt wel bijgewerkt om aan te geven dat de server is verwijderd uit het cluster.

Zie '[Servers uit gebruik nemen](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f)' eerder in dit onderwerp voor meer informatie over het uit gebruik nemen van servers en de problemen die daarbij kunnen optreden.
