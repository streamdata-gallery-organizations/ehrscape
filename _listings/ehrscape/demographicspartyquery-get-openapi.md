---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Queries the demographics store for
    matching parties, with the query parameters specified in the URL.
  description: Queries the demographics store for matching parties, with the query
    parameters specified in the url..
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
  /demographics/party:
    post:
      summary: Creates a new party record in the remote demographics store.
      description: Creates a new party record in the remote demographics store..
      operationId: addParty
      x-api-path-slug: demographicsparty-post
      parameters:
      - in: body
        name: body
        description: The party to create in whatever format the demographics service
          supports
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
    put:
      summary: Updates a party record in the remote demographics store.
      description: Updates a party record in the remote demographics store..
      operationId: updateParty
      x-api-path-slug: demographicsparty-put
      parameters:
      - in: body
        name: body
        description: The party to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
  /demographics/party/query:
    get:
      summary: Queries the demographics store for matching parties, with the query
        parameters specified in the URL.
      description: Queries the demographics store for matching parties, with the query
        parameters specified in the url..
      operationId: queryParties
      x-api-path-slug: demographicspartyquery-get
      parameters:
      - in: query
        name: maxHits
        description: Limit the query results to this many hits
      - in: query
        name: parameters
        description: Query parameters in the key1=value1&key2=value2 format
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - Query
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