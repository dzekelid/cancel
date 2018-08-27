---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Cancel a single or multiple tasks from a to-do bucket
  version: 1.0.0
  description: Cancel a single or multiple tasks from a to-do bucket.
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
  /api/appointment/cancel/{id}/Date/{date}:
    put:
      summary: Cancel calculated appointment by id and datetime, if it exists.
      description: Cancel calculated appointment by id and datetime, if it exists..
      operationId: Appointment_CancelByidBydateBycancelAppointmentDataContract
      x-api-path-slug: apiappointmentcanceliddatedate-put
      parameters:
      - in: body
        name: cancelAppointmentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: date
        description: appointment start date
      - in: path
        name: id
        description: appointment id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Calculated
      - Appointment
      - By
      - Id
      - Datetime
      - ""
      - If
      - It
      - Exists
  /api/todo/canceltodo:
    put:
      summary: Cancel a to-do list from the tile overview of to-dos
      description: Cancel a to-do list from the tile overview of to-dos.
      operationId: DefaultToDo_CancelTodoBycancelTodoCommandData
      x-api-path-slug: apitodocanceltodo-put
      parameters:
      - in: body
        name: cancelTodoCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - To-do
      - List
      - From
      - Tile
      - Overview
      - Of
      - To-dos
  /api/todo/canceltasks:
    put:
      summary: Cancel a single or multiple tasks from a to-do bucket
      description: Cancel a single or multiple tasks from a to-do bucket.
      operationId: DefaultToDo_CancelTasksBycancelTasksCommandData
      x-api-path-slug: apitodocanceltasks-put
      parameters:
      - in: body
        name: cancelTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Single
      - Multiple
      - Tasks
      - From
      - To-do
      - Bucket
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