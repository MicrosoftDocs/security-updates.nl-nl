---
TOCTitle: 'Uitgifte van RMS-services'
Title: 'Uitgifte van RMS-services'
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18113887
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720247(v=WS.10)'
---

Uitgifte van RMS-services
=========================

De URL's voor RMS-services worden tijdens het inrichten van de server verleend aan Active Directory. Tijdens het inrichten voert het installatieprogramma van RMS query's uit in Active Directory om te controleren of er andere RMS-servers zijn geïnstalleerd in het forest. Als er geen andere RMS-servers zijn geïnstalleerd, wordt de server geconfigureerd als een basiscertificeringsserver. Voordat u RMS gebruikt, moet u het serviceverbindingspunt in Active Directory registreren, zodat clients de URL van de basiscertificeringsserver kunnen opsporen. Op clients waarmee verbindingen worden aangevraagd naar de services die op de basiscertificeringsserver worden uitgevoerd, wordt eerst gecontroleerd of de URL van deze basiscertificeringsserver is opgenomen in Active Directory. Zie 'Het serviceverbindingspunt registreren' in 'Een RMS-server beheren' in deze documentatie voor meer informatie.

| ![](/security-updates/images/Cc720247.note(WS.10).gif)Opmerking                                                                                                                                              |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als in uw topologie meerdere servers zijn opgenomen in een basiscertificeringscluster, leidt de URL naar de taakverdelingsserver voor het cluster. Deze server wordt tijdens het inrichten ingesteld door de beheerder. |
