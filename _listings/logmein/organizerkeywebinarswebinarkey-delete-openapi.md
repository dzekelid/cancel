---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToWebinar Cancel Webinar
  description: Cancel webinar.
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/trainings/{trainingKey}/registrants/{registrantKey}:
    delete:
      summary: Cancel Registration
      description: Cancel registration.
      operationId: OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyDelete
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Registration
  /{organizerKey}/webinars/{webinarKey}:
    delete:
      summary: Cancel Webinar
      description: Cancel webinar.
      operationId: WebinarsByOrganizerKeyAndWebinarKeyDelete
      x-api-path-slug: organizerkeywebinarswebinarkey-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: query
        name: sendCancellationEmails
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Webinar
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