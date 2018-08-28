---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List plugins
  description: |-
    Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
    also be shown.
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
  /rest/plugin_sets/{setId}/plugins/search:
    get:
      summary: Search plugins
      description: Searches for plugins. The search can be refined with numerous parameters.
      operationId: getRestPluginSetsSetPluginsSearch
      x-api-path-slug: restplugin-setssetidpluginssearch-get
      parameters:
      - in: query
        name: active
        description: Only search for plugins that are active / inactive
      - in: query
        name: checkRequirements
        description: Add the requirements to the response
      - in: query
        name: checkUpdate
        description: Check for updates
      - in: query
        name: in-productive
        description: Search for plugins that are in productive
      - in: query
        name: in-stage
        description: Search for plugins that are in stage
      - in: query
        name: installed
        description: Only search for installed / not installed plugins
      - in: query
        name: itemsPerPage
        description: How many plugins to include per page of the search result
      - in: query
        name: name
        description: Search for plugins with a specific name
      - in: query
        name: pluginSetId
        description: Search for plugins from a specific plugin set
      - in: path
        name: setId
      - in: query
        name: source
        description: Search for plugins from a specific source
      - in: query
        name: type
        description: Search for plugins of a given type
      responses:
        200:
          description: OK
      tags:
      - Search
      - Plugins
  /rest/plugin_sets/{setId}/plugins/{pluginId}:
    put:
      summary: Change a plugin's 'active' status for a set.
      description: Change a plugin's 'active' status for a set..
      operationId: putRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-put
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Plugins
      - Active
      - Statusa
      - Set
  /rest/plugin_sets/{setId}/plugins/{pluginId}/setPosition:
    post:
      summary: Set a plugin's position in a set
      description: Set a plugin's position in a set.
      operationId: postRestPluginSetsSetPluginsPluginSetposition
      x-api-path-slug: restplugin-setssetidpluginspluginidsetposition-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Set
      - Plugins
      - Position
      - In
      - Set
  /rest/plugins:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPlugins
      x-api-path-slug: restplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
  /rest/plugins/plugin_sets/{pluginSetId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginsPluginSetsPluginsetPlugins
      x-api-path-slug: restpluginsplugin-setspluginsetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
  /rest/plugins/search:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPluginsSearch
      x-api-path-slug: restpluginssearch-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the plugin
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the plugin (template, theme, etc
      - in: query
        name: webstoreId
        description: The ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
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