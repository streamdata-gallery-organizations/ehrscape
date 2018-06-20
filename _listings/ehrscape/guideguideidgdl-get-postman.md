{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs Returns guide definition.",
    "_postman_id": "29091664-4f96-490e-a49c-3693a07ec578",
    "description": "Returns guide definition..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "c7b82354-9890-4e50-a293-5010afa8b5db",
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
              "id": "db785e9d-060c-4d0a-9cd5-6e701ee435d5"
            }
          ]
        },
        {
          "id": "7f59d2c9-192b-4d1b-b8f5-9212d188e2e3",
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
              "id": "eab648bd-1094-4f55-b7d2-d67ba81e118d"
            }
          ]
        },
        {
          "id": "a5663364-2792-45f6-811a-2cb5198bf4a3",
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
              "id": "89a6cb38-088b-486c-b23e-03fc57a6ee62"
            }
          ]
        },
        {
          "id": "0187b25d-fcc7-4fc4-b9f8-943382f7aca5",
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
              "id": "12424e5e-88e2-4cde-840b-61a40284bd5c"
            }
          ]
        },
        {
          "id": "4b6f0d32-ad74-4c84-8034-c3d0b9baead8",
          "name": "getGuideGDL",
          "request": {
            "url": {
              "protocol": "http",
              "host": "rest.ehrscape.com",
              "path": [
                "ThinkCDS",
                "services",
                "CDSResources",
                "guide/:guideId/gdl"
              ],
              "variable": [
                {
                  "id": "guideId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns guide definition.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01a43b6d-c1cc-4ab5-a74d-ddd73465edbb"
            }
          ]
        }
      ]
    }
  ]
}