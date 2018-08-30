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
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/apis.md
specificationVersion: "0.14"
apis:
- name: Ehr Scape Clinical Decision Support APIs - List available guides.
  x-api-slug: guide-get
  description: List available guides..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guide-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guide-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs - Execute guide on given EHR IDs
  x-api-slug: guideexecuteguideidehrids-get
  description: Execute guide on given ehr ids.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideexecuteguideidehrids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideexecuteguideidehrids-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs - Uploads new guide definition.
  x-api-slug: guideupload-post
  description: Uploads new guide definition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideupload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideupload-post-openapi.md
- name: Ehr Scape Clinical Decision Support APIs - Deletes guide.
  x-api-slug: guideguideid-delete
  description: Deletes guide..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideid-delete-openapi.md
- name: Ehr Scape Clinical Decision Support APIs - Returns guide definition.
  x-api-slug: guideguideidgdl-get
  description: Returns guide definition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidgdl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidgdl-get-openapi.md
- name: Ehr Scape Clinical Decision Support APIs - Toggles default behaviour of persisting
    guide execution result.
  x-api-slug: guideguideidtoggleguidepersistence-put
  description: Toggles default behaviour of persisting guide execution result..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//ThinkCDS/services/CDSResources
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidtoggleguidepersistence-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/guideguideidtoggleguidepersistence-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Creates a new OpenEhr composition.
  x-api-slug: composition-post
  description: Creates a new openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/composition-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Deletes an existing OpenEhr composition.
  x-api-slug: compositionuid-delete
  description: Deletes an existing openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Loads an OpenEhr composition.
  x-api-slug: compositionuid-get
  description: Loads an openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Updates an existing OpenEhr composition.
  x-api-slug: compositionuid-put
  description: Updates an existing openehr composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/compositionuid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Retrieves the demographics info
    for the specified party.
  x-api-slug: demographicsehrehridparty-get
  description: Retrieves the demographics info for the specified party..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsehrehridparty-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Creates a new party record in the
    remote demographics store.
  x-api-slug: demographicsparty-post
  description: Creates a new party record in the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsparty-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Updates a party record in the remote
    demographics store.
  x-api-slug: demographicsparty-put
  description: Updates a party record in the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicsparty-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Queries the demographics store for
    matching parties, with the query parameters specified in the URL.
  x-api-slug: demographicspartyquery-get
  description: Queries the demographics store for matching parties, with the query
    parameters specified in the url..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartyquery-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Queries the demographics store for
    matching parties.
  x-api-slug: demographicspartyquery-post
  description: Queries the demographics store for matching parties..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartyquery-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Deletes a party record from the
    remote demographics store.
  x-api-slug: demographicspartypartyid-delete
  description: Deletes a party record from the remote demographics store..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartypartyid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Retrieves the demographics info
    for the specified party.
  x-api-slug: demographicspartypartyid-get
  description: Retrieves the demographics info for the specified party..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/demographicspartypartyid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns the EHR for the specified
    subject ID and namespace.
  x-api-slug: ehr-get
  description: Returns the ehr for the specified subject id and namespace..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehr-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Creates a new EHR.
  x-api-slug: ehr-post
  description: Creates a new ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehr-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Update EHR_STATUS of an EHR.
  x-api-slug: ehrstatusehrid-put
  description: Update ehr_status of an ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehrstatusehrid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns information about the specified
    EHR.
  x-api-slug: ehrehrid-get
  description: Returns information about the specified ehr..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/ehrehrid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Lists Think!Ehr forms.
  x-api-slug: form-get
  description: Lists think!ehr forms..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/form-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Loads a Think!Ehr form.
  x-api-slug: formnameversion-get
  description: Loads a think!ehr form..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/formnameversion-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Loads a Think!Ehr form resource
    content.
  x-api-slug: formnameversionresourceresource-get
  description: Loads a think!ehr form resource content..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/formnameversionresourceresource-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Import CSV data.
  x-api-slug: importcsv-post
  description: Import csv data..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/importcsv-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns presentation documents for
    a specified AQL query.
  x-api-slug: presentation-post
  description: Returns presentation documents for a specified aql query..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/presentation-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns the results of the specified
    AQL query.
  x-api-slug: query-get
  description: Returns the results of the specified aql query..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/query-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Querying with named parameter support.
  x-api-slug: query-post
  description: Querying with named parameter support..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/query-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Closes an OpenEhr session.
  x-api-slug: session-delete
  description: Closes an openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Creates a new OpenEhr session.
  x-api-slug: session-post
  description: Creates a new openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Pings an OpenEhr session.
  x-api-slug: session-put
  description: Pings an openehr session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/session-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Sets the EHR on the session.
  x-api-slug: sessionehrehrid-put
  description: Sets the ehr on the session..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/sessionehrehrid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Sets the EHR on the session (via
    subject namespace and ID).
  x-api-slug: sessionehrsubjectnamespacesubjectid-put
  description: Sets the ehr on the session (via subject namespace and id)..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/sessionehrsubjectnamespacesubjectid-put-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns SMART records for a patient.
  x-api-slug: smartrecordsehridmodelname-get
  description: Returns smart records for a patient..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/smartrecordsehridmodelname-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns specific SMART record for
    a patient.
  x-api-slug: smartrecordsehridmodelnamerecordid-get
  description: Returns specific smart record for a patient..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/smartrecordsehridmodelnamerecordid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Delete a composition's tags.
  x-api-slug: tagging-delete
  description: Delete a composition's tags..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns objects matching the specified
    tags.
  x-api-slug: tagging-get
  description: Returns objects matching the specified tags..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Tags the specified composition and/or
    its sub-structures.
  x-api-slug: tagging-post
  description: Tags the specified composition and/or its sub-structures..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/tagging-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns tags for the specified composition.
  x-api-slug: taggingcompositionuid-get
  description: Returns tags for the specified composition..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/taggingcompositionuid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets all template ids.
  x-api-slug: template-get
  description: Gets all template ids..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/template-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Uploads an operational template.
  x-api-slug: template-post
  description: Uploads an operational template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/template-post-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Deletes an existing OpenEHR template.
  x-api-slug: templatetemplateid-delete
  description: Deletes an existing openehr template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateid-delete-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Loads an OpenEhr web template.
  x-api-slug: templatetemplateid-get
  description: Loads an openehr web template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateid-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Returns an example of data values
    for a web template.
  x-api-slug: templatetemplateidexample-get
  description: Returns an example of data values for a web template..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/templatetemplateidexample-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets allergies for a patient
  x-api-slug: viewehridallergy-get
  description: Gets allergies for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridallergy-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets recorded blood pressures for
    a patient
  x-api-slug: viewehridblood-pressure-get
  description: Gets recorded blood pressures for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridblood-pressure-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets recorded body temperatures
    for a patient
  x-api-slug: viewehridbody-temperature-get
  description: Gets recorded body temperatures for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridbody-temperature-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets recorded heights for a patient
  x-api-slug: viewehridheight-get
  description: Gets recorded heights for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridheight-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Lab results
  x-api-slug: viewehridlabs-get
  description: Lab results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridlabs-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets medications prescribed for
    a a patient
  x-api-slug: viewehridmedication-get
  description: Gets medications prescribed for a a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridmedication-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets problems/diagnoses for a patient
  x-api-slug: viewehridproblem-get
  description: Gets problems/diagnoses for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridproblem-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets pulse measurements for a patient
  x-api-slug: viewehridpulse-get
  description: Gets pulse measurements for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridpulse-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets SpO2 measurements for a patient
  x-api-slug: viewehridspo2-get
  description: Gets spo2 measurements for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridspo2-get-openapi.md
