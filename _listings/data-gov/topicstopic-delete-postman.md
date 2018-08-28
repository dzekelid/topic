{
  "info": {
    "name": "Data.gov API Delete Topics Topic",
    "_postman_id": "03b9eec1-4b7a-4a9b-8645-c6292c78c415",
    "description": "Delete a given topic",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "topics",
      "item": [
        {
          "id": "d3016298-a42e-486a-ac90-58af77d8f0ab",
          "name": "deleteTopicsTopic",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a given topic"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f2f1a26-a1b0-4e69-8066-54a477fb37d4"
            }
          ]
        }
      ]
    }
  ]
}