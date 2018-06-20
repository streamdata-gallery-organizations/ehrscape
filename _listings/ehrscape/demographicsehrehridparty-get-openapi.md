---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Retrieves the demographics info for
    the specified party.
  description: Retrieves the demographics info for the specified party..
  version: 1.0.0
host: rest.ehrscape.com
basePath: /rest/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /composition:
    post:
      summary: Creates a new OpenEhr composition.
      description: Creates a new openehr composition..
      operationId: createComposition
      x-api-path-slug: composition-post
      parameters:
      - in: body
        name: body
        description: The composition to create, in one of the supported formats
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: committerId
        description: The external id of the committer user
      - in: query
        name: committerName
        description: The name of the committer user
      - in: query
        name: ehrId
        description: The EHR id to save the composition into
      - in: query
        name: format
        description: The format of the composition
      - in: query
        name: templateId
        description: OpenEhr template id for the composition
      responses:
        200:
          description: OK
      tags:
      - Composition
  /composition/{uid}:
    delete:
      summary: Deletes an existing OpenEhr composition.
      description: Deletes an existing openehr composition..
      operationId: deleteComposition
      x-api-path-slug: compositionuid-delete
      parameters:
      - in: query
        name: committerId
        description: The external id of the committer user
      - in: query
        name: committerName
        description: The name of the committer user
      - in: path
        name: uid
        description: Composition UID to be deleted
      responses:
        200:
          description: OK
      tags:
      - Composition
      - Uid
    get:
      summary: Loads an OpenEhr composition.
      description: Loads an openehr composition..
      operationId: getComposition
      x-api-path-slug: compositionuid-get
      parameters:
      - in: query
        name: format
        description: The format of the composition
      - in: path
        name: uid
        description: The unique ID of the composition, with or without the domain
          and version part
      responses:
        200:
          description: OK
      tags:
      - Composition
      - Uid
    put:
      summary: Updates an existing OpenEhr composition.
      description: Updates an existing openehr composition..
      operationId: updateComposition
      x-api-path-slug: compositionuid-put
      parameters:
      - in: body
        name: body
        description: The composition to create, in one of the supported formats
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: committerId
        description: The external id of the committer user
      - in: query
        name: committerName
        description: The name of the committer user
      - in: query
        name: format
        description: The format of the composition
      - in: query
        name: templateId
        description: OpenEhr template id for the composition
      - in: path
        name: uid
        description: UID of an existing composition to be updated
      responses:
        200:
          description: OK
      tags:
      - Composition
      - Uid
  /demographics/ehr/{ehrId}/party:
    get:
      summary: Retrieves the demographics info for the specified party.
      description: Retrieves the demographics info for the specified party..
      operationId: getPartyByEhrId
      x-api-path-slug: demographicsehrehridparty-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID of the party to retrieve
      - in: query
        name: when
        description: The instant of time for which to return the information about
          the party in the ISO-8601 format (2014-03-03T15:05:43
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Ehr
      - EhrId
      - Party
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