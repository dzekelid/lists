---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Billing API Invoice Line Items List
  description: Invoice line items list.
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/accounts.xml:
    get:
      summary: Account List
      description: Account list.
      operationId: account
      x-api-path-slug: adminapiaccounts-xml-get
      parameters:
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: state
        description: Account state
      responses:
        200:
          description: OK
      tags:
      - Account
      - List
  /admin/api/accounts/{account_id}/applications.xml:
    get:
      summary: Application List
      description: Application list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplications-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - List
  /admin/api/accounts/{account_id}/applications/{application_id}/keys.xml:
    get:
      summary: Application Key List
      description: Application key list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idkeys-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Key
      - List
  /admin/api/accounts/{account_id}/applications/{application_id}/referrer_filters.xml:
    get:
      summary: Application Referrer Filter List
      description: Application referrer filter list.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsapplication-idreferrer-filters-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: application_id
        description: id of the application
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Referrer
      - Filter
      - List
  /admin/api/accounts/{account_id}/users.xml:
    get:
      summary: User List
      description: User list.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusers-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: role
        description: Filter users by Role
      - in: query
        name: state
        description: Filter users by State
      responses:
        200:
          description: OK
      tags:
      - User
      - List
  /admin/api/account_plans.xml:
    get:
      summary: Account Plan List
      description: Account plan list.
      operationId: account_plan
      x-api-path-slug: adminapiaccount-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - List
  /admin/api/account_plans/{account_plan_id}/features.xml:
    get:
      summary: Account Plan Feature List
      description: Account plan feature list.
      operationId: account_plan_feature
      x-api-path-slug: adminapiaccount-plansaccount-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: account_plan_id
        description: id of the account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Plan
      - Feature
      - List
  /admin/api/applications.xml:
    get:
      summary: Application List (all services)
      description: Application list (all services).
      operationId: application
      x-api-path-slug: adminapiapplications-xml-get
      parameters:
      - in: query
        name: active_since
        description: filter date
      - in: query
        name: inactive_since
        description: filter date
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: service_id
        description: filter by service
      responses:
        200:
          description: OK
      tags:
      - Application
      - List
      - (all
      - Services)
  /admin/api/application_plans.xml:
    get:
      summary: Application Plan List (all services)
      description: Application plan list (all services).
      operationId: application_plan
      x-api-path-slug: adminapiapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
      - (all
      - Services)
  /admin/api/application_plans/{application_plan_id}/features.xml:
    get:
      summary: Application Plan Feature List
      description: Application plan feature list.
      operationId: application_plan_feature
      x-api-path-slug: adminapiapplication-plansapplication-plan-idfeatures-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - Feature
      - List
  /admin/api/application_plans/{application_plan_id}/limits.xml:
    get:
      summary: Limits List per Application Plan
      description: Limits list per application plan.
      operationId: application_plan_limits
      x-api-path-slug: adminapiapplication-plansapplication-plan-idlimits-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limits
      - List
      - Per
      - Application
      - Plan
  /admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/limits.xml:
    get:
      summary: Limit List per Metric
      description: Limit list per metric.
      operationId: application_plan_limit
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idlimits-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Limit
      - List
      - Per
      - Metric
  /admin/api/application_plans/{application_plan_id}/metrics/{metric_id}/pricing_rules.xml:
    get:
      summary: Pricing Rules List per Metric
      description: Pricing rules list per metric.
      operationId: application_plan_pricing_rules
      x-api-path-slug: adminapiapplication-plansapplication-plan-idmetricsmetric-idpricing-rules-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Rules
      - List
      - Per
      - Metric
  /admin/api/application_plans/{application_plan_id}/pricing_rules.xml:
    get:
      summary: Pricing Rules List per Application Plan
      description: Pricing rules list per application plan.
      operationId: application_plan_pricing_rules
      x-api-path-slug: adminapiapplication-plansapplication-plan-idpricing-rules-xml-get
      parameters:
      - in: path
        name: application_plan_id
        description: id of the application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Pricing
      - Rules
      - List
      - Per
      - Application
      - Plan
  /admin/api/end_user_plans.xml:
    get:
      summary: End User Plan List (all services)
      description: End user plan list (all services).
      operationId: end_user_plan
      x-api-path-slug: adminapiend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
      - (all
      - Services)
  /admin/api/features.xml:
    get:
      summary: Account Feature List
      description: Account feature list.
      operationId: account_feature
      x-api-path-slug: adminapifeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Feature
      - List
  /admin/api/services.xml:
    get:
      summary: Service List
      description: Service list.
      operationId: service
      x-api-path-slug: adminapiservices-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - List
  /admin/api/services/{id}/service_plans.xml:
    get:
      summary: Service Plan List
      description: Service plan list.
      operationId: service_plan
      x-api-path-slug: adminapiservicesidservice-plans-xml-get
      parameters:
      - in: path
        name: id
        description: id of the service
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - List
  /admin/api/services/{service_id}/application_plans.xml:
    get:
      summary: Application Plan List
      description: Application plan list.
      operationId: application_plan
      x-api-path-slug: adminapiservicesservice-idapplication-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Application
      - Plan
      - List
  /admin/api/services/{service_id}/end_user_plans.xml:
    get:
      summary: End User Plan List
      description: End user plan list.
      operationId: end_user_plan
      x-api-path-slug: adminapiservicesservice-idend-user-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Plan
      - List
  /admin/api/services/{service_id}/features.xml:
    get:
      summary: Service Feature List
      description: Service feature list.
      operationId: service_feature
      x-api-path-slug: adminapiservicesservice-idfeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Service
      - Feature
      - List
  /admin/api/services/{service_id}/metrics.xml:
    get:
      summary: Metric List
      description: Metric list.
      operationId: metric
      x-api-path-slug: adminapiservicesservice-idmetrics-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Metric
      - List
  /admin/api/services/{service_id}/metrics/{metric_id}/methods.xml:
    get:
      summary: Method List
      description: Method list.
      operationId: metric_method
      x-api-path-slug: adminapiservicesservice-idmetricsmetric-idmethods-xml-get
      parameters:
      - in: path
        name: metric_id
        description: id of the metric
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      responses:
        200:
          description: OK
      tags:
      - Method
      - List
  /admin/api/service_plans.xml:
    get:
      summary: Service Plan List (all services)
      description: Service plan list (all services).
      operationId: service_plan
      x-api-path-slug: adminapiservice-plans-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - List
      - (all
      - Services)
  /admin/api/service_plans/{service_plan_id}/features.xml:
    get:
      summary: Service Plan Feature List
      description: Service plan feature list.
      operationId: service_plan_feature
      x-api-path-slug: adminapiservice-plansservice-plan-idfeatures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_plan_id
        description: id of the service plan
      responses:
        200:
          description: OK
      tags:
      - Service
      - Plan
      - Feature
      - List
  /admin/api/users.xml:
    get:
      summary: User List (provider account)
      description: User list (provider account).
      operationId: user_provider_account
      x-api-path-slug: adminapiusers-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: role
        description: Filter users by Role
      - in: query
        name: state
        description: Filter users by State
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - (provider
      - Account)
  /admin/api/webhooks/failures.xml:
    get:
      summary: Webhooks List Failed Deliveries
      description: Webhooks list failed deliveries.
      operationId: webhooks
      x-api-path-slug: adminapiwebhooksfailures-xml-get
      parameters:
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - List
      - Failed
      - Deliveries
  /api/accounts/{account_id}/invoices.xml:
    get:
      summary: Invoice List by Account
      description: Invoice list by account.
      operationId: finance
      x-api-path-slug: apiaccountsaccount-idinvoices-xml-get
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: query
        name: month
        description: Filter the invoice by month
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale
      - in: query
        name: state
        description: Filter the invoice by state
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - List
      - By
      - Account
  /api/invoices.xml:
    get:
      summary: Invoice List
      description: Invoice list.
      operationId: finance
      x-api-path-slug: apiinvoices-xml-get
      parameters:
      - in: query
        name: month
        description: Filter the invoice by month
      - in: query
        name: page
        description: Page in the paginated list
      - in: query
        name: per_page
        description: Number of results per page
      - in: query
        name: provider_key
        description: Your api key with 3scale
      - in: query
        name: state
        description: Filter the invoice by state
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - List
  /api/invoices/{invoice_id}/line_items.xml:
    get:
      summary: Invoice Line Items List
      description: Invoice line items list.
      operationId: finance
      x-api-path-slug: apiinvoicesinvoice-idline-items-xml-get
      parameters:
      - in: path
        name: invoice_id
        description: id of the invoice
      - in: query
        name: provider_key
        description: Your api key with 3scale
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - Line
      - Items
      - List
  /api/invoices/{invoice_id}/payment_transactions.xml:
    get:
      summary: Invoice Payment Transactions List
      description: Invoice payment transactions list.
      operationId: finance
      x-api-path-slug: apiinvoicesinvoice-idpayment-transactions-xml-get
      parameters:
      - in: path
        name: invoice_id
        description: id of the invoice
      - in: query
        name: provider_key
        description: Your api key with 3scale
      responses:
        200:
          description: OK
      tags:
      - Invoice
      - Payment
      - Transactions
      - List
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