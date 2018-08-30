---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Clinical Decision Support APIs List available guides.
  description: List available guides..
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