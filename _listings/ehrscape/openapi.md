---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: Ehr Scape Terminology APIs
  description: validates-and-resolves-terminology-codes
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
  /terminology/codesystem/{codeSystem}/resolve:
    post:
      summary: Resolves a list of entity codes with associated types into a list of
        actual entity codes
      description: <p>Resolves a list of entity codes with associated types into a
        list of actual entity codes<p>Each entity code in the input has an associated
        type. Depending on the type, the code will resolve to the following:<ul><li>fixed
        - itself<li>tree - itself and all its children</ul>
      operationId: resolveEntityCodes
      x-api-path-slug: terminologycodesystemcodesystemresolve-post
      parameters:
      - in: body
        name: body
        description: list of entities to be resolved
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: codeSystem
      - in: query
        name: codesystemversion
      responses:
        200:
          description: OK
      tags:
      - ""
  /terminology/codesystem/{codeSystem}/validate:
    get:
      summary: Validates a list of entity codes in a given code system
      description: ""
      operationId: validateCodes
      x-api-path-slug: terminologycodesystemcodesystemvalidate-get
      parameters:
      - in: path
        name: codeSystem
        description: Identifying code of the codesystem
      - in: query
        name: codesystemversion
        description: Version of the codesystem
      - in: query
        name: entities
        description: Codes of the entities to validate
      responses:
        200:
          description: OK
      tags:
      - ""
  /terminology/codesystems:
    get:
      summary: Lists code systems matching a criteria
      description: Only the newest version of each code system will be returned
      operationId: listCodeSystems
      x-api-path-slug: terminologycodesystems-get
      parameters:
      - in: query
        name: codelist
        description: Filter to results whose code exactly matches one of the codes
          in this list
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
---