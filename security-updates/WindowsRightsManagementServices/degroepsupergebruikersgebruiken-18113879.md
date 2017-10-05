---
TOCTitle: De groep supergebruikers gebruiken
Title: De groep supergebruikers gebruiken
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18113879
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720198(v=WS.10)'
---

De groep supergebruikers gebruiken
==================================

Tijdens het inrichten van RMS wordt de speciale groep supergebruikers gemaakt. Leden van deze groep hebben volledig beheer over de door RMS beveiligde inhoud. Aan de leden van de groep supergebruikers worden volledige eigenaarsrechten toegewezen voor alle gebruikslicenties die worden uitgegeven door de RMS-server of het RMS-cluster waarvoor de groep supergebruikers is geconfigureerd. Dit betekent dat leden van deze groep alle beveiligde inhoudsbestanden kunnen decoderen en de beveiliging kunnen opheffen. Een lid van deze groep kan bijvoorbeeld de beveiliging opheffen voor bestanden die zijn uitgegeven door een ontslagen medewerker, zodat een nieuwe eigenaar de bestanden kan uitgeven en beheren.

De groep supergebruikers heeft standaard geen leden; zelfs beheerders zijn niet automatisch lid. Als u de beheerwebsite gebruikt, kunt u een Active Directory-beveiligingsgroep opgeven als de groep supergebruikers voor RMS. U kunt hiervoor een bestaande Active Directory-groep gebruiken of een nieuwe groep maken. De groep moet zich in hetzelfde Active Directory-forest bevinden als de RMS-installatie. De gebruikersaccounts die deel uitmaken van de groep die u opgeeft als de groep supergebruikers voor RMS, krijgen automatisch de rechten van de groep supergebruikers toegewezen.

Zie '[Een groep supergebruikers instellen](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)' verderop in dit onderwerp voor meer informatie over het opgeven van een groep supergebruikers voor RMS.

| ![](images/Cc720198.note(WS.10).gif)Opmerking                                                                                                                                                                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Als u een groep wilt aanwijzen als de groep supergebruikers voor RMS, moet deze groep aanwezig zijn in hetzelfde Active Directory-forest als de RMS-installatie. In de eigenschappen van deze groep moet een e-mailadres zijn opgenomen met een FQDN-naam (Fully Qualified Domain Name) die overeenkomt met de accountnaam. Het e-mailadres moet de notatie *groepsnaam*@*domeinnaam* hebben. |
