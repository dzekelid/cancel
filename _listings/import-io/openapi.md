swagger: "2.0"
x-collection-name: Import.io
x-complete: 1
info:
  title: import.io
  version: "1.0"
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