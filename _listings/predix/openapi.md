swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/plugins/archive/tenants/{tenant_uuid}/archives:
    get:
      summary: Get Plugins Archive Tenants Archives
      description: Get plugins archive tenants archives.
      operationId: getV1PluginsArchiveTenantsTenantUuArchives
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchives-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
  /v1/plugins/archive/tenants/{tenant_uuid}/archives/{uuid}:
    get:
      summary: Get Plugins Archive Tenants Archives
      description: Get plugins archive tenants archives.
      operationId: getV1PluginsArchiveTenantsTenantUuArchivesUu
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchivesuuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
    delete:
      summary: Delete Plugins Archive Tenants Archives
      description: Delete plugins archive tenants archives.
      operationId: deleteV1PluginsArchiveTenantsTenantUuArchivesUu
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidarchivesuuid-delete
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Archives
  /v1/plugins/archive/tenants/{tenant_uuid}/configuration:
    get:
      summary: Get Plugins Archive Tenants Configuration
      description: Get plugins archive tenants configuration.
      operationId: getV1PluginsArchiveTenantsTenantUuConfiguration
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidconfiguration-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Configuration
    post:
      summary: Post Plugins Archive Tenants Configuration
      description: Post plugins archive tenants configuration.
      operationId: postV1PluginsArchiveTenantsTenantUuConfiguration
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidconfiguration-post
      parameters:
      - in: body
        name: archivePluginConfiguration
        description: archivePluginConfiguration
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Configuration
  /v1/plugins/archive/tenants/{tenant_uuid}/staged-events:
    get:
      summary: Get Plugins Archive Tenants Staged Events
      description: Get plugins archive tenants staged events.
      operationId: getV1PluginsArchiveTenantsTenantUuStagedEvents
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidstagedevents-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Staged
      - Events