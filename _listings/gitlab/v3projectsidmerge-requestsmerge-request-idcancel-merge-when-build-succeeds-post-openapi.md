---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Merge Requests Merge Request Cancel Merge When Build
    Succeeds
  version: 1.0.0
  description: Post projects merge requests merge request cancel merge when build
    succeeds.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/builds/{build_id}/cancel:
    post:
      summary: Post Projects Builds Build Cancel
      description: Cancel a specific build of a project
      operationId: postV3ProjectsIdBuildsBuildIdCancel
      x-api-path-slug: v3projectsidbuildsbuild-idcancel-post
      parameters:
      - in: path
        name: build_id
        description: The ID of a build
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Build
      - Cancel
  /v3/projects/{id}/merge_request/{merge_request_id}/cancel_merge_when_build_succeeds:
    post:
      summary: Post Projects Merge Request Merge Request Cancel Merge When Build Succeeds
      description: Post projects merge request merge request cancel merge when build
        succeeds.
      operationId: postV3ProjectsIdMergeRequestMergeRequestIdCancelMergeWhenBuildSucceeds
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcancel-merge-when-build-succeeds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Cancel
      - Merge
      - When
      - Build
      - Succeeds
  /v3/projects/{id}/merge_requests/{merge_request_id}/cancel_merge_when_build_succeeds:
    post:
      summary: Post Projects Merge Requests Merge Request Cancel Merge When Build
        Succeeds
      description: Post projects merge requests merge request cancel merge when build
        succeeds.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdCancelMergeWhenBuildSucceeds
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcancel-merge-when-build-succeeds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Cancel
      - Merge
      - When
      - Build
      - Succeeds
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