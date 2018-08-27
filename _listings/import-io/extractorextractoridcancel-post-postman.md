{
  "info": {
    "name": "import.io Post Extractor Extractorid Cancel",
    "_postman_id": "060f5f3c-08b8-44c2-8f6d-c718af53fecd",
    "description": "Cancel an existing crawl..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Extractor",
      "item": [
        {
          "id": "ef3c39dc-6aa2-4fc7-88a2-91070bcb1aa7",
          "name": "getExtractorExtractorCsvLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/csv/latest"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the latest crawl run results as a csv."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50034b2b-861d-4815-83ce-166a0ca727a0"
            }
          ]
        },
        {
          "id": "bd695c65-534a-4623-aadb-f341269b2f0a",
          "name": "getExtractorExtractorJsonLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/json/latest"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the latest crawl run results as json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eebd2d1a-3f05-4471-aced-d2dc108c2cca"
            }
          ]
        },
        {
          "id": "4c9d7b9a-171f-4228-82ee-0d821aee318c",
          "name": "getExtractorExtractor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId"
              ],
              "query": [
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Query by extractor endpoint, adhoc runs only.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "737fecb8-afdf-4653-b910-f16ec3be2dd4"
            }
          ]
        },
        {
          "id": "a4777634-edeb-41e3-ad73-b72b707eaa15",
          "name": "getExtractorExtractorRuns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/runs"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a feed of the runs performed on an extractor."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d38ebfb2-0b08-4119-8775-f092c95be757"
            }
          ]
        },
        {
          "id": "96c189a9-77c3-4fc8-a740-ce3a714616a6",
          "name": "postExtractorExtractorCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/cancel"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Cancel an existing crawl.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "910c9882-407f-414b-b68b-2d97173d0362"
            }
          ]
        }
      ]
    }
  ]
}