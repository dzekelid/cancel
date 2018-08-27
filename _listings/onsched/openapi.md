swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/appointments/{id}/cancel:
    put:
      summary: Returns an appointment object
      description: "This end point cancels a booking or reservation. Only appointments
        in a \"BK\" booked, or \"RS\" reserved status can be cancelled.\r\nPast dated
        appointments cannot be cancelled.\r\n\r\nA valid appointment id is required.
        Use the appointmentId returned from POST /consumer/v1/appointments"
      operationId: ConsumerV1AppointmentsByIdCancelPut
      x-api-path-slug: consumerv1appointmentsidcancel-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Cancel