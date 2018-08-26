---
swagger: "2.0"
x-collection-name: Zencoder
x-complete: 0
info:
  title: Zencoder API Cancel a Job
  version: v2
  description: If you wish to cancel a job that has not yet finished processing you
    may send a request.
host: app.zencoder.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{job_id}/cancel:
    put:
      summary: Cancel a Job
      description: If you wish to cancel a job that has not yet finished processing
        you may send a request.
      operationId: putJobsJobCancel
      x-api-path-slug: jobsjob-idcancel-put
      parameters:
      - in: query
        name: api_key
        description: The API Key
      - in: query
        name: job_id
        description: The job id
      responses:
        200:
          description: OK
      tags:
      - Jobs
      - Job
      - Id
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