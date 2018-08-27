swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AbortEnvironmentUpdate:
    get:
      summary: Abort Environment Update
      description: |-
        Cancels in-progress environment configuration update or application version
              deployment.
      operationId: abortEnvironmentUpdate
      x-api-path-slug: actionabortenvironmentupdate-get
      parameters:
      - in: query
        name: EnvironmentId
        description: This specifies the ID of the environment with the in-progress
          update that you want to      cancel
        type: string
      - in: query
        name: EnvironmentName
        description: This specifies the name of the environment with the in-progress
          update that you want to      cancel
        type: string
      responses:
        200:
          description: OK
      tags:
      - Environments