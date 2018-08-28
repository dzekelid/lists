---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Lists the debtor accounts by mode.
  description: Lists the debtor accounts of an accounting location by mode. The ID
    of the accounting location and the mode have to be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounting/locations/{locationId}/debtor_accounts/{mode}:
    get:
      summary: Lists the debtor accounts by mode.
      description: Lists the debtor accounts of an accounting location by mode. The
        ID of the accounting location and the mode have to be specified.
      operationId: getRestAccountingLocationsLocationDebtorAccountsMode
      x-api-path-slug: restaccountinglocationslocationiddebtor-accountsmode-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: mode
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Debtor
      - Accounts
      - By
      - Mode
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