swagger: "2.0"
x-collection-name: CircleCI
x-complete: 1
info:
  title: CircleCI
  description: the-circleci-api-is-a-restful-fullyfeatured-api-that-allows-you-to-do-almost-anything-in-circleci--you-can-access-all-information-and-trigger-all-actions--the-only-thing-we-dont-provide-access-to-is-billing-functions-which-must-be-done-from-the-circleci-web-ui-
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
    post:
      summary: Add Project Username Project Build Num Cancel
      description: Cancels the build, returns a summary of the build.
      operationId: postProjectUsernameProjectBuildNumCancel
      x-api-path-slug: projectusernameprojectbuild-numcancel-post
      responses:
        200:
          description: OK
      tags:
      - Project
      - Username
      - Project
      - Build
      - Num
      - Cancel