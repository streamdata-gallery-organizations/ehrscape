---
name: EhrScape
x-slug: ehrscape
description: Health app development shouldnt be harder than other verticals. EhrScape
  is all about making awesome healthcare apps easy to build and integrate into your
  environment. Healthcare computing that just works. EhrScape handles all the hard
  bits, including detailed clinical models, semantic interoperability, vendor independent
  data storage, health data query and more. Our mission is to empower you to build
  amazing healthcare apps and services. Welcome aboard. Were just getting started
  and weve got very big plans!
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: EhrScape
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/apis.md
specificationVersion: "0.14"
apis:
- name: Ehr Scape Clinical Decision Support APIs List available guides.
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: List available guides..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide
  tags: Guide
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guide-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guide-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs Execute guide on given EHR IDs
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Execute guide on given ehr ids.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide/execute/{guideId}/{ehrIds}
  tags: Guide,Execute,GuideId,EhrIds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideexecuteguideidehrids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideexecuteguideidehrids-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs Uploads new guide definition.
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Uploads new guide definition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide/upload
  tags: Guide,Upload
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideupload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideupload-post-openapi.md
- name: Ehr Scape Clinical Decision Support APIs Deletes guide.
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Deletes guide..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide/{guideId}
  tags: Guide,GuideId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideid-delete-openapi.md
