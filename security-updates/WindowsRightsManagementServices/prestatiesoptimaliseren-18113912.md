---
TOCTitle: Prestaties optimaliseren
Title: Prestaties optimaliseren
ms:assetid: '24dc9ca4-652b-41a6-9a99-95fdeca9120b'
ms:contentKeyID: 18113912
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720220(v=WS.10)'
---

Prestaties optimaliseren
========================

In de onderwerpen in dit gedeelte vindt u informatie over het optimaliseren van de prestaties van uw RMS-implementatie.

Prestaties van directoryservices optimaliseren
----------------------------------------------

U kunt de prestatiemeteritems voor Active Directory-services controleren die zijn opgenomen in RMS. Indien nodig kunt u de prestaties optimaliseren door in de registerinstellingen de kenmerken van de Active Directory-cache te wijzigen.

In de registerinstellingen kunt u de volgende kenmerken van de Active Directory-cache opgeven:

-   het maximumaantal principals dat in de cache kan worden opgeslagen;
-   de geldigheidsduur van de gegevens die in de cache zijn opgeslagen voor principals;
-   het maximumaantal groepen dat in de cache kan worden opgeslagen;
-   de geldigheidsduur van de gegevens die in de cache zijn opgeslagen voor groepen;
-   het maximumaantal vermeldingen van groepslidmaatschappen;
-   de geldigheidsduur van de gegevens die in de cache zijn opgeslagen voor groepslidmaatschappen.

Bij een langere geldigheidsduur voor de gegevens in de cache of bij een groot aantal vermeldingen in de cache wordt in RMS doorgaans sneller gereageerd op aanvragen voor gegevens over Active Directory-services. Als de gegevens zijn opgeslagen in de Active Directory-cache, hoeven er geen zoekopdrachten worden uitgevoerd in Active Directory. Hierdoor wordt de reactietijd voor de aanvraag verkort.

Wanneer u meer gegevens in de Active Directory-cache opslaat, zijn er echter wel meer systeemgeheugenbronnen vereist. Daarnaast is de kans groter dat sommige resultaten uit de Active Directory-cache ongeldig zijn als u in de registerinstellingen een lange geldigheidsduur opgeeft. Dit probleem kan zich voordoen wanneer gegevens worden gewijzigd in Active Directory, maar deze wijziging niet wordt doorgevoerd in de Active Directory-cache. Als Active Directory regelmatig wordt gewijzigd, kunt u beter een kortere geldigheidsduur voor de gegevens in de cache opgeven: een geldigheidsduur die overeenkomt met de regelmaat waarmee u wijzigingen doorvoert.

De prestatiemeteritems voor directoryservices worden beschreven in '[RMS: Prestatiemeteritems voor DirectoryServices](https://technet.microsoft.com/37afea1d-f320-4040-96d8-57c0b45e6d46)' verderop in dit onderwerp. Zie '[Prestatiemeteritems gebruiken](https://technet.microsoft.com/096c3b17-c082-46c4-939c-4373af0c9dec)' eerder in dit onderwerp voor instructies over het gebruik van prestatiemeteritems. De meteritems waarop u moet letten, zijn de treffers en de missers. In RMS moet voor elke misser een zoekopdracht in Active Directory worden uitgevoerd.

Zie '[Cache-instellingen voor Active Directory wijzigen](https://technet.microsoft.com/8789a7a5-2065-4fae-9104-e0a70f1f2fb6)' verderop in dit onderwerp voor meer informatie over registerinstellingen en instructies voor het wijzigen van deze instellingen.

De instellingen van de Active Directory-verbindingengroep optimaliseren
-----------------------------------------------------------------------

Als u de systeemprestaties wilt verbeteren, kunt u de registersleutels toevoegen en wijzigen waarmee de instellingen voor de LDAP-verbindingengroep (Lightweight Directory Access Protocol) van Active Directory worden bepaald. In '[Registerinstellingen voor de verbindingengroep wijzigen](https://technet.microsoft.com/c61d91db-a1ad-4ca5-a492-015da629afbc)' verderop in dit onderwerp wordt beschreven hoe u de registersleutels configureert.

RMS is ontwikkeld voor optimale LDAP-verbindingen. Hierbij wordt één verbinding tot stand gebracht voor elke globale catalogus van Active Directory en elke verbinding ondersteunt meerdere threads. Voor de stabiliteit wordt een verbindingengroep beheerd voor het verwerken van aanvragen. In RMS wordt voor de distributie van aanvragen een algoritme gebruikt om de taken te verdelen tussen de globale catalogussen die zijn opgenomen in de lijst met globale catalogussen die moeten worden doorzocht. Op deze manier wordt voorkomen dat één globale catalogus te zwaar wordt belast. Daarnaast worden LDAP-fouten automatisch verwerkt en worden aanvragen indien nodig omgeleid naar een andere globale catalogus.

In RMS wordt een lijst met globale catalogussen gemaakt die moeten worden doorzocht met de algoritme voor het opsporen van topologie. U kunt het minimum- en maximumaantal beschikbare globale catalogussen opgeven dat met deze algoritme moet worden gevonden voordat RMS-services kunnen worden gestart. Met de algoritme voor het opsporen van topologie wordt eerst naar de globale catalogussen in de huidige site gezocht. Pas als er extra globale catalogussen vereist zijn, wordt ook in andere sites gezocht. U geeft ook op bij hoeveel niet-beschikbare verbindingen in RMS geen aanvragen meer worden geaccepteerd. Als een of meer van de globale catalogussen in de zoeklijst later onbeschikbaar worden, wordt met de algoritme voor het opsporen van topologie gezocht naar vervangende globale catalogussen die aan de zoeklijst kunnen worden toegevoegd.

U kunt zelf ook een lijst maken met de globale catalogussen die in RMS moeten worden gebruikt. In dat geval wordt met de algoritme voor het opsporen van topologie niet gezocht naar globale catalogussen die aan de zoeklijst worden toegevoegd.

U kunt ook instellingen configureren voor de wijze waarop de taken worden verdeeld in de globale catalogussen. U kunt opgeven welke van de volgende drie overwegingen het belangrijkste is bij het bepalen naar welke globale catalogus een bepaalde aanvraag moet worden verstuurd:

-   **WtRoundRobin (round robin)**. Met deze parameter geeft u het relatieve belang van taakverdeling op basis van round-robinlogica op. De standaardinstelling is 1. Dit betekent dat dit de minst belangrijke overweging is bij het selecteren van een globale catalogus.
-   **WtThreadCount (aantal threads tijdens verbinding)**. Met deze parameter geeft u het relatieve belang op van het aantal threads dat wordt toegewezen aan een verbinding. De standaardinstelling is 100. Dit betekent dat het honderd keer belangrijker is dat het aantal threads van een globale catalogus voor een geselecteerde verbinding laag is dan dat er een taakverdeling is ingesteld op basis van round-robinlogica.
-   **WtSlow (langzame verbinding)**. Met deze parameter geeft u het relatieve belang van een langzame verbinding op. De standaardinstelling is 1000. Dit betekent dat het tien keer belangrijker is dat een verbinding met een globale catalogus niet langzaam is dan dat het aantal threads laag is.
