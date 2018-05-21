---
name: BMC Software
x-slug: bmc-software
description: TrueSight Pulse responds to fluid IT demands with SaaS-based monitoring
  for real-time visibility into web-scale application metrics helping DevOps teams
  detect and diagnose problems fast.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
x-kinRank: "8"
x-alexaRank: ""
tags: Plugins
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software API Get all plugins
  x-api-slug: bmc-software-api
  description: Gets all known plugin definitions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1plugins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1plugins-get-openapi.md
- name: BMC Software API Get plugin components
  x-api-slug: bmc-software-api
  description: Finds the components associated with an installed plugin including
    metrics and dashboards
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/:plugin/components
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugincomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugincomponents-get-openapi.md
- name: BMC Software API Get installed plugins
  x-api-slug: bmc-software-api
  description: Gets plugins that are installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalled-get-openapi.md
- name: BMC Software API Install or update plugin
  x-api-slug: bmc-software-api
  description: Installs a plugin
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed/:plugin
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-put-openapi.md
- name: BMC Software API Add private plugin
  x-api-slug: bmc-software-api
  description: |-
    Adds or updates a private plugin.
    A plugin exists as a repository in Github.
    By adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which
    can then be installed and/or added to a relay.
    If a private plugin has the same name as an existing plugin it will override the existing plugin within your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/private/:plugin/:org/:repo
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsprivatepluginorgrepo-put-openapi.md
- name: BMC Software API Remove private plugin
  x-api-slug: bmc-software-api
  description: |-
    Removes a private plugin from your account. Use this function after adding a private plugin to make your private
    plugin disappear from available plugins in your settings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/private/:plugin
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsprivateplugin-delete-openapi.md
- name: BMC Software API Uninstall plugin
  x-api-slug: bmc-software-api
  description: Uninstalls a plugin and optionally removes related dashboard(s) and
    metric(s).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/installed/:plugin
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-openapi.md
- name: BMC Software API Get plugin
  x-api-slug: bmc-software-api
  description: Gets a single plugin definition
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https://///v1/plugins/:plugin
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugin-get-openapi.md
- name: BMC Software API
  x-api-slug: bmc-software-api
  description: TrueSight Pulse responds to fluid IT demands with SaaS-based monitoring
    for real-time visibility into web-scale application metrics helping DevOps teams
    detect and diagnose problems fast.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/bmc-truesight.png
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/openapi.md
x-common:
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-github
  url: https://github.com/bmcsoftware
- type: x-twitter
  url: https://twitter.com/bmcsoftware
- type: x-website
  url: http://www.bmc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---