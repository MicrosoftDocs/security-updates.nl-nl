---
TOCTitle: Rechtenaccountcertificaten uitsluiten
Title: Rechtenaccountcertificaten uitsluiten
ms:assetid: 'cba5e901-942c-4d06-9865-e6c4648c95e6'
ms:contentKeyID: 18114134
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747670(v=WS.10)'
---

Rechtenaccountcertificaten uitsluiten
=====================================

Als een gebruiker wordt vertrouwd, maar zijn of haar RMS-referenties zijn gewijzigd, kunt u het gebruikersaccountcertificaat van de gebruiker uitsluiten door de openbare sleutel van deze gebruiker uit te sluiten. Wanneer u dit doet, worden nieuwe licentieaanvragen met dit rechtenaccountcertificaat geweigerd in RMS. Hebt u een rechtenaccountcertificaat uitgesloten, dan wordt de volgende aanvraag van die gebruiker voor een gebruikslicentie voor nieuwe inhoud geweigerd. Als de gebruiker een gebruikslicentie wil aanvragen, moet deze eerst een nieuw rechtenaccountcertificaat met een nieuw sleutelpaar ophalen.

RM-accountcertificaten kunnen worden uitgesloten via de pagina **Uitsluitingsbeleid** op de beheerwebsite. Als u een rechtenaccountcertificaat van een gebruiker uitsluit, worden in RMS de uitgesloten sleutel, de accountnaam van de gebruiker en de datum en tijd van de uitsluiting toegevoegd aan de tabel DRMS\_GicExclusionList in de configuratiedatabase voor het basiscertificeringscluster. Deze gegevens worden eveneens weergegeven op de pagina **Uitsluitingsbeleid** op de beheerwebsite. Daarnaast worden de openbare en persoonlijke sleutels die aan het uitgesloten accountcertificaat zijn gekoppeld, verwijderd uit de tabel UD\_Users in de configuratiedatabase.

Als u een rechtenaccountcertificaat wilt uitsluiten dat zich op de basiscertificeringsserver of in het basiscertificeringscluster bevindt, geeft u op de pagina **Uitsluitingsbeleid** van de basiscertificeringsserver de domeinaccount van de gebruiker op. Wilt u een rechtenaccountcertificaat op alle subinschrijvingsservers uitsluiten, dan moet u dit opgeven op de beheerwebsite van elke server. Als u een gebruiker op een subinschrijvingsserver of in een subinschrijvingscluster wilt uitsluiten, geeft u op de pagina **Uitsluitingsbeleid** van de beheerwebsite van de licentieserver de waarde van de openbare sleutel voor het rechtenaccountcertificaat op. Deze waarde kan worden opgehaald op de pagina **Uitsluitingsbeleid** van de beheerwebsite van het basiscertificeringscluster.

Als u de uitsluiting van rechtenaccountcertificaten in een RMS-implementatie met meerdere clusters wilt vereenvoudigen, kunt u de tabel DRMS\_GicExclusionList vanuit de configuratiedatabase van het basiscertificeringscluster naar de configuratiedatabase van elk licentiecluster kopiëren. Wanneer u dit doet, hoeft u de waarde van de openbare sleutel niet handmatig op te geven op elke server.
