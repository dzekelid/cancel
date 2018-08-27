swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
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