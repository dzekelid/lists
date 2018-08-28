---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 0
info:
  title: Azure DocumentDB API Database Accounts List Read Only Keys
  description: Lists the read-only access keys for the specified Azure DocumentDB
    database account.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---