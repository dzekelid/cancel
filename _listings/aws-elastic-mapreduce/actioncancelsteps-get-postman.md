{
  "info": {
    "name": "AWS Elastic MapReduce API Cancel Steps",
    "_postman_id": "b09a3130-3231-4f91-926d-b784bf110cfb",
    "description": "Cancels a pending step or steps in a running cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Job Flow Steps",
      "item": [
        {
          "id": "37d445ce-d8cb-49a1-a8c5-c25ddc74d4bc",
          "name": "addJobFlowSteps",
          "request": {
            "url": "http://example.com/api/?Action=AddJobFlowSteps?JobFlowId=JobFlowId&Steps=Steps",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AddJobFlowSteps adds new steps to a running job flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab7adc59-427a-42e2-bf79-36ea2e364aa4"
            }
          ]
        }
      ]
    },
    {
      "name": "Steps",
      "item": [
        {
          "id": "c0ddf427-82e2-409f-b9b1-95d9380edef6",
          "name": "cancelSteps",
          "request": {
            "url": "http://example.com/api/?Action=CancelSteps?ClusterId=ClusterId&StepIds=StepIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending step or steps in a running cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34348db2-8a31-448e-b64a-22c8a79c0c97"
            }
          ]
        }
      ]
    }
  ]
}