---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava List Segment Efforts
  description: Returns a set of the authenticated athlete's segment efforts for a
    given segment.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /segments/starred:
    get:
      summary: List Starred Segments
      description: List of the authenticated athlete's starred segments.
      operationId: getLoggedInAthleteStarredSegments
      x-api-path-slug: segmentsstarred-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Starred
      - Segments
  /segments/{id}/all_efforts:
    get:
      summary: List Segment Efforts
      description: Returns a set of the authenticated athlete's segment efforts for
        a given segment.
      operationId: getEffortsBySegmentId
      x-api-path-slug: segmentsidall-efforts-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Segment
      - Efforts
  /running_races:
    get:
      summary: List Running Races
      description: Returns a list running races based on a set of search criteria.
      operationId: getRunningRaces
      x-api-path-slug: running-races-get
      parameters:
      - in: query
        name: year
        description: Filters the list by a given year
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Running
      - Races
  /athlete/activities:
    get:
      summary: List Athlete Activities
      description: Returns the activities of an athlete for a specific identifier.
      operationId: getLoggedInAthleteActivities
      x-api-path-slug: athleteactivities-get
      parameters:
      - in: query
        name: after
        description: An epoch timestamp to use for filtering activities that have
          taken place after a certain time
      - in: query
        name: before
        description: An epoch timestamp to use for filtering activities that have
          taken place before a certain time
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Athlete
      - Activities
  /activities/{id}/laps:
    get:
      summary: List Activity Laps
      description: Returns the laps of an activity identified by an identifier.
      operationId: getLapsByActivityId
      x-api-path-slug: activitiesidlaps-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Activity
      - Laps
  /activities/{id}/comments:
    get:
      summary: List Activity Comments
      description: Returns the comments on the given activity.
      operationId: getCommentsByActivityId
      x-api-path-slug: activitiesidcomments-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Activity
      - Comments
  /activities/{id}/kudos:
    get:
      summary: List Activity Kudoers
      description: Returns the athletes who kudoed an activity identified by an identifier.
      operationId: getKudoersByActivityId
      x-api-path-slug: activitiesidkudos-get
      parameters:
      - in: path
        name: id
        description: The identifier of the activity
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Activity
      - Kudoers
  /clubs/{id}/members:
    get:
      summary: List Club Members
      description: Returns a list of the athletes who are members of a given club.
      operationId: getClubMembersById
      x-api-path-slug: clubsidmembers-get
      parameters:
      - in: path
        name: id
        description: The identifier of the club
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Club
      - Members
  /clubs/{id}/admins:
    get:
      summary: List Club Administrators.
      description: Returns a list of the administrators of a given club.
      operationId: getClubAdminsById
      x-api-path-slug: clubsidadmins-get
      parameters:
      - in: path
        name: id
        description: The identifier of the club
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Club
      - Administrators
  /clubs/{id}/activities:
    get:
      summary: List Club Activities
      description: Retrieve recent activities from members of a specific club. The
        authenticated athlete must belong to the requested club in order to hit this
        endpoint. Pagination is supported. Enhanced Privacy Mode is respected for
        all activities.
      operationId: getClubActivitiesById
      x-api-path-slug: clubsidactivities-get
      parameters:
      - in: path
        name: id
        description: The identifier of the club
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Club
      - Activities
  /athlete/clubs:
    get:
      summary: List Athlete Clubs
      description: Returns a list of the clubs whose membership includes the authenticated
        athlete.
      operationId: getLoggedInAthleteClubs
      x-api-path-slug: athleteclubs-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Athlete
      - Clubs
  /athletes/{id}/routes:
    get:
      summary: List Athlete Routes
      description: Returns a list of the routes created by the authenticated athlete
        using their athlete ID.
      operationId: getRoutesByAthleteId
      x-api-path-slug: athletesidroutes-get
      parameters:
      - in: path
        name: id
        description: The identifier of the athlete
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Athlete
      - Routes
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