---
swagger: "2.0"
x-collection-name: SwaggerHub
x-complete: 0
info:
  title: Swagger Hub Registry Deletes the provided Plugin configuration
  description: Deletes the provided plugin configuration.
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