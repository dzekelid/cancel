{
  "info": {
    "name": "Viddler  API Encoding Cancel",
    "_postman_id": "ace351cf-80bb-4884-bd72-8849f40fe950",
    "description": "Cancel encoding a specific video file.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "a1589fee-1d90-4c7d-a374-63819b71ee29",
          "name": "api-echo",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.api.echo?message=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method is used for testing purposes only. Simply call this method to make sure the API is responding fine."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c0b2ab4-bd2b-46d8-a7a3-28cb216273a8"
            }
          ]
        },
        {
          "id": "307b9b22-fb86-4f65-8d26-90e1fedd06c9",
          "name": "encoding-cancel",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.encoding.cancel?file_id=%7B%7D&sessionid=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel encoding a specific video file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a4fe132-2f0f-4ed5-8fab-f03cbf4aaef1"
            }
          ]
        }
      ]
    }
  ]
}