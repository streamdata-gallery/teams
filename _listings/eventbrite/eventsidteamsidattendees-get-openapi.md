---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Events Teams Attendees
  description: Returns attendee for a single attendee-team.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/teams/:
    get:
      summary: Get Events Teams
      description: Returns a list of attendee-team for the event.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteams-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/:
    get:
      summary: Get Events Teams
      description: Returns information for a single attendee-team.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteamsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/attendees/:
    get:
      summary: Get Events Teams Attendees
      description: Returns attendee for a single attendee-team.
      operationId: getEventsTeamsAttendees
      x-api-path-slug: eventsidteamsidattendees-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
      - Attendees
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