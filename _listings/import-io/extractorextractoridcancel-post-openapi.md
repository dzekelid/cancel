---
swagger: "2.0"
x-collection-name: Import.io
x-complete: 0
info:
  title: import.io Post Extractor Extractorid Cancel
  version: "1.0"
  description: Cancel an existing crawl..
host: schedule.import.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extractor/{extractorId}/cancel:
    post:
      summary: Post Extractor Extractorid Cancel
      description: Cancel an existing crawl..
      operationId: postExtractorExtractorCancel
      x-api-path-slug: extractorextractoridcancel-post
      parameters:
      - in: path
        name: extractorId
        description: extractorId
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
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