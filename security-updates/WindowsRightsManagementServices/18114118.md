---
TOCTitle: Berichtenwachtrijen controleren
Title: Berichtenwachtrijen controleren
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18114118
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc747716(v=WS.10)'
---

Berichtenwachtrijen controleren
===============================

In RMS wordt Message Queuing (ook bekend als MSMQ) gebruikt voor het versturen van gebeurtenissen naar de logboekdatabase. Vanuit elke front-endserver met RMS worden berichten naar de Message Queuing-service verstuurd en op elke front-endserver worden met de service van de logboekregistratie-listener logboekregistratieberichten opgehaald uit de Message Queuing-wachtrij en naar de logboekdatabase geschreven. Als de logboekdatabase of databaseserver niet meer beschikbaar is of als de service van de logboekregistratie-listener is beëindigd, worden de berichten in de Message Queuing-wachtrij opgeslagen. Als u de logboekdatabase of databaseserver wilt afsluiten, kunt u het beste eerst de service van de logboekregistratie-listener op elke front-endserver afsluiten. Als u de database of databaseserver weer opnieuw opstart, start u vervolgens de service van de logboekregistratie-listener op elke front-endserver opnieuw op.

Als de database niet werkt en de service van de logboekregistratie-listener nog wordt uitgevoerd, kunnen met deze service geen logboekregistratieberichten naar de database worden geschreven. De berichten worden naar een Message Queuing-wachtrij met onbestelbare berichten verplaatst tot de database beschikbaar is en er weer nieuwe logboekregistratieberichten naar de database worden geschreven. De berichten in de wachtrij met onbestelbare berichten worden niet automatisch naar de logboekdatabase geschreven. Als u de berichten in deze wachtrij wilt weergeven en verwijderen, gaat u als volgt te werk:

1.  U opent de module Computerbeheer in de MMC (Microsoft Management Console) door op **Start** te klikken, **Alle programma's** en **Systeembeheer** aan te wijzen en vervolgens op **Computerbeheer** te klikken.
2.  Klik onder Services en toepassingen in de consolestructuur op Berichten in wachtrij plaatsen en vervolgens op Persoonlijke wachtrijen.
3.  Er worden twee wachtrijen weergegeven. Beide wachtrijen hebben een naam die begint met **drms\_logging**, gevolgd door de naam van het cluster. Een van de wachtrijen heeft de naam **drms\_logging\_***&lt;uw clusternaam&gt;***\_deadletter**. Dit is de wachtrij met onbestelbare berichten. Klik op de wachtrijnaam en op de wachtrij Wachtrijberichten.
4.  Dubbelklik op elk bericht om de eigenschappen weer te geven.
5.  Als u de wachtrij wilt verwijderen, klikt u met de rechtermuisknop op de wachtrij **Wachtrijberichten** en kiest u **Alle taken** en vervolgens **Leegmaken**.

In de standaardconfiguratie worden in Message Queuing-wachtrijberichten opgeslagen tot er geen opslagruimte meer beschikbaar is op de server. Als er geen ruimte meer in Message Queuing beschikbaar is, kunnen op de RMS-server geen clientaanvragen meer worden verwerkt. Wilt u dit voorkomen, dan gaat u als volgt te werk om de hoeveelheid schijfruimte te beperken die in Message Queuing kan worden gebruikt voor wachtrijen:

1.  U opent de module Computerbeheer in de MMC (Microsoft Management Console) door op Start te klikken, Alle programma's en Systeembeheer aan te wijzen en vervolgens op Computerbeheer te klikken.
2.  Klik onder Services en toepassingen in de consolestructuur op Berichten in wachtrij plaatsen en vervolgens op Persoonlijke wachtrijen.
3.  Er worden twee wachtrijen weergegeven. Beide wachtrijen hebben een naam die begint met drms\_logging. Voer de volgende handelingen uit voor elke wachtrij:
    -   Klik op Eigenschappen.
    -   Schakel het selectievakje Maximale grootte van berichtenarchief (in kB) in en geef in kilobytes de maximale grootte voor de wachtrijberichten in de wachtrij op.

Als een wachtrij vol is, worden de berichten uit RMS bij binnenkomst verwijderd en wordt het volgende gebeurtenisbericht, dat aan gebeurtenis-id 48 is gekoppeld, naar het logboek voor systeemgebeurtenissen verstuurd:

Kan de eigenschappenverzameling niet verzenden naar Message Queuing.

U kunt de hulpprogramma's voor systeemcontrole het beste zo configureren dat u op de hoogte wordt gesteld wanneer deze gebeurtenis optreedt, omdat dit op een probleem met de logboekdatabase duidt.
