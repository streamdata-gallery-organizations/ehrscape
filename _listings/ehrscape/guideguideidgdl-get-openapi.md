---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Clinical Decision Support APIs Returns guide definition.
  description: Returns guide definition..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /ThinkCDS/services/CDSResources
paths:
  /guide:
    get:
      summary: List available guides.
      description: List available guides..
      operationId: getGuides
      x-api-path-slug: guide-get
      responses:
        200:
          description: OK
      tags:
      - Guide
  /guide/execute/{guideId}/{ehrIds}:
    get:
      summary: Execute guide on given EHR IDs
      description: Execute guide on given ehr ids.
      operationId: executeGuide
      x-api-path-slug: guideexecuteguideidehrids-get
      parameters:
      - in: header
        name: Authorization
        description: ThinkEhr credentials as HTTP Basic Authorization
      - in: header
        name: Ehr-Session
        description: Active Ehr Session token
      - in: path
        name: ehrIds
        description: Comma separated list of EHR ids, * for all
      - in: path
        name: guideId
        description: Guide ID
      - in: query
        name: persist
        description: Should save result of execution into EHR?
      responses:
        200:
          description: OK
      tags:
      - Guide
      - Execute
      - GuideId
      - EhrIds
  /guide/upload:
    post:
      summary: Uploads new guide definition.
      description: Uploads new guide definition..
      operationId: uploadGuide
      x-api-path-slug: guideupload-post
      parameters:
      - in: form
        name: guide
        description: Base64 encoded guide definition
      responses:
        200:
          description: OK
      tags:
      - Guide
      - Upload
  /guide/{guideId}:
    delete:
      summary: Deletes guide.
      description: Deletes guide..
      operationId: deleteGuide
      x-api-path-slug: guideguideid-delete
      parameters:
      - in: path
        name: guideId
        description: Guide ID
      responses:
        200:
          description: OK
      tags:
      - Guide
      - GuideId
  /guide/{guideId}/gdl:
    get:
      summary: Returns guide definition.
      description: Returns guide definition..
      operationId: getGuideGDL
      x-api-path-slug: guideguideidgdl-get
      parameters:
      - in: path
        name: guideId
        description: Guide ID
      responses:
        200:
          description: OK
      tags:
      - Guide
      - GuideId
      - Gdl
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---