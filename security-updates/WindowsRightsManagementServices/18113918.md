---
TOCTitle: Implementatie naar verschillende forests plannen
Title: Implementatie naar verschillende forests plannen
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18113918
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720233(v=WS.10)'
---

Implementatie naar verschillende forests plannen
================================================

Als u RMS implementeert in een omgeving met meerdere forests, moet u vaststellen welke ondersteuning nodig kan zijn voor gebruikers of groepen die zich buiten het forest bevinden waarbinnen RMS wordt geïmplementeerd. Het probleem is dat gebruikers- of groepsobjecten uit andere forests meestal geen vertegenwoordigende objecten hebben in het forest waarin RMS zich bevindt. Als u van plan bent RMS te gebruiken om machtigingen te beperken tot gebruikers of groepen die van andere forests komen, moet u uw forest zo configureren dat het optreden van groepsuitbreiding over forests is toegestaan.

U kunt ondersteuning voor groepsuitbreiding naar andere forests voor RMS op twee manieren implementeren:

-   Distribueer RMS naar het forest waarin de groepen zijn gedefinieerd en waar Windows RMS wordt gebruikt om het lidmaatschap van deze groepen uit te breiden.
-   Synchroniseer groepsdefinities tussen forests om de lokale RMS-installatie in staat te stellen het volledige groepslidmaatschap van iedere gebruiker vast te stellen. Als de gebruiker die een gebruikslicentie aanvraagt, een Windows-account heeft in een afzonderlijk forest, moet er tevens een contactobject in het lokale forest aanwezig zijn dat het groepslidmaatschap van die gebruiker vertegenwoordigt. U kunt meta-directoryen gebruiken, zoals Microsoft® Identity Integration Server (MIIS) 2003 of Identity Integration Feature Pack (IIFP), om volledig getrouwe synchronisatie van groepsobjecten naar forests te implementeren.

Als u van plan bent RMS alleen voor één forest te gebruiken, kunt u het proces voor het uitgeven van gebruikslicenties optimaliseren door het clusterbeleid **MaxCrossForestCalls** in de RMS-configuratiedatabase te wijzigen. In dit beleid staat aangegeven hoe vaak het lidmaatschap van een groep naar andere forests kan gaan. De standaardwaarde is 10. Met de volgende SQL-opdracht wijzigt u die waarde in 0:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`
