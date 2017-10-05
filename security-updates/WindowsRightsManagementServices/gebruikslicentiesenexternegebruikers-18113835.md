---
TOCTitle: Gebruikslicenties en externe gebruikers
Title: Gebruikslicenties en externe gebruikers
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18113835
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720176(v=WS.10)'
---

Gebruikslicenties en externe gebruikers
=======================================

Met RMS kunnen auteurs beveiligde inhoud via internet delen met gemachtigde externe gebruikers. RMS biedt aan interne en externe gebruikers evenveel bescherming voor het uitgeven van inhoud, omdat voor de inhoudsrechten een licentie moet worden uitgegeven door een RMS-server. Dit stelt organisaties in staat vertrouwelijke documenten, zoals contracten, te delen via internet.

Een externe gebruiker verkrijgt doorgaans via internet toegang tot RMS. Heeft een externe gebruiker rechtstreeks toegang tot het interne netwerk, bijvoorbeeld via een VPN-verbinding, dan is hij of zij functioneel gelijkwaardig aan een interne gebruiker. Ongeacht of de gebruiker zich binnen of buiten de uitgevende organisatie bevindt, komt het proces voor het verkrijgen van een gebruikslicentie feitelijk overeen met het proces dat wordt beschreven in '[Gebruikslicentie verkrijgen](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)' eerder in dit onderwerp Voor het aanvragen van een gebruikslicentie hoeft de gebruiker zich niet in het netwerk van de auteur te bevinden of een gebruikersaccount voor het netwerk te hebben.

Hiervoor is het volgende vereist:

-   De gebruiker heeft een geldig rechtenaccountcertificaat.
-   De gebruiker heeft toegang tot de RMS-licentieserver waarmee de uitgiftelicentie is uitgegeven. Deze server kan zich op het intranet of een extranet bevinden.
-   De RMS-installatie waarmee het accountcertificaat van de gebruiker is uitgegeven, is opgenomen in de lijst met vertrouwde gebruikersdomeinen van de RMS-installatie waarmee de gebruikslicentie wordt uitgegeven.

De volgende soorten externe gebruikers kunnen gebruikslicenties verkrijgen:

-   Gebruikers met accounts die deel uitmaken van een ander Active Directory-forest waarin eveneens een RMS-installatie is opgenomen. De RMS-installatie in het andere forest moet worden ingesteld als vertrouwde gebruikersdomeinen voor deze installatie.
-   Gebruikers in een andere organisatie waarin eveneens een RMS-installatie wordt uitgevoerd en die is toegevoegd aan de lijst met vertrouwde gebruikersdomeinen voor deze installatie.
-   Gebruikers met rechtenaccountcertificaten van .NET Passport als de certificeringsservice van Microsoft RMS is opgenomen in de lijst met vertrouwde gebruikersdomeinen voor deze installatie.

U kunt een andere organisatie of een andere RMS-installatie in uw organisatie toevoegen aan de lijst met vertrouwde gebruikersdomeinen. Wanneer u een domein hebt toegevoegd, kunt u opgeven welke e-maildomeinen in dat domein moeten worden vertrouwd. Daarnaast kunt u opgeven of de beveiligings-id's (SID's) in dit domein moeten worden vertrouwd.

Uw RMS-installatie kan eveneens aan de lijst met vertrouwde gebruikersdomeinen van een andere organisatie of een andere RMS-installatie binnen uw organisatie worden toegevoegd, zodat aanvragen voor gebruikslicenties van uw gebruikers kunnen worden verwerkt.

Zie '[Vertrouwde gebruikersdomeinen](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24)' verderop in dit onderwerp en 'Vertrouwde uitgiftedomeinen toevoegen en verwijderen' in 'Een RMS-server beheren' in deze documentatie voor meer informatie over het maken van vertrouwde gebruikersdomeinen tussen RMS en andere organisaties.
