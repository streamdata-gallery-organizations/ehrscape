---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Import CSV data.
  description: Import csv data..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
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
  /guide/{guideId}/toggleGuidePersistence:
    put:
      summary: Toggles default behaviour of persisting guide execution result.
      description: Toggles default behaviour of persisting guide execution result..
      operationId: toggleGuidePersistence
      x-api-path-slug: guideguideidtoggleguidepersistence-put
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
      - ToggleGuidePersistence
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
    post:
      summary: Queries the demographics store for matching parties.
      description: Queries the demographics store for matching parties..
      operationId: queryParties
      x-api-path-slug: demographicspartyquery-post
      parameters:
      - in: body
        name: body
        description: An array of key-value query criteria
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: maxHits
        description: Limit the query results to this many hits
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - Query
  /demographics/party/{partyId}:
    delete:
      summary: Deletes a party record from the remote demographics store.
      description: Deletes a party record from the remote demographics store..
      operationId: deleteParty
      x-api-path-slug: demographicspartypartyid-delete
      parameters:
      - in: path
        name: partyId
        description: The id of the party to delete
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - PartyId
    get:
      summary: Retrieves the demographics info for the specified party.
      description: Retrieves the demographics info for the specified party..
      operationId: getParty
      x-api-path-slug: demographicspartypartyid-get
      parameters:
      - in: path
        name: partyId
        description: The external ID of the party to retrieve
      - in: query
        name: when
        description: The instant of time for which to return the information about
          the party in the ISO-8601 format (2014-03-03T15:05:43
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - PartyId
  /ehr:
    get:
      summary: Returns the EHR for the specified subject ID and namespace.
      description: Returns the ehr for the specified subject id and namespace..
      operationId: getEhr
      x-api-path-slug: ehr-get
      parameters:
      - in: query
        name: subjectId
        description: The subject ID whose EHR needs to be located
      - in: query
        name: subjectNamespace
        description: The namespace that the subject belongs to
      responses:
        200:
          description: OK
      tags:
      - Ehr
    post:
      summary: Creates a new EHR.
      description: Creates a new ehr..
      operationId: createEhr
      x-api-path-slug: ehr-post
      parameters:
      - in: query
        name: committerName
        description: The name of the committer user
      - in: query
        name: subjectId
        description: The external ID of the user who will own this EHR
      - in: query
        name: subjectNamespace
        description: The namespace the subjectId belongs to
      responses:
        200:
          description: OK
      tags:
      - Ehr
  /ehr/status/{ehrId}:
    put:
      summary: Update EHR_STATUS of an EHR.
      description: Update ehr_status of an ehr..
      operationId: updateEhrStatus
      x-api-path-slug: ehrstatusehrid-put
      parameters:
      - in: body
        name: body
        description: EHR status
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: ehrId
        description: EHR ID
      responses:
        200:
          description: OK
      tags:
      - Ehr
      - Status
      - EhrId
  /ehr/{ehrId}:
    get:
      summary: Returns information about the specified EHR.
      description: Returns information about the specified ehr..
      operationId: getEhr
      x-api-path-slug: ehrehrid-get
      parameters:
      - in: path
        name: ehrId
        description: The ID of the EHR to return
      responses:
        200:
          description: OK
      tags:
      - Ehr
      - EhrId
  /form:
    get:
      summary: Lists Think!Ehr forms.
      description: Lists think!ehr forms..
      operationId: getForms
      x-api-path-slug: form-get
      responses:
        200:
          description: OK
      tags:
      - Form
  /form/{name}/{version}:
    get:
      summary: Loads a Think!Ehr form.
      description: Loads a think!ehr form..
      operationId: getForm
      x-api-path-slug: formnameversion-get
      parameters:
      - in: path
        name: name
        description: The name of the form
      - in: query
        name: resources
        description: Which, if any, resources to expand
      - in: path
        name: version
        description: The version of the form, such as 1
      responses:
        200:
          description: OK
      tags:
      - Form
      - Name
      - Version
  /form/{name}/{version}/resource/{resource}:
    get:
      summary: Loads a Think!Ehr form resource content.
      description: Loads a think!ehr form resource content..
      operationId: getFormResource
      x-api-path-slug: formnameversionresourceresource-get
      parameters:
      - in: query
        name: envelope
        description: Whether or not to wrap a response in a JSON object that includes
          meta-data, or just return the resource content (default)
      - in: path
        name: name
        description: The name of the form
      - in: path
        name: resource
        description: The name of the form resource
      - in: path
        name: version
        description: The version of the form, such as 1
      responses:
        200:
          description: OK
      tags:
      - Form
      - Name
      - Version
      - Resource
      - Resource
  /import/csv:
    post:
      summary: Import CSV data.
      description: Import csv data..
      operationId: importData
      x-api-path-slug: importcsv-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: committerName
        description: Committer name (if not specified username is used instead)
      - in: query
        name: composerName
        description: Composer name (if not specified username is used instead)
      - in: query
        name: converterLocale
        description: Converter locale - specify when numeric values are formatted
          in a specific locale
      - in: query
        name: subjectNamespace
        description: Subject namespace (required when using subjectIds to identify
          EHRs)
      - in: query
        name: templateId
        description: Template ID
      - in: query
        name: templateLanguage
        description: Template language
      responses:
        200:
          description: OK
      tags:
      - Import
      - Csv
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