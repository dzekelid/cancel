swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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