---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Terminology APIs List of all children of a single entity
  description: ""
  version: 1.0.0
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /terminology/codesystem/{codeSystem}/entities:
    get:
      summary: List of entities in an explicit version of a single code system
      description: ""
      operationId: listEntities
      x-api-path-slug: terminologycodesystemcodesystementities-get
      parameters:
      - in: query
        name: codelist
        description: Filter to results whose code exactly matches one of the codes
          in this list
      - in: path
        name: codeSystem
        description: Identifying code of the codesystem
      - in: query
        name: codesystemversion
        description: Version of the codesystem
      - in: query
        name: matchvalue
        description: Filter to results that contain this value, either in code or
          description
      - in: query
        name: page
        description: Page of results to return
      - in: query
        name: pagesize
        description: Size of a single page
      responses:
        200:
          description: OK
      tags:
      - ""
  /terminology/codesystem/{codeSystem}/entity/{entity}:
    get:
      summary: Returns details about a single entity
      description: ""
      operationId: getEntityDescription
      x-api-path-slug: terminologycodesystemcodesystementityentity-get
      parameters:
      - in: path
        name: codeSystem
        description: Identifying code of the codesystem
      - in: query
        name: codesystemversion
        description: Version of the codesystem
      - in: path
        name: entity
        description: code of the parent entity
      responses:
        200:
          description: OK
      tags:
      - ""
  /terminology/codesystem/{codeSystem}/entity/{entity}/children:
    get:
      summary: List of all children of a single entity
      description: ""
      operationId: listEntityChildren
      x-api-path-slug: terminologycodesystemcodesystementityentitychildren-get
      parameters:
      - in: query
        name: codelist
        description: Filter to results whose code exactly matches one of the codes
          in this list
      - in: path
        name: codeSystem
        description: Identifying code of the codesystem
      - in: query
        name: codesystemversion
        description: Version of the codesystem
      - in: path
        name: entity
        description: code of the parent entity
      - in: query
        name: matchvalue
        description: Filter to results that contain this value, either in code or
          description
      - in: query
        name: page
        description: Page of results to return
      - in: query
        name: pagesize
        description: Size of a single page
      responses:
        200:
          description: OK
      tags:
      - ""
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