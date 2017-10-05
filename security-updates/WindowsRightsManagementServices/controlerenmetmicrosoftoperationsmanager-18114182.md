---
TOCTitle: Controleren met Microsoft Operations Manager
Title: Controleren met Microsoft Operations Manager
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18114182
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747758(v=WS.10)'
---

Controleren met Microsoft Operations Manager
============================================

RMS bevat een beheerpakket dat u kunt gebruiken met Microsoft® Operations Manager (MOM). Met MOM kunt u als volgt de werking van de servers in uw organisatie beheren:

-   Gebeurtenissen controleren die door RMS in het gebeurtenislogboek voor toepassingen zijn geplaatst.
-   Gebeurtenissen markeren die mogelijk duiden op onderbrekingen van services of configuratieproblemen zodat u snel de juiste maatregelen kunt nemen.
-   Waarschuwingen en fouten melden, bijvoorbeeld wanneer het serverlicentieverleningscertificaat is verlopen of er een probleem is opgetreden met een webservice.

Het RMS-beheerpakket (RMS\_MOMPack.akm) wordt met RMS geïnstalleerd in de map %programfiles%\\Windows Rights Management Services\\Tools.

Dit beheerpakket bestaat uit de volgende regelsets, aan de hand waarvan de RMS-beheerder de implementatie van de RMS-server kan beheren.

**Regels voor RMS MOM-beheerpakketten**

1.  PMC Measure - Activation Proxy total failures
2.  PMC Measure - Activation Proxy Total time
3.  PMC Measure - Activation Total Processing Time
4.  PMC Measure - Activation Total Reqs
5.  PMC Measure - ActivationProxy total reqs
6.  PMC Measure - AD cache (DB cache) hits
7.  PMC Measure - AD cache (DB cache) misses
8.  PMC Measure - Average License Processing time
9.  Event - Configuration Info corruption
10. PMC Measure - Dead GC connections
11. PMC Measure - Enroll failures
12. Event - General Error
13. Event - Init Failure
14. Event - Licensor Cert has expired
15. Event - Licensor Cert Request Failure
16. Event - Logging service failure
17. PMC Measure - Max GC connections available
18. Event - Missing License Acq Point generation plugin
19. PMC Measure - MSMQ Queue length on all RM servers
20. Event - No GCs available
21. Event - Plugin Init Failure
22. Event - PrivateKey protection password changed
23. Event - RM Server Shut Down
24. Event - RM Server ShutDown Failure
25. Event - Server Startup Failure
26. PMC Measure - SubEnroll failures
27. Event - SuperUser privileged override power was invoked
28. PMC Threshold - Too Many GetLicensorCert failures
29. Event - Upcoming Licensor Cert Expiry - 1 Month
30. Event - Upcoming Licensor Cert expiry - 1 Week

Voor meer informatie over de implementatie van MOM-beheerpakketten in uw organisatie verwijzen wij u naar de [website van Microsoft](http://www.microsoft.com/) (http://www.microsoft.com/).