- name: Ehr Scape Electronic Health Record APIs - Gets recorded weights for a patient
  x-api-slug: viewehridweight-get
  description: Gets recorded weights for a patient.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//rest/v1
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/viewehridweight-get-openapi.md
- name: Ehr Scape Terminology APIs - List of entities in an explicit version of a
    single code system
  x-api-slug: terminologycodesystemcodesystementities-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementities-get-openapi.md
- name: Ehr Scape Terminology APIs - Returns details about a single entity
  x-api-slug: terminologycodesystemcodesystementityentity-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentity-get-openapi.md
- name: Ehr Scape Terminology APIs - List of all children of a single entity
  x-api-slug: terminologycodesystemcodesystementityentitychildren-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentitychildren-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystementityentitychildren-get-openapi.md
- name: Ehr Scape Terminology APIs - Resolves a list of entity codes with associated
    types into a list of actual entity codes
  x-api-slug: terminologycodesystemcodesystemresolve-post
  description: <p>Resolves a list of entity codes with associated types into a list
    of actual entity codes<p>Each entity code in the input has an associated type.
    Depending on the type, the code will resolve to the following:<ul><li>fixed -
    itself<li>tree - itself and all its children</ul>
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystemresolve-post-openapi.md
- name: Ehr Scape Terminology APIs - Validates a list of entity codes in a given code
    system
  x-api-slug: terminologycodesystemcodesystemvalidate-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystemcodesystemvalidate-get-openapi.md
- name: Ehr Scape Terminology APIs - Lists code systems matching a criteria
  x-api-slug: terminologycodesystems-get
  description: Only the newest version of each code system will be returned
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/EHRScape-Logo.png
  humanURL: https://www.ehrscape.com
  baseURL: https://rest.ehrscape.com//terminology-adapter/rest
  tags: Healthcare, Healthcare, Target, Stack Network, API Provider, Profiles, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ehrscape/master/_listings/ehrscape/terminologycodesystems-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://ebay.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ehrscape.stack.network
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