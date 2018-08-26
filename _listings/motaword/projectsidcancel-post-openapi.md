---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 0
info:
  title: Mota Word Cancel your translation project
  description: Cancel your translation project.
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{id}/cancel:
    post:
      summary: Cancel your translation project
      description: Cancel your translation project.
      operationId: cancelProject
      x-api-path-slug: projectsidcancel-post
      parameters:
      - in: path
        name: id
        description: Project ID
      - in: formData
        name: reason
        description: Cancellation reason
      responses:
        200:
          description: OK
      tags:
      - Projects
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