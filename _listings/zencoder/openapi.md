---
swagger: "2.0"
x-collection-name: Zencoder
x-complete: 1
info:
  title: Zencoder
  version: v2
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
---