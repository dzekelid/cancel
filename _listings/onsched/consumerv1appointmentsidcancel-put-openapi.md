---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns an appointment object
  description: "This end point cancels a booking or reservation. Only appointments
    in a \"BK\" booked, or \"RS\" reserved status can be cancelled.\r\nPast dated
    appointments cannot be cancelled.\r\n\r\nA valid appointment id is required. Use
    the appointmentId returned from POST /consumer/v1/appointments"
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/appointments/{id}/cancel:
    put:
      summary: Returns an appointment object
      description: "This end point cancels a booking or reservation. Only appointments
        in a \"BK\" booked, or \"RS\" reserved status can be cancelled.\r\nPast dated
        appointments cannot be cancelled.\r\n\r\nA valid appointment id is required.
        Use the appointmentId returned from POST /consumer/v1/appointments"
      operationId: ConsumerV1AppointmentsByIdCancelPut
      x-api-path-slug: consumerv1appointmentsidcancel-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Cancel
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