- name: Ehr Scape Clinical Decision Support APIs Returns guide definition.
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Returns guide definition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide/{guideId}/gdl
  tags: Guide,GuideId,Gdl
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidgdl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidgdl-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs Toggles default behaviour of persisting
    guide execution result.
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Toggles default behaviour of persisting guide execution result..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources//guide/{guideId}/toggleGuidePersistence
  tags: Guide,GuideId,ToggleGuidePersistence
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidtoggleguidepersistence-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidtoggleguidepersistence-put-openapi.md
- name: Ehr Scape Clinical Decision Support APIs
  x-api-slug: ehr-scape-clinical-decision-support-apis
  description: Health app development shouldnt be harder than other verticals. EhrScape
    is all about making awesome healthcare apps easy to build and integrate into your
    environment. Healthcare computing that just works. EhrScape handles all the hard
    bits, including detailed clinical models, semantic interoperability, vendor independent
    data storage, health data query and more. Our mission is to empower you to build
    amazing healthcare apps and services. Welcome aboard. Were just getting started
    and weve got very big plans!
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: EhrScape
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/openapi.md
- name: Ehr Scape Electronic Health Record APIs Creates a new OpenEhr composition.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Creates a new openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//composition
  tags: Composition
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/composition-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Deletes an existing OpenEhr composition.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Deletes an existing openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//composition/{uid}
  tags: Composition,Uid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs Loads an OpenEhr composition.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Loads an openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//composition/{uid}
  tags: Composition,Uid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Updates an existing OpenEhr composition.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Updates an existing openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//composition/{uid}
  tags: Composition,Uid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Retrieves the demographics info for
    the specified party.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Retrieves the demographics info for the specified party..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/ehr/{ehrId}/party
  tags: Demographics,Ehr,EhrId,Party
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsehrehridparty-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Creates a new party record in the
    remote demographics store.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Creates a new party record in the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party
  tags: Demographics,Party
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsparty-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Updates a party record in the remote
    demographics store.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Updates a party record in the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party
  tags: Demographics,Party
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsparty-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Queries the demographics store for
    matching parties, with the query parameters specified in the URL.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Queries the demographics store for matching parties, with the query
    parameters specified in the url..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party/query
  tags: Demographics,Party,Query
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartyquery-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Queries the demographics store for
    matching parties.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Queries the demographics store for matching parties..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party/query
  tags: Demographics,Party,Query
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartyquery-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Deletes a party record from the remote
    demographics store.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Deletes a party record from the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party/{partyId}
  tags: Demographics,Party,PartyId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartypartyid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs Retrieves the demographics info for
    the specified party.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Retrieves the demographics info for the specified party..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//demographics/party/{partyId}
  tags: Demographics,Party,PartyId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartypartyid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns the EHR for the specified
    subject ID and namespace.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns the ehr for the specified subject id and namespace..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//ehr
  tags: Ehr
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehr-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Creates a new EHR.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Creates a new ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//ehr
  tags: Ehr
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehr-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Update EHR_STATUS of an EHR.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Update ehr_status of an ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//ehr/status/{ehrId}
  tags: Ehr,Status,EhrId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehrstatusehrid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns information about the specified
    EHR.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns information about the specified ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//ehr/{ehrId}
  tags: Ehr,EhrId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehrehrid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Lists Think!Ehr forms.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Lists think!ehr forms..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//form
  tags: Form
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/form-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Loads a Think!Ehr form.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Loads a think!ehr form..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//form/{name}/{version}
  tags: Form,Name,Version
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/formnameversion-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Loads a Think!Ehr form resource content.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Loads a think!ehr form resource content..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//form/{name}/{version}/resource/{resource}
  tags: Form,Name,Version,Resource,Resource
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/formnameversionresourceresource-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Import CSV data.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Import csv data..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//import/csv
  tags: Import,Csv
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/importcsv-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns presentation documents for
    a specified AQL query.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns presentation documents for a specified aql query..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//presentation
  tags: Presentation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/presentation-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns the results of the specified
    AQL query.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns the results of the specified aql query..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//query
  tags: Query
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/query-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Querying with named parameter support.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Querying with named parameter support..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//query
  tags: Query
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/query-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Closes an OpenEhr session.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Closes an openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//session
  tags: Session
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs Creates a new OpenEhr session.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Creates a new openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//session
  tags: Session
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Pings an OpenEhr session.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Pings an openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//session
  tags: Session
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Sets the EHR on the session.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Sets the ehr on the session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//session/ehr/{ehrId}
  tags: Session,Ehr,EhrId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/sessionehrehrid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Sets the EHR on the session (via subject
    namespace and ID).
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Sets the ehr on the session (via subject namespace and id)..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//session/ehr/{subjectNamespace}/{subjectId}
  tags: Session,Ehr,SubjectNamespace,SubjectId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/sessionehrsubjectnamespacesubjectid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns SMART records for a patient.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns smart records for a patient..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//smart/records/{ehrId}/{modelName}
  tags: Smart,Records,EhrId,ModelName
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/smartrecordsehridmodelname-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns specific SMART record for
    a patient.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns specific smart record for a patient..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//smart/records/{ehrId}/{modelName}/{recordId}
  tags: Smart,Records,EhrId,ModelName,RecordId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/smartrecordsehridmodelnamerecordid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Delete a composition's tags.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Delete a composition's tags..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//tagging
  tags: Tagging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns objects matching the specified
    tags.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns objects matching the specified tags..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//tagging
  tags: Tagging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Tags the specified composition and/or
    its sub-structures.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Tags the specified composition and/or its sub-structures..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//tagging
  tags: Tagging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns tags for the specified composition.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns tags for the specified composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//tagging/{compositionUid}
  tags: Tagging,CompositionUid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/taggingcompositionuid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets all template ids.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets all template ids..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//template
  tags: Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/template-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Uploads an operational template.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Uploads an operational template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//template
  tags: Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/template-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs Deletes an existing OpenEHR template.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Deletes an existing openehr template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//template/{templateId}
  tags: Template,TemplateId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs Loads an OpenEhr web template.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Loads an openehr web template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//template/{templateId}
  tags: Template,TemplateId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Returns an example of data values
    for a web template.
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Returns an example of data values for a web template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//template/{templateId}/example
  tags: Template,TemplateId,Example
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateidexample-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets allergies for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets allergies for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/allergy
  tags: View,EhrId,Ergy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridallergy-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets recorded blood pressures for
    a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets recorded blood pressures for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/blood_pressure
  tags: View,EhrId,Blood,Pressure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridblood-pressure-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets recorded body temperatures for
    a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets recorded body temperatures for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/body_temperature
  tags: View,EhrId,Body,Temperature
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridbody-temperature-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets recorded heights for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets recorded heights for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/height
  tags: View,EhrId,Height
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridheight-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Lab results
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Lab results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/labs
  tags: View,EhrId,Labs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridlabs-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets medications prescribed for a
    a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets medications prescribed for a a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/medication
  tags: View,EhrId,Medication
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridmedication-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets problems/diagnoses for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets problems/diagnoses for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/problem
  tags: View,EhrId,Problem
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridproblem-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets pulse measurements for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets pulse measurements for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/pulse
  tags: View,EhrId,Pulse
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridpulse-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets SpO2 measurements for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets spo2 measurements for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/spO2
  tags: View,EhrId,SpO2
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridspo2-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs Gets recorded weights for a patient
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Gets recorded weights for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1//view/{ehrId}/weight
  tags: View,EhrId,Weight
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridweight-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs
  x-api-slug: ehr-scape-electronic-health-record-apis
  description: Health app development shouldnt be harder than other verticals. EhrScape
    is all about making awesome healthcare apps easy to build and integrate into your
    environment. Healthcare computing that just works. EhrScape handles all the hard
    bits, including detailed clinical models, semantic interoperability, vendor independent
    data storage, health data query and more. Our mission is to empower you to build
    amazing healthcare apps and services. Welcome aboard. Were just getting started
    and weve got very big plans!
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: EhrScape
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/openapi.md
- name: Ehr Scape Terminology APIs List of entities in an explicit version of a single
    code system
  x-api-slug: ehr-scape-terminology-apis
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystem/{codeSystem}/entities
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementities-get-openapi.md
- name: Ehr Scape Terminology APIs Returns details about a single entity
  x-api-slug: ehr-scape-terminology-apis
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystem/{codeSystem}/entity/{entity}
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentity-get-openapi.md
- name: Ehr Scape Terminology APIs List of all children of a single entity
  x-api-slug: ehr-scape-terminology-apis
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystem/{codeSystem}/entity/{entity}/children
  tags: ~
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentitychildren-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentitychildren-get-openapi.md
- name: Ehr Scape Terminology APIs Resolves a list of entity codes with associated
    types into a list of actual entity codes
  x-api-slug: ehr-scape-terminology-apis
  description: <p>Resolves a list of entity codes with associated types into a list
    of actual entity codes<p>Each entity code in the input has an associated type.
    Depending on the type, the code will resolve to the following:<ul><li>fixed -
    itself<li>tree - itself and all its children</ul>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystem/{codeSystem}/resolve
  tags: ~
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystemresolve-post-openapi.md
- name: Ehr Scape Terminology APIs Validates a list of entity codes in a given code
    system
  x-api-slug: ehr-scape-terminology-apis
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystem/{codeSystem}/validate
  tags: ~
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystemvalidate-get-openapi.md
- name: Ehr Scape Terminology APIs Lists code systems matching a criteria
  x-api-slug: ehr-scape-terminology-apis
  description: Only the newest version of each code system will be returned
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest//terminology/codesystems
  tags: ~
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystems-get-openapi.md
- name: Ehr Scape Terminology APIs
  x-api-slug: ehr-scape-terminology-apis
  description: Health app development shouldnt be harder than other verticals. EhrScape
    is all about making awesome healthcare apps easy to build and integrate into your
    environment. Healthcare computing that just works. EhrScape handles all the hard
    bits, including detailed clinical models, semantic interoperability, vendor independent
    data storage, health data query and more. Our mission is to empower you to build
    amazing healthcare apps and services. Welcome aboard. Were just getting started
    and weve got very big plans!
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: EhrScape
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/openapi.md
x-common:
- type: x-contact-form
  url: https://www.ehrscape.com/contact.html
- type: x-faq
  url: https://www.ehrscape.com/index.html
- type: x-github
  url: https://github.com/ehrscape
- type: x-privacy
  url: https://www.ehrscape.com/privacy.html
- type: x-terms-of-service
  url: https://www.ehrscape.com/terms.html
- type: x-twitter
  url: https://twitter.com/ehrscape
- type: x-website
  url: https://www.ehrscape.com
- type: x-website
  url: http://ehrscape.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---