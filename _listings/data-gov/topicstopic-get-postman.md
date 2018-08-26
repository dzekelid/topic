{
  "info": {
    "name": "Data.gov API Get Topics Topic",
    "_postman_id": "dd8743f6-34c5-4d32-ae1a-e9c215967070",
    "description": "Get a given topic",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "topics",
      "item": [
        {
          "id": "98710bf3-4c72-41a1-8697-079497ba4487",
          "name": "getTopicsTopic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "topics/:topic/"
              ],
              "variable": [
                {
                  "id": "topic",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a given topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57e8541c-1ba1-4e77-80ca-b94087a21645"
            }
          ]
        }
      ]
    }
  ]
}