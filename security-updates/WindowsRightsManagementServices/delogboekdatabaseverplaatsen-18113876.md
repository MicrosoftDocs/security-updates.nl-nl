---
TOCTitle: De logboekdatabase verplaatsen
Title: De logboekdatabase verplaatsen
ms:assetid: '34ea8045-dc94-422e-9601-29927cfc1534'
ms:contentKeyID: 18113876
ms:mtpsurl: 'https://technet.microsoft.com/nl-nl/library/Cc720238(v=WS.10)'
---

De logboekdatabase verplaatsen
==============================

Standaard wordt bij RMS de logboekdatabase op dezelfde server geïnstalleerd als de configuratiedatabase. Controleer regelmatig of in SQL Server voldoende ruimte beschikbaar is voor beide databases.

Als de logboekdatabase te groot wordt, kunt u deze op elk moment naar een andere server verplaatsen. U kunt de logboekdatabase niet verplaatsen via de beheerwebsite. U doet dit handmatig en u gaat hierbij als volgt te werk:

1.  Schakel logboekregistratie uit zoals wordt beschreven in [Logboekregistratie in- of uitschakelen](https://technet.microsoft.com/8e672f95-566f-4070-9a2a-2f70f087148f)' verderop in dit onderwerp.
2.  Kopieer de logboekdatabase met SQL Server Enterprise Manager van de bronserver naar de doelserver. Controleer of de tabellen en de opgeslagen procedures worden gemaakt in de nieuwe database. U kunt de database kopiëren met de wizard Copy Database in SQL Server Enterprise Manager.
3.  Geef de gewijzigde server- en databasenamen op in de configuratiedatabase. In de tabel DRMS\_ClusterPolicies van de configuratiedatabase voor het cluster waarvoor u de database verplaatst, doet u het volgende:
    -   Geef de nieuwe databaseservernaam op in het beleid LoggingDatabaseServer.
    -   Geef de nieuwe databasenaam op in het beleid LoggingDatabaseName.

    | ![](/security-updates/images/Cc720238.note(WS.10).gif)Opmerking                                                                                                                        |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | SQL Server Enterprise Manager is niet geschikt voor de velden db\_variant. Hiervoor kunt u Query Analyzer, dat bij SQL Server hoort, of een ander hulpprogramma voor databasebewerking gebruiken. |

4.  Start IIS opnieuw op alle servers in het cluster.
5.  Logboekregistratie opnieuw inschakelen
