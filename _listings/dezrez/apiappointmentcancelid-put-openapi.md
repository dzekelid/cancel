---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Cancel an appointment by id if it exists.
  version: 1.0.0
  description: Cancel an appointment by id if it exists..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/appointment/cancel/{id}:
    put:
      summary: Cancel an appointment by id if it exists.
      description: Cancel an appointment by id if it exists..
      operationId: Appointment_CancelByidBycancelAppointmentDataContract
      x-api-path-slug: apiappointmentcancelid-put
      parameters:
      - in: body
        name: cancelAppointmentDataContract
        description: The cancellation details, including reason of cancellation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the appointment id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Appointment
      - By
      - Id
      - If
      - It
      - Exists
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