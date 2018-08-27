{
  "info": {
    "name": "AWS EC2 API Cancel Import Task",
    "_postman_id": "a16bea0b-4afd-4717-bb5b-d4d19611bd29",
    "description": "Cancels an in-process import virtual machine or import snapshot task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Bundle Task",
      "item": [
        {
          "id": "6add9b5c-19c6-4cfe-9adb-85d289935dc2",
          "name": "cancelbundletask",
          "request": {
            "url": "http://example.com/api/?Action=CancelBundleTask?BundleId.N=BundleId.N&DryRun=DryRun&Filter.N=Filter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a bundling operation for an instance store-backed Windows instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4356aa5c-321d-4b38-8b5b-068d9aa371f0"
            }
          ]
        },
        {
          "id": "85680b1a-fcae-4a8b-9c49-d1fea6400287",
          "name": "describebundletasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBundleTasks?DryRun=DryRun&InstanceId=InstanceId&SecurityGroupId.N=SecurityGroupId.N&VpcId=VpcId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your bundling tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31b1a677-8edd-45bb-8bd5-80299ebc94c6"
            }
          ]
        },
        {
          "id": "97a076b5-9821-44ea-a32f-0c3a846bfc21",
          "name": "cancelconversiontask",
          "request": {
            "url": "http://example.com/api/?Action=CancelConversionTask",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an active conversion task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "229d5d7a-424a-4437-83ac-648a98f678c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Import Task",
      "item": [
        {
          "id": "fa439814-6086-4909-b69a-77fa43acfc24",
          "name": "cancelimporttask",
          "request": {
            "url": "http://example.com/api/?Action=CancelImportTask?ConversionTaskId.N=ConversionTaskId.N&DryRun=DryRun",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-process import virtual machine or import snapshot task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f301a564-a597-4dfe-9ded-36477ece677b"
            }
          ]
        }
      ]
    }
  ]
}