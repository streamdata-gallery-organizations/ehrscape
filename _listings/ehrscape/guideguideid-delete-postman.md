{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs Deletes guide.",
    "_postman_id": "d60b6ff7-3409-4d16-851e-57ac80b742c4",
    "description": "Deletes guide..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "16fe2384-c8b8-48b0-a2bc-7ed555525688",
          "name": "getGuides",
          "request": {
            "url": "http://rest.ehrscape.com/ThinkCDS/services/CDSResources/guide",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List available guides.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66e98b8f-843d-4c45-9c01-ba3e854122d9"
            }
          ]
        },
        {
          "id": "23217e90-7053-4fbd-8b95-f8c7775f141d",
          "name": "executeGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/execute/:guideId/:ehrIds"
              ],
              "query": [
                {
                  "key": "persist",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "ehrIds",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "ThinkEhr credentials as HTTP Basic Authorization",
                "disabled": false
              },
              {
                "key": "Ehr-Session",
                "value": "{}",
                "description": "Active Ehr Session token",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Execute guide on given ehr ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53b84de9-a15f-421e-a72f-cebcdce6d380"
            }
          ]
        },
        {
          "id": "05d62839-47a4-4003-8fad-b42f4b9cfd3f",
          "name": "uploadGuide",
          "request": {
            "url": "http://rest.ehrscape.com/ThinkCDS/services/CDSResources/guide/upload",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "guide",
                  "value": "{}",
                  "disabled": false,
                  "description": "Base64 encoded guide definition"
                }
              ]
            },
            "description": "Uploads new guide definition.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d1a5d07-5e8b-471d-865a-bf8ee17aef2a"
            }
          ]
        },
        {
          "id": "8b8719c4-975c-4a0a-b72d-380c38d60d74",
          "name": "deleteGuide",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/:guideId"
              ],
              "variable": [
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes guide.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b26af722-7349-41ba-a29a-58023328b65c"
            }
          ]
        }
      ]
    }
  ]
}