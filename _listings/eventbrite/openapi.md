---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /events/{id}/cancel/:
    post:
      summary: Post Events Cancel
      description: |-
        Cancels an event if it has not already been deleted. In order for cancel to be permitted, there must be no pending or
        completed orders. Returns a boolean indicating success or failure of the cancel.
      operationId: postEventsCancel
      x-api-path-slug: eventsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Cancel
  /series/{id}/cancel/:
    post:
      summary: Post Series Cancel
      description: |-
        Cancels a repeating event series and all of its occurrences that are not already canceled or deleted. In order for
        cancel to be permitted, there must be no pending or completed orders for any dates in the series. Returns a boolean
        indicating success or failure of the cancel.
      operationId: postSeriesCancel
      x-api-path-slug: seriesidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Cancel
---