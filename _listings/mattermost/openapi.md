swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{job_id}/cancel:
    post:
      summary: Cancel a job.
      description: |-
        Cancel a job.
        __Minimum server version: 4.1__
        ##### Permissions
        Must have `manage_jobs` permission.
      operationId: cancel-a-job-minimum-server-version-41--permissionsmust-have-manage-jobs-permission
      x-api-path-slug: jobsjob-idcancel-post
      parameters:
      - in: path
        name: job_id
        description: Job GUID
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Job.