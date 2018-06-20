{
  "info": {
    "name": "Ehr Scape Terminology APIs Returns details about a single entity",
    "_postman_id": "20792536-fc0b-412a-a3a1-afbc288cc0e6",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "79e30682-c4a0-4164-a845-76aeff32c85a",
      "name": "listEntities",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.ehrscape.com",
          "path": [
            "terminology-adapter",
            "rest",
            "terminology/codesystem/:codeSystem/entities"
          ],
          "query": [
            {
              "key": "codelist",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "codesystemversion",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "matchvalue",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "page",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "pagesize",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "codeSystem",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "List of entities in an explicit version of a single code system"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "3445ee6b-330a-487e-8380-17d8207e0cff"
        }
      ]
    },
    {
      "id": "2b184460-ec83-4d05-83a4-fb396fab0307",
      "name": "getEntityDescription",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.ehrscape.com",
          "path": [
            "terminology-adapter",
            "rest",
            "terminology/codesystem/:codeSystem/entity/:entity"
          ],
          "query": [
            {
              "key": "codesystemversion",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "codeSystem",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "entity",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Returns details about a single entity"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "86d04f01-e4ab-4558-81fe-08fd7b7221f9"
        }
      ]
    }
  ]
}