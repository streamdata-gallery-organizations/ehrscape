---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Gets medications prescribed for a
    a patient
  description: Gets medications prescribed for a a patient.
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
  /presentation:
    post:
      summary: Returns presentation documents for a specified AQL query.
      description: Returns presentation documents for a specified aql query..
      operationId: getPresentationDocuments
      x-api-path-slug: presentation-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Presentation
  /query:
    get:
      summary: Returns the results of the specified AQL query.
      description: Returns the results of the specified aql query..
      operationId: query
      x-api-path-slug: query-get
      parameters:
      - in: query
        name: aql
        description: The AQL query to execute
      responses:
        200:
          description: OK
      tags:
      - Query
    post:
      summary: Querying with named parameter support.
      description: Querying with named parameter support..
      operationId: query
      x-api-path-slug: query-post
      parameters:
      - in: body
        name: body
        description: A JSON object representing the AQL query and its parameters (see
          model)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Query
  /session:
    delete:
      summary: Closes an OpenEhr session.
      description: Closes an openehr session..
      operationId: close
      x-api-path-slug: session-delete
      parameters:
      - in: header
        name: Ehr-Session
        description: The ID of the session to close
      - in: query
        name: sessionId
        description: The ID of the session to close
      responses:
        200:
          description: OK
      tags:
      - Session
    post:
      summary: Creates a new OpenEhr session.
      description: Creates a new openehr session..
      operationId: login
      x-api-path-slug: session-post
      parameters:
      - in: query
        name: password
        description: Password
      - in: query
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Session
    put:
      summary: Pings an OpenEhr session.
      description: Pings an openehr session..
      operationId: ping
      x-api-path-slug: session-put
      parameters:
      - in: header
        name: Ehr-Session
        description: The ID of the session to ping
      - in: query
        name: sessionId
        description: The ID of the session to ping
      responses:
        200:
          description: OK
      tags:
      - Session
  /session/ehr/{ehrId}:
    put:
      summary: Sets the EHR on the session.
      description: Sets the ehr on the session..
      operationId: useEhr
      x-api-path-slug: sessionehrehrid-put
      parameters:
      - in: header
        name: Ehr-Session
        description: The ID of the session to set the EHR on
      - in: path
        name: ehrId
        description: The ID of the EHR to set on the session
      - in: query
        name: sessionId
        description: The ID of the session to set the EHR on
      responses:
        200:
          description: OK
      tags:
      - Session
      - Ehr
      - EhrId
  /session/ehr/{subjectNamespace}/{subjectId}:
    put:
      summary: Sets the EHR on the session (via subject namespace and ID).
      description: Sets the ehr on the session (via subject namespace and id)..
      operationId: findAndUseEhr
      x-api-path-slug: sessionehrsubjectnamespacesubjectid-put
      parameters:
      - in: header
        name: Ehr-Session
        description: The ID of the session to set the EHR on
      - in: query
        name: sessionId
        description: The ID of the session to set the EHR on
      - in: path
        name: subjectId
        description: The subject ID
      - in: path
        name: subjectNamespace
        description: The namespace where the subject ID lives
      responses:
        200:
          description: OK
      tags:
      - Session
      - Ehr
      - SubjectNamespace
      - SubjectId
  /smart/records/{ehrId}/{modelName}:
    get:
      summary: Returns SMART records for a patient.
      description: Returns smart records for a patient..
      operationId: getRecords
      x-api-path-slug: smartrecordsehridmodelname-get
      parameters:
      - in: path
        name: ehrId
        description: EHR id
      - in: path
        name: modelName
        description: SMART model name
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Records
      - EhrId
      - ModelName
  /smart/records/{ehrId}/{modelName}/{recordId}:
    get:
      summary: Returns specific SMART record for a patient.
      description: Returns specific smart record for a patient..
      operationId: getRecord
      x-api-path-slug: smartrecordsehridmodelnamerecordid-get
      parameters:
      - in: path
        name: ehrId
        description: EHR id
      - in: path
        name: modelName
        description: SMART model name
      - in: path
        name: recordId
        description: Record id
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Records
      - EhrId
      - ModelName
      - RecordId
  /tagging:
    delete:
      summary: Delete a composition's tags.
      description: Delete a composition's tags..
      operationId: deleteTags
      x-api-path-slug: tagging-delete
      parameters:
      - in: body
        name: body
        description: The tag request object specifies tags on what AQL paths to delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tagging
    get:
      summary: Returns objects matching the specified tags.
      description: Returns objects matching the specified tags..
      operationId: findObjectsWithTags
      x-api-path-slug: tagging-get
      parameters:
      - in: query
        name: includeCurrentlyDeleted
        description: Whether or not to include compositions whose current (last) version
          is deleted
      - in: query
        name: includeDeletedVersions
        description: Whether or not to include deleted composition versions
      - in: query
        name: tags
        description: A collection of tags that the returned objects need to be tagged
          with (a conjunction)
      - in: query
        name: versionsToReturn
        description: Which composition versions to return
      responses:
        200:
          description: OK
      tags:
      - Tagging
    post:
      summary: Tags the specified composition and/or its sub-structures.
      description: Tags the specified composition and/or its sub-structures..
      operationId: tag
      x-api-path-slug: tagging-post
      parameters:
      - in: body
        name: body
        description: The tag request object specifies what to tag and how
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tagging
  /tagging/{compositionUid}:
    get:
      summary: Returns tags for the specified composition.
      description: Returns tags for the specified composition..
      operationId: getTags
      x-api-path-slug: taggingcompositionuid-get
      parameters:
      - in: path
        name: compositionUid
        description: The ID of the composition whose tags to return
      responses:
        200:
          description: OK
      tags:
      - Tagging
      - CompositionUid
  /template:
    get:
      summary: Gets all template ids.
      description: Gets all template ids..
      operationId: getAllTemplates
      x-api-path-slug: template-get
      responses:
        200:
          description: OK
      tags:
      - Template
    post:
      summary: Uploads an operational template.
      description: Uploads an operational template..
      operationId: saveTemplate
      x-api-path-slug: template-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Template
  /template/{templateId}:
    delete:
      summary: Deletes an existing OpenEHR template.
      description: Deletes an existing openehr template..
      operationId: deleteTemplate
      x-api-path-slug: templatetemplateid-delete
      parameters:
      - in: path
        name: templateId
        description: The ID of the template to delete
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
    get:
      summary: Loads an OpenEhr web template.
      description: Loads an openehr web template..
      operationId: getTemplate
      x-api-path-slug: templatetemplateid-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the returned web template with
      - in: query
        name: languages
        description: Other languages to include in the returned web template, separated
          by a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
  /template/{templateId}/example:
    get:
      summary: Returns an example of data values for a web template.
      description: Returns an example of data values for a web template..
      operationId: getTemplateExample
      x-api-path-slug: templatetemplateidexample-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the web template with
      - in: query
        name: exampleFilter
        description: The type of example to produce - intended for input (sent to
          the server), output (received back from the server) etc
      - in: query
        name: format
        description: The format of JSON representation of the example composition
          to return
      - in: query
        name: languages
        description: Other languages to include in the web template, separated by
          a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
      - Example
  /view/{ehrId}/allergy:
    get:
      summary: Gets allergies for a patient
      description: Gets allergies for a patient.
      operationId: get_allergy
      x-api-path-slug: viewehridallergy-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Ergy
  /view/{ehrId}/blood_pressure:
    get:
      summary: Gets recorded blood pressures for a patient
      description: Gets recorded blood pressures for a patient.
      operationId: get_blood_pressure
      x-api-path-slug: viewehridblood-pressure-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Blood
      - Pressure
  /view/{ehrId}/body_temperature:
    get:
      summary: Gets recorded body temperatures for a patient
      description: Gets recorded body temperatures for a patient.
      operationId: get_body_temperature
      x-api-path-slug: viewehridbody-temperature-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Body
      - Temperature
  /view/{ehrId}/height:
    get:
      summary: Gets recorded heights for a patient
      description: Gets recorded heights for a patient.
      operationId: get_height
      x-api-path-slug: viewehridheight-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Height
  /view/{ehrId}/labs:
    get:
      summary: Lab results
      description: Lab results.
      operationId: get_labs
      x-api-path-slug: viewehridlabs-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Labs
  /view/{ehrId}/medication:
    get:
      summary: Gets medications prescribed for a a patient
      description: Gets medications prescribed for a a patient.
      operationId: get_medication
      x-api-path-slug: viewehridmedication-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID
      - in: query
        name: from
        description: Limit by date from
      - in: query
        name: limit
        description: Maximum number of results to return (default = 10, max = 100)
      - in: query
        name: to
        description: Limit by date to
      responses:
        200:
          description: OK
      tags:
      - View
      - EhrId
      - Medication
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