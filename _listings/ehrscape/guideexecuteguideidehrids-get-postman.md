{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs Execute guide on given EHR IDs",
    "_postman_id": "2de913c8-f211-4945-8bb0-6afecfade4d0",
    "description": "Execute guide on given ehr ids.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "2d93b5ce-ae7a-4095-b557-4a1538868dfa",
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
              "id": "25afd705-165a-46c8-b07a-63990e82695e"
            }
          ]
        },
        {
          "id": "b13885a3-7e7a-4b8f-b449-514b45165f09",
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
              "id": "798adc40-24c8-470c-8ad5-c9e91f51da03"
            }
          ]
        }
      ]
    }
  ]
}