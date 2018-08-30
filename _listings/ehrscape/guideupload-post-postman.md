{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs Uploads new guide definition.",
    "_postman_id": "7eb5b9cb-7377-4fd2-a217-f915151dc544",
    "description": "Uploads new guide definition..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "61f88bff-9a80-4ce7-9d74-da5239bb6c67",
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
              "id": "9374e03d-8d71-4730-b544-bbef17bb4b02"
            }
          ]
        },
        {
          "id": "3d3022dc-0a7b-4d06-9c58-5b867705de2a",
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
              "id": "ccfdfd3d-f1b0-43af-8526-94f497f684b3"
            }
          ]
        },
        {
          "id": "7fcf84af-0619-4dd9-bb0d-e153e03b688d",
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
              "id": "270a08a9-c964-44dd-8099-283d8eb393d2"
            }
          ]
        }
      ]
    }
  ]
}