swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
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