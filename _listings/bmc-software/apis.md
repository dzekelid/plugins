---
name: BMC Software
x-slug: bmc-software
description: Transform your digital enterprise with BMC IT solutions. From mainframe
  to cloud to mobile, we???ll help you drive innovation and industrial efficiency.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
x-kinRank: "8"
x-alexaRank: "27308"
tags: Plugins
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/apis.md
specificationVersion: "0.14"
apis:
- name: BMC Software Merged API - Get all plugins
  x-api-slug: v1plugins-get
  description: Gets all known plugin definitions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1plugins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1plugins-get-openapi.md
- name: BMC Software Merged API - Get plugin components
  x-api-slug: v1pluginsplugincomponents-get
  description: Finds the components associated with an installed plugin including
    metrics and dashboards
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugincomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugincomponents-get-openapi.md
- name: BMC Software Merged API - Get installed plugins
  x-api-slug: v1pluginsinstalled-get
  description: Gets plugins that are installed for the project
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalled-get-openapi.md
- name: BMC Software Merged API - Install or update plugin
  x-api-slug: v1pluginsinstalledplugin-put
  description: Installs a plugin
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-put-openapi.md
- name: BMC Software Merged API - Add private plugin
  x-api-slug: v1pluginsprivatepluginorgrepo-put
  description: |-
    Adds or updates a private plugin.
    A plugin exists as a repository in Github.
    By adding a private plugin the plugin will appear on your settings -&gt; plugins tab just like any other plugin which
    can then be installed and/or added to a relay.
    If a private plugin has the same name as an existing plugin it will override the existing plugin within your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsprivatepluginorgrepo-put-openapi.md
- name: BMC Software Merged API - Remove private plugin
  x-api-slug: v1pluginsprivateplugin-delete
  description: |-
    Removes a private plugin from your account. Use this function after adding a private plugin to make your private
    plugin disappear from available plugins in your settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsprivateplugin-delete-openapi.md
- name: BMC Software Merged API - Uninstall plugin
  x-api-slug: v1pluginsinstalledplugin-delete
  description: Uninstalls a plugin and optionally removes related dashboard(s) and
    metric(s).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsinstalledplugin-delete-openapi.md
- name: BMC Software Merged API - Get plugin
  x-api-slug: v1pluginsplugin-get
  description: Gets a single plugin definition
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/713-bmc-software.jpg
  humanURL: http://www.bmc.com
  baseURL: https:///
  tags: Monitoring, Applications, Devops, SaaS, Enterprise, Technology, ISP, API Provider,
    API Service Provider, Profiles, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/bmc-software/v1pluginsplugin-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://blogger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bmc.software.stack.network
- type: x-blog
  url: http://www.bmc.com/blogs
- type: x-blog-rss
  url: http://feeds.feedburner.com/BmcBlogs
- type: x-crunchbase
  url: https://crunchbase.com/organization/bmc
- type: x-documentation
  url: https://docs.bmc.com/docs/dashboard.action
- type: x-email
  url: customer_support@bmc.com
- type: x-email
  url: NA_Accounts_Payable@bmc.com
- type: x-email
  url: Collections_NA@bmc.com
- type: x-email
  url: education@bmc.com
- type: x-email
  url: investor@bmc.com
- type: x-email
  url: global_security@bmc.com
- type: x-email
  url: Compliance_EthicsOffice@bmc.com
- type: x-email
  url: 26Ethics@bmc.com
- type: x-email
  url: Community_Relations@bmc.com
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