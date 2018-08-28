---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Get plugin
  version: 1.0.0
  description: Gets a single plugin definition
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/plugins:
    get:
      summary: Get all plugins
      description: Gets all known plugin definitions
      operationId: get-all-plugins
      x-api-path-slug: v1plugins-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/:plugin/components:
    get:
      summary: Get plugin components
      description: Finds the components associated with an installed plugin including
        metrics and dashboards
      operationId: get-plugin-components
      x-api-path-slug: v1pluginsplugincomponents-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/installed:
    get:
      summary: Get installed plugins
      description: Gets plugins that are installed for the project
      operationId: get-installed-plugins
      x-api-path-slug: v1pluginsinstalled-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/installed/:plugin:
    put:
      summary: Install or update plugin
      description: Installs a plugin
      operationId: install-or-update-plugin
      x-api-path-slug: v1pluginsinstalledplugin-put
      responses:
        200:
          description: OK
      tags:
      - Plugins
    delete:
      summary: Uninstall plugin
      description: Uninstalls a plugin and optionally removes related dashboard(s)
        and metric(s).
      operationId: uninstall-plugin
      x-api-path-slug: v1pluginsinstalledplugin-delete
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/private/:plugin/:org/:repo:
    put:
      summary: Add private plugin
      description: |-
        Adds or updates a private plugin.
        A plugin exists as a repository in Github.
        By adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which
        can then be installed and/or added to a relay.
        If a private plugin has the same name as an existing plugin it will override the existing plugin within your account.
      operationId: add-private-plugin
      x-api-path-slug: v1pluginsprivatepluginorgrepo-put
      parameters:
      - in: query
        name: |-
          plugin
          Name of the plugin
          org
          Github organization or user owning the plugin
          repo
          Github repository name for plugin
        type: string
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/private/:plugin:
    delete:
      summary: Remove private plugin
      description: |-
        Removes a private plugin from your account. Use this function after adding a private plugin to make your private
        plugin disappear from available plugins in your settings.
      operationId: remove-private-plugin
      x-api-path-slug: v1pluginsprivateplugin-delete
      parameters:
      - in: query
        name: |-
          plugin
          Name of plugin to remove
        type: string
      responses:
        200:
          description: OK
      tags:
      - Plugins
  /v1/plugins/:plugin:
    get:
      summary: Get plugin
      description: Gets a single plugin definition
      operationId: get-plugin
      x-api-path-slug: v1pluginsplugin-get
      parameters:
      - in: query
        name: |-
          plugin
          Name of plugin
        type: string
      responses:
        200:
          description: OK
      tags:
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