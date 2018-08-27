swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
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