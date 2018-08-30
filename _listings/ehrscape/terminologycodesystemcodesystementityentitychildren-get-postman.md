{
  "info": {
    "name": "Ehr Scape Terminology APIs List of all children of a single entity",
    "_postman_id": "23774e40-0947-4069-9e2d-612e761d2d4e",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "16ad539b-f70c-4c56-ba73-3d1ffbb37ec0",
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
          "id": "d82fda73-5913-4b37-bce2-910bb11f3b79"
        }
      ]
    },
    {
      "id": "954bce1c-a203-4609-ac7f-f7bd57e448a8",
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
          "id": "bcee4882-7f9d-46b4-8bd3-7c1173652add"
        }
      ]
    },
    {
      "id": "bddd5d6e-b286-4ce1-9fa8-d40e9d716390",
      "name": "listEntityChildren",
      "request": {
        "url": {
          "protocol": "http",
          "host": "rest.ehrscape.com",
          "path": [
            "terminology-adapter",
            "rest",
            "terminology/codesystem/:codeSystem/entity/:entity/children"
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
        "description": "List of all children of a single entity"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c4bb78b7-845a-48f0-ac79-47323daf5876"
        }
      ]
    }
  ]
}