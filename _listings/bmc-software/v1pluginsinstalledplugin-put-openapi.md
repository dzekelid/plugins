---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Install or update plugin
  version: 1.0.0
  description: Installs a plugin
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