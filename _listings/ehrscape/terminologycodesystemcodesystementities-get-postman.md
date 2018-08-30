{
  "info": {
    "name": "Ehr Scape Terminology APIs List of entities in an explicit version of a single code system",
    "_postman_id": "03a9949f-68d5-464e-be37-c1789c9402cb",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "e150b373-1e5d-4660-8f05-62167e6c347e",
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
          "id": "e3ed5c3c-31ae-4679-a3dd-8e9895d03612"
        }
      ]
    }
  ]
}