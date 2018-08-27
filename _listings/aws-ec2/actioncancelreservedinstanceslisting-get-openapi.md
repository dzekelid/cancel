---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Cancel Reserved Instances Listing
  version: 1.0.0
  description: Cancels the specified Reserved Instance listing in the Reserved Instance
    Marketplace.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CancelBundleTask:
    get:
      summary: Cancel Bundle Task
      description: Cancels a bundling operation for an instance store-backed Windows
        instance.
      operationId: cancelbundletask
      x-api-path-slug: actioncancelbundletask-get
      parameters:
      - in: query
        name: BundleId.N
        description: One or more bundle task IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=CancelConversionTask:
    get:
      summary: Cancel Conversion Task
      description: Cancels an active conversion task.
      operationId: cancelconversiontask
      x-api-path-slug: actioncancelconversiontask-get
      responses:
        200:
          description: OK
      tags:
      - Bundle Task
  /?Action=CancelExportTask:
    get:
      summary: Cancel Export Task
      description: Cancels an active export task.
      operationId: cancelexporttask
      x-api-path-slug: actioncancelexporttask-get
      parameters:
      - in: query
        name: Description
        description: A description for the conversion task or the resource being exported
        type: string
      - in: query
        name: ExportToS3
        description: The format and location for an instance export task
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: TargetEnvironment
        description: The target virtualization environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task
  /?Action=CancelImportTask:
    get:
      summary: Cancel Import Task
      description: Cancels an in-process import virtual machine or import snapshot
        task.
      operationId: cancelimporttask
      x-api-path-slug: actioncancelimporttask-get
      parameters:
      - in: query
        name: ConversionTaskId.N
        description: One or more conversion task IDs
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,      and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Import Task
  /?Action=CancelReservedInstancesListing:
    get:
      summary: Cancel Reserved Instances Listing
      description: Cancels the specified Reserved Instance listing in the Reserved
        Instance Marketplace.
      operationId: cancelreservedinstanceslisting
      x-api-path-slug: actioncancelreservedinstanceslisting-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of yourlistings
        type: string
      - in: query
        name: InstanceCount
        description: The number of instances that are a part of a Reserved Instance
          account to be listed in the Reserved Instance Marketplace
        type: string
      - in: query
        name: PriceSchedules.N
        description: A list specifying the price of the Standard Reserved Instance
          for each month remaining in the Reserved Instance term
        type: string
      - in: query
        name: ReservedInstancesId
        description: The ID of the active Standard Reserved Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
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