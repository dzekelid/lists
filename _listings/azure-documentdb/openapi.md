swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 1
info:
  title: DocumentDB
  description: azure-documentdb-database-service-resource-provider-rest-api
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.DocumentDB/databaseAccounts:
    get:
      summary: Database Accounts List
      description: Lists all the Azure DocumentDB database accounts available under
        the subscription.
      operationId: DatabaseAccounts_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-documentdbdatabaseaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listKeys
  : post:
      summary: Database Accounts List Keys
      description: Lists the access keys for the specified Azure DocumentDB database
        account.
      operationId: DatabaseAccounts_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamelistkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
      - Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/listConnectionStrings
  : post:
      summary: Database Accounts List Connection Strings
      description: Lists the connection strings for the specified Azure DocumentDB
        database account.
      operationId: DatabaseAccounts_ListConnectionStrings
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamelistconnectionstrings-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
      - Connection
      - Strings
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/readonlykeys
  : get:
      summary: Database Accounts List Read Only Keys
      description: Lists the read-only access keys for the specified Azure DocumentDB
        database account.
      operationId: DatabaseAccounts_ListReadOnlyKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccountsaccountnamereadonlykeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - List
      - Read
      - Only
      - Keys