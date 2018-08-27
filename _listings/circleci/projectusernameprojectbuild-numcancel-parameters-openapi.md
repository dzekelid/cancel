---
swagger: "2.0"
x-collection-name: CircleCI
x-complete: 0
info:
  title: CircleCI Parameters Project Username Project Build Num Cancel
  description: Parameters project username project build num cancel.
  version: 1.0.0
host: circleci.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /project/{username}/{project}/{build_num}/cancel:
    parameters:
      summary: Parameters Project Username Project Build Num Cancel
      description: Parameters project username project build num cancel.
      operationId: parametersProjectUsernameProjectBuildNumCancel
      x-api-path-slug: projectusernameprojectbuild-numcancel-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Num
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