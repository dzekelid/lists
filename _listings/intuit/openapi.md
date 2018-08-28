swagger: "2.0"
x-collection-name: Intuit
x-complete: 1
info:
  title: QuickBooks Online V3 API
  description: the-quickbooks-online-accounting-api-is-a-restful-api-that-is-used-to-access-quickbooks-companies-docs-
  version: 1.0.0
host: DefaultParameterValue
basePath: /v3/company/DefaultParameterValue
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/AccountList:
    get:
      summary: Get Reports Account List
      description: |-
        Report - Account list detail
        Method : GET

        The information below provides a reference on how to access the account list detail report from the QuickBooks Online Report Service.
      operationId: getReportsAccountlist
      x-api-path-slug: reportsaccountlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Account
      - List
  /reports/TransactionList:
    get:
      summary: Get Reports Transaction LIST
      description: "Report - Trial List \nMethod : GET\n\nDocs - https://developer.intuit.com/docs/api/accounting/transaction%20list"
      operationId: getReportsTransactionlist
      x-api-path-slug: reportstransactionlist-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: minorversion
      - in: header
        name: User-Agent
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Accounting
      - Reports
      - Transaction
      - LIST