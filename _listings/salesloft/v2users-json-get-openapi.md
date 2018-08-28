---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft List users
  description: |-
    Non Admin: Lists only your user, or all on team depending on group visibility policy
    Team Admin: Lists users associated with your team
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/accounts.json:
    get:
      summary: List accounts
      description: |-
        Fetches multiple account records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.accounts.json.get
      x-api-path-slug: v2accounts-json-get
      parameters:
      - in: query
        name: domain
        description: Domain of the accounts to fetch
      - in: query
        name: ids
        description: IDs of accounts to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_contacted_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Accounts
  /v2/action_details/call_instructions.json:
    get:
      summary: List call instructions
      description: |-
        Fetches multiple call instruction records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.action_details.call_instructions.json.get
      x-api-path-slug: v2action-detailscall-instructions-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of call instructions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Instructions
  /v2/actions.json:
    get:
      summary: List actions
      description: |-
        Fetches multiple action records. The records can be filtered, paged, and sorted according to
        the respective parameters. Only actions that are currently "in_progess" will be returned by
        this endpoint.
      operationId: v2.actions.json.get
      x-api-path-slug: v2actions-json-get
      parameters:
      - in: query
        name: due_on
        description: Equality filters that are applied to the due_on field
      - in: query
        name: ids
        description: IDs of actions to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: step_id
        description: Fetch actions by step ID
      - in: query
        name: type
        description: Filter actions by type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Actions
  /v2/activities/calls.json:
    get:
      summary: List calls
      description: |-
        Fetches multiple call records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.calls.json.get
      x-api-path-slug: v2activitiescalls-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of calls to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Calls
  /v2/activities/emails.json:
    get:
      summary: List emails
      description: |-
        Fetches multiple email records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.activities.emails.json.get
      x-api-path-slug: v2activitiesemails-json-get
      parameters:
      - in: query
        name: bounced
        description: Filters emails by whether they have bounced or not
      - in: query
        name: ids
        description: IDs of emails to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Emails
  /v2/cadence_memberships.json:
    get:
      summary: List cadence memberships
      description: |-
        Fetches multiple cadence membership records. The records can be filtered, paged, and sorted according to
        the respective parameters. A cadence membership is the association between a person and their current and
        historical time on a cadence. Cadence membership records are mutable and change over time. If a person is
        added to a cadence and re-added to the same cadence in the future, there is a single membership record.
      operationId: v2.cadence_memberships.json.get
      x-api-path-slug: v2cadence-memberships-json-get
      parameters:
      - in: query
        name: cadence_id
        description: ID of the cadence to find cadence memberships for
      - in: query
        name: ids
        description: IDs of cadence memberships to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: person_id
        description: ID of the person to find cadence memberships for
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Cadence
      - Memberships
  /v2/cadences.json:
    get:
      summary: List cadences
      description: |-
        Fetches multiple cadence records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.cadences.json.get
      x-api-path-slug: v2cadences-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of cadences to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: team_cadence
        description: Filters cadences by whether they are a team cadence or not
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Cadences
  /v2/call_data_records.json:
    get:
      summary: List call data records
      description: |-
        Fetches multiple call data records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Call data records are records of all inbound and outbound calls through SalesLoft. A call data record may
        be associated with a call, but does not have to be.
      operationId: v2.call_data_records.json.get
      x-api-path-slug: v2call-data-records-json-get
      parameters:
      - in: query
        name: has_call
        description: Return only call data records which have or do not have a call
          logged for them
      - in: query
        name: ids
        description: IDs of call data records to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Call
      - Data
      - Records
  /v2/crm_activities.json:
    get:
      summary: List crm activities
      description: |-
        Fetches multiple crm activity records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.crm_activities.json.get
      x-api-path-slug: v2crm-activities-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of crm activities to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Crm
      - Activities
  /v2/custom_fields.json:
    get:
      summary: List custom fields
      description: |-
        Fetches multiple custom field records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.custom_fields.json.get
      x-api-path-slug: v2custom-fields-json-get
      parameters:
      - in: query
        name: field_type
        description: Type of field to fetch
      - in: query
        name: ids
        description: IDs of custom fields to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, name'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Custom
      - Fields
  /v2/email_templates.json:
    get:
      summary: List email templates
      description: |-
        Fetches multiple email template records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.email_templates.json.get
      x-api-path-slug: v2email-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of email templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: linked_to_team_template
        description: Filters email templates by whether they are linked to a team
          template or not
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Email
      - Templates
  /v2/imports.json:
    get:
      summary: List imports
      description: Fetches multiple imports.
      operationId: v2.imports.json.get
      x-api-path-slug: v2imports-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of imports to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: user_ids
        description: ID of users to fetch imports for
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Imports
  /v2/notes.json:
    get:
      summary: List notes
      description: |-
        Fetches multiple note records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.notes.json.get
      x-api-path-slug: v2notes-json-get
      parameters:
      - in: query
        name: associated_with_id
        description: ID of the item with which the note is associated
      - in: query
        name: associated_with_type
        description: Case insensitive type of item with which the note is associated
      - in: query
        name: ids
        description: IDs of notes to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Notes
  /v2/people.json:
    get:
      summary: List people
      description: |-
        Fetches multiple person records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.people.json.get
      x-api-path-slug: v2people-json-get
      parameters:
      - in: query
        name: email_addresses
        description: Filters people by email address
      - in: query
        name: ids
        description: IDs of people to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_contacted_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - People
  /v2/person_stages.json:
    get:
      summary: List person stages
      description: |-
        Fetches multiple person stage records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.person_stages.json.get
      x-api-path-slug: v2person-stages-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of person stages to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Person
      - Stages
  /v2/phone_numbers/caller_ids.json:
    get:
      summary: List caller ids
      description: |-
        Each entry is a possible caller ID match for the number. Multiple
        entries may be returned if the phone number is present on more than one
        person in the system.  Phone number should be in E.164 format.
      operationId: v2.phone_numbers.caller_ids.json.get
      x-api-path-slug: v2phone-numberscaller-ids-json-get
      parameters:
      - in: query
        name: phone_number
        description: E
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Caller
      - Ids
  /v2/steps.json:
    get:
      summary: List steps
      description: |-
        Fetches multiple step records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.steps.json.get
      x-api-path-slug: v2steps-json-get
      parameters:
      - in: query
        name: cadence_id
        description: Filter by cadence ID
      - in: query
        name: has_due_actions
        description: Filter by whether a step has due actions
      - in: query
        name: ids
        description: IDs of steps to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: type
        description: Filter by step type
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Steps
  /v2/successes.json:
    get:
      summary: List successes
      description: |-
        Fetches multiple success records. The records can be filtered, paged, and sorted according to
        the respective parameters.
      operationId: v2.successes.json.get
      x-api-path-slug: v2successes-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of successes to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, succeeded_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Successes
  /v2/team_templates.json:
    get:
      summary: List team templates
      description: |-
        Fetches multiple team template records. The records can be filtered, paged, and sorted according to
        the respective parameters.

        Team templates are templates that are available team-wide. Admins may use
        team templates to create original content for the entire team, monitor version control to ensure templates are always up to date,
        and track template performance across the entire organization. All metrics on a team template reflect usage across the team; individual metrics can be found with the email_templates API endpoint.
      operationId: v2.team_templates.json.get
      x-api-path-slug: v2team-templates-json-get
      parameters:
      - in: query
        name: ids
        description: IDs of team templates to fetch
      - in: query
        name: include_paging_counts
        description: Whether to include total_pages and total_count in the metadata
      - in: query
        name: page
        description: The current page to fetch results from
      - in: query
        name: per_page
        description: How many records to show per page in the range [1, 100]
      - in: query
        name: sort_by
        description: 'Key to sort on, must be one of: created_at, updated_at, last_used_at'
      - in: query
        name: sort_direction
        description: 'Direction to sort in, must be one of: ASC, DESC'
      - in: query
        name: updated_at
        description: Equality filters that are applied to the updated_at field
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Team
      - Templates
  /v2/users.json:
    get:
      summary: List users
      description: |-
        Non Admin: Lists only your user, or all on team depending on group visibility policy
        Team Admin: Lists users associated with your team
      operationId: v2.users.json.get
      x-api-path-slug: v2users-json-get
      responses:
        200:
          description: OK
      tags:
      - Sales
      - List
      - Users
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