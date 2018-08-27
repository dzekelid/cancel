---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Event Delete
  description: Cancels or removes an event from a groups calendar
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/events/:id:
    delete:
      summary: Event Delete
      description: Cancels or removes an event from a groups calendar
      operationId: events
      x-api-path-slug: urlnameeventsid-delete
      parameters:
      - in: query
        name: remove_from_calendar
        description: Optional boolean parameter that, when set to true, fully deletes
          the event
        type: string
      - in: query
        name: update_series
        description: Optional boolean parameter that, when set to true, will update
          all future recurrences of this event if this event belongs to an event series
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
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