---
swagger: "2.0"
x-collection-name: Swagger
x-complete: 0
info:
  title: Swagger Hub Registry get configuration schema for the provided Plugin configuration
  description: Get configuration schema for the provided plugin configuration.
  contact:
    name: SwaggerHub
    url: http://swaggerhub.com
    email: info@swaggerhub.com
  version: 1.0.45
host: api.swaggerhub.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /plugins:
    get:
      summary: Retrieves a list of all available plugins (ignore system plugins)
      description: Retrieves a list of all available plugins (ignore system plugins).
      operationId: getAvailablePlugins
      x-api-path-slug: plugins-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /plugins/configurations:
    delete:
      summary: Deletes the provided Plugin configuration
      description: Deletes the provided plugin configuration.
      operationId: removePluginConfiguration
      x-api-path-slug: pluginsconfigurations-delete
      parameters:
      - in: body
        name: pluginConfiguration
        description: the Plugin configuration to be added or updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
    get:
      summary: Retrieves a list of enabled plugin configurations
      description: Retrieves a list of enabled plugin configurations.
      operationId: getPlugins
      x-api-path-slug: pluginsconfigurations-get
      parameters:
      - in: query
        name: limit
        description: number of results per page
      - in: query
        name: objectId
        description: plugin configuration objectId
      - in: query
        name: page
        description: page to return
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
    post:
      summary: Saves the provided Plugin configuration
      description: Saves the provided plugin configuration.
      operationId: addPluginConfiguration
      x-api-path-slug: pluginsconfigurations-post
      parameters:
      - in: body
        name: pluginConfiguration
        description: the Plugin configuration to be added or updated
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: trigger
        description: if true, also execute plugin
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
    put:
      summary: Updated the provided Plugin configuration
      description: Updated the provided plugin configuration.
      operationId: updatePluginConfiguration
      x-api-path-slug: pluginsconfigurations-put
      parameters:
      - in: body
        name: pluginConfiguration
        description: the Plugin configuration to be added or updated
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: trigger
        description: if true, also execute plugin
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
  /plugins/configurations/execute/{id}:
    post:
      summary: triggers execution of plugin configuration identified by id
      description: Triggers execution of plugin configuration identified by id.
      operationId: triggerPluginConfiguration
      x-api-path-slug: pluginsconfigurationsexecuteid-post
      parameters:
      - in: path
        name: id
        description: plugin configuration id
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
      - Execute
      - Id
  /plugins/configurations/schema:
    post:
      summary: get configuration schema for the provided Plugin configuration
      description: Get configuration schema for the provided plugin configuration.
      operationId: buildConfigurationSchema
      x-api-path-slug: pluginsconfigurationsschema-post
      parameters:
      - in: body
        name: pluginConfiguration
        description: the Plugin configuration to be added or updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Plugins
      - Configurations
      - Schema
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