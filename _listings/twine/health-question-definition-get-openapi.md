---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine List health question definitions
  description: Get a list of all health question definitions
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendar_event:
    get:
      summary: List calendar events
      description: Get a list of calendar events
      operationId: fetchCalendarEvents
      x-api-path-slug: calendar-event-get
      parameters:
      - in: query
        name: filter[attendees]
        description: Comma-separated list of coach or patient ids
      - in: query
        name: filter[completed]
        description: If not specified, return all calendar events
      - in: query
        name: filter[completed_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[created_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[end_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch calendar event
      - in: query
        name: filter[start_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[type]
        description: Calendar event type
      - in: query
        name: filter[updated_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Calendar
      - Events
  /email_history:
    get:
      summary: List email histories
      description: Get a list of email histories
      operationId: fetchEmailHistories
      x-api-path-slug: email-history-get
      parameters:
      - in: query
        name: filter[emailType]
        description: Type of email
      - in: query
        name: filter[receiver]
        description: Twine user id of email recipient
      - in: query
        name: filter[sender]
        description: Twine user id of email sender
      - in: query
        name: sort
        description: 'valid sorts:  * send_time - ascending by send_time  * -send_time
          - descending by send_time'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Email
      - Histories
  /group:
    get:
      summary: List groups
      description: Get a list of groups matching the specified filters.
      operationId: fetchGroups
      x-api-path-slug: group-get
      parameters:
      - in: query
        name: filter[name]
        description: Group name
      - in: query
        name: filter[organization]
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groups
  /health_profile:
    get:
      summary: List health profiles
      description: Get a list of health profiles
      operationId: fetchHealthProfiles
      x-api-path-slug: health-profile-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch health profile
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Profiles
  /health_profile_answer:
    get:
      summary: List health profile answers
      description: Get a list of health profile answers
      operationId: fetchHealthProfileAnswers
      x-api-path-slug: health-profile-answer-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch healt profile answers
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Profile
      - Answers
  /health_question_definition:
    get:
      summary: List health question definitions
      description: Get a list of all health question definitions
      operationId: fetchHealthQuestionDefinitions
      x-api-path-slug: health-question-definition-get
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Health
      - Question
      - Definitions
  /patient:
    get:
      summary: List patients
      description: Get a list of patients.
      operationId: fetchPatients
      x-api-path-slug: patient-get
      parameters:
      - in: query
        name: filter[archived]
        description: If not specified, return all patients
      - in: query
        name: filter[created_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[identifier][system]
        description: 'Identifier system (example: MyEHR) - requires a filter[identifier][value]
          parameter'
      - in: query
        name: filter[identifier][value]
        description: 'Identifier value (example: 12345) - requires a filter[identifier][system]
          parameter'
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[updated_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Patients
  /patient/{id}/coaches:
    get:
      summary: List coaches for a patient
      description: Get the list of coaches for a patient.
      operationId: fetchPatientCoaches
      x-api-path-slug: patientidcoaches-get
      parameters:
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Coachesa
      - Patient
  /patient/{id}/groups:
    get:
      summary: List groups for a patient
      description: Get the list of groups for a patient.
      operationId: fetchPatientGroups
      x-api-path-slug: patientidgroups-get
      parameters:
      - in: path
        name: id
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groupsa
      - Patient
  /patient_health_metric:
    get:
      summary: List patient health metrics
      description: Get a list of patient health metrics.
      operationId: fetchPatientHealthMetrics
      x-api-path-slug: patient-health-metric-get
      parameters:
      - in: query
        name: filter[patient]
        description: Filter the patient health metrics for a specified patient
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Patient
      - Health
      - Metrics
  /patient_plan_summary:
    get:
      summary: List patient plan summaries
      description: Get a list of patient plan summaries
      operationId: fetchPatientPlanSummaries
      x-api-path-slug: patient-plan-summary-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient id to fetch plan summary for
      - in: query
        name: include
        description: List of related resources to include in the response
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Patient
      - Plan
      - Summaries
  /reward:
    get:
      summary: List rewards
      description: Get a list of rewards matching the specified filters.
      operationId: fetchRewards
      x-api-path-slug: reward-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient identifier
      - in: query
        name: filter[reward_program_activation]
        description: Reward program activation identifier
      - in: query
        name: filter[thread]
        description: Thread identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Rewards
  /reward_earning:
    get:
      summary: List reward earnings
      description: Get a list of reward earnings matching the specified filters.
      operationId: fetchRewardEarnings
      x-api-path-slug: reward-earning-get
      parameters:
      - in: query
        name: filter[groups]
        description: Group identifiers
      - in: query
        name: filter[patient]
        description: Patient identifier
      - in: query
        name: filter[ready_for_fulfillment]
        description: If true, only returns those reward earnings for which ready_for_fulfillment
          is true and fulfilled_at is null
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Reward
      - Earnings
  /reward_earning_fulfillment:
    get:
      summary: List reward earning fulfillments
      description: Get a list of reward earning fulfillments matching the specified
        filters.
      operationId: fetchRewardEarningFulfillments
      x-api-path-slug: reward-earning-fulfillment-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Reward
      - Earning
      - Fulfillments
  /reward_program:
    get:
      summary: List reward programs
      description: Get a list of reward programs matching the specified filters.
      operationId: fetchRewardPrograms
      x-api-path-slug: reward-program-get
      parameters:
      - in: query
        name: filter[groups]
        description: Comma-separated list of group identifiers
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Reward
      - Programs
  /reward_program_activation:
    get:
      summary: List reward program activations
      description: Get a list of reward program activations matching the specified
        filters.
      operationId: fetchRewardProgramActivations
      x-api-path-slug: reward-program-activation-get
      parameters:
      - in: query
        name: filter[patient]
        description: Patient identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Reward
      - Program
      - Activations
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