{
  "info": {
    "name": "AWS CloudFormation API Cancel Update Stack",
    "_postman_id": "a86b07a9-70d4-4866-bfbf-f4da9132c7e1",
    "description": "Cancels an update on the specified stack.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "3e9bcd39-e699-40aa-8222-08e88dfcdf00",
          "name": "cancelUpdateStack",
          "request": {
            "url": "http://example.com/api/?Action=CancelUpdateStack?StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an update on the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cd67b24-0103-43f0-aaf8-99f94cdeb646"
            }
          ]
        }
      ]
    }
  ]
}