---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List all Plugins of Set
  description: Lists all active Plugins of given Set.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/shipping/returns/returns_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingReturnsReturnsServiceProversPlugins
      x-api-path-slug: restordersshippingreturnsreturns-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/orders/shipping/shipping_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingShippingServiceProversPlugins
      x-api-path-slug: restordersshippingshipping-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/plugin_sets/{pluginSetId}/languages:
    get:
      summary: List all the plugins translations for a plugin set
      description: Lists all the plugins translations for a plugin set
      operationId: getRestPluginSetsPluginsetLanguages
      x-api-path-slug: restplugin-setspluginsetidlanguages-get
      parameters:
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Translationsa
      - Plugin
      - Set
  /rest/plugin_sets/{setId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginSetsSetPlugins
      x-api-path-slug: restplugin-setssetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
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