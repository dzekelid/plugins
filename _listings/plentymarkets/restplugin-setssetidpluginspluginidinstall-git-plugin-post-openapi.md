---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Install a git plugin into a set
  description: Installs a git plugin into a set. Response content will be in the form
    ['gitPluginInstalled' => 'true' / 'false'].
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
    delete:
      summary: Remove a plugin from a set
      description: |-
        Removes a plugin from a set and deletes all plugin files. Response content will be 'true' if the deletion was successful,
        'false' if not. If no plugin set with the given id can be found or the plugin is not associated to the set, a 404 will be returned.
      operationId: deleteRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Plugin
      - From
      - Set
    post:
      summary: Add a plugin to a set
      description: Add a plugin to a set.
      operationId: postRestPluginSetsSetPluginsPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginid-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Plugin
      - To
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
    post:
      summary: Create a plugin
      description: Creates a plugin with empty plugin folders and a plugin.json file.
      operationId: postRestPlugins
      x-api-path-slug: restplugins-post
      parameters:
      - in: body
        name: /rest/plugins
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Plugin
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
  /rest/shop_builder/pages:
    get:
      summary: List content pages from all plugins in a given plugin set.
      description: List content pages from all plugins in a given plugin set..
      operationId: getRestShopBuilderPages
      x-api-path-slug: restshop-builderpages-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Pages
      - From
      - ""
      - Plugins
      - In
      - Given
      - Plugin
      - Set
  /rest/shop_builder/widgets:
    get:
      summary: List all widgets provided by all frontend plugins of a given plugin
        set.
      description: List all widgets provided by all frontend plugins of a given plugin
        set..
      operationId: getRestShopBuilderWgets
      x-api-path-slug: restshop-builderwidgets-get
      parameters:
      - in: query
        name: identifier
        description: Filter results by widget identifier
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Widgets
      - Provided
      - By
      - ""
      - Frontend
      - Plugins
      - Of
      - Given
      - Plugin
      - Set
  /rest/plugin_sets/{setId}/plugins/{pluginId}/install_git_plugin:
    post:
      summary: Install a git plugin into a set
      description: Installs a git plugin into a set. Response content will be in the
        form ['gitPluginInstalled' => 'true' / 'false'].
      operationId: postRestPluginSetsSetPluginsPluginInstallGitPlugin
      x-api-path-slug: restplugin-setssetidpluginspluginidinstall-git-plugin-post
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - Install
      - Git
      - Plugin
      - Into
      - Set
  /rest/plugins/{pluginId}:
    delete:
      summary: Delete a plugin
      description: |-
        Deletes a plugin. This call also deletes all plugin files in the inbox folder! To commit the deletion, the
        plugin must be provisioned in Stage or Productive. The ID of the plugin must be specified.
      operationId: deleteRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-delete
      parameters:
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
    get:
      summary: Get a plugin
      description: Gets a plugin. The ID of the plugin must be specified.
      operationId: getRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-get
      parameters:
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
    put:
      summary: Update a plugin
      description: |-
        Updates a plugin. The plugin position can be changed. The plugin can be activated or deactivated for Stage or
        Productive. The plugin can be activated or deactivated for online stores. The ID of the plugin must be
        specified.
      operationId: putRestPluginsPlugin
      x-api-path-slug: restpluginspluginid-put
      parameters:
      - in: body
        name: /rest/plugins/{pluginId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pluginId
      responses:
        200:
          description: OK
      tags:
      - Plugin
  /rest/plugins/{pluginId}/plugin_sets/{pluginSetId}:
    delete:
      summary: Delete a plugin
      description: |-
        Deletes a plugin. This call also deletes all plugin files in the inbox folder! To commit the deletion, the
        plugin must be provisioned in Stage or Productive. The ID of the plugin must be specified.
      operationId: deleteRestPluginsPluginPluginSetsPluginset
      x-api-path-slug: restpluginspluginidplugin-setspluginsetid-delete
      parameters:
      - in: path
        name: pluginId
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - Plugin
  /rest/shop_builder/content_links:
    get:
      summary: List all content links for a given plugin set
      description: List all content links for a given plugin set.
      operationId: getRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Content
      - Linksa
      - Given
      - Plugin
      - Set
    post:
      summary: Link a content to a a layout container of a frontend plugin.
      description: Link a content to a a layout container of a frontend plugin..
      operationId: postRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-post
      parameters:
      - in: body
        name: /rest/shop_builder/content_links
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Link
      - Content
      - To
      - A
      - Layout
      - Container
      - Of
      - Frontend
      - Plugin
  /rest/user/backend_pluginset:
    get:
      summary: get the backend plugin set for user
      description: Get the backend plugin set for user.
      operationId: getRestUserBackendPluginset
      x-api-path-slug: restuserbackend-pluginset-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Backend
      - Plugin
      - Setuser
    post:
      summary: set the backend plugin set for user
      description: Set the backend plugin set for user.
      operationId: postRestUserBackendPluginset
      x-api-path-slug: restuserbackend-pluginset-post
      responses:
        200:
          description: OK
      tags:
      - Set
      - Backend
      - Plugin
      - Setuser
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