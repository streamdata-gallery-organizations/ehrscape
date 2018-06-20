{
  "info": {
    "name": "Ehr Scape Clinical Decision Support APIs List available guides.",
    "_postman_id": "cec9863f-c47d-4cbd-bd54-d4f7ea1133f7",
    "description": "List available guides..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Guide",
      "item": [
        {
          "id": "d4459acf-41e1-4fb9-a7a2-75dea9e289ef",
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
              "id": "da4eabc7-b403-4cce-8a69-fed390da8f84"
            }
          ]
        }
      ]
    }
  ]
}