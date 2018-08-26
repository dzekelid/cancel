---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Cancel task
  description: |-
    Requests that the task that corresponds to the given task id is cancelled.

    To cancel a task, you need to be its creator or a Jira admin. Otherwise a 403 response will be returned.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/task/{taskId}/cancel:
    post:
      summary: Cancel task
      description: |-
        Requests that the task that corresponds to the given task id is cancelled.

        To cancel a task, you need to be its creator or a Jira admin. Otherwise a 403 response will be returned.
      operationId: com.atlassian.jira.rest.v2.task.TaskResource.cancelTask_post
      x-api-path-slug: api2tasktaskidcancel-post
      parameters:
      - in: path
        name: taskId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Task
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