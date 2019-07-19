---
title: Sitewide Configuration
permalink: /page-components/sitewide-config/
---
Configuration options that applies to your entire site but are not part of a component such as the footer falls under `_config.yml`, located in the topmost folder of your site's repository.

On top of the configuration options outlined below, there are also additional configuration options needed for Isomer to work properly. These configuration options have already been set up for you. Please do not edit these options.

The configuration options available are:

* `title`: the name of your site. It can be the name of your agency, name of the microsite, etc

* `url`: the production URL of your site, e.g. `https://www.abc.gov.sg`. This option is needed for features such as Facebook sharing to work properly

* `collections`: a list of all collections on your site. Refer to the [collection configuration](/page-components/pages/leftnav/) for more details

* `resources_name`: the name of your resource room. Refer to the [resource room setup](/page-components/resources/setup/) for more details

* `favicon`: the path to the favicon that will appear on the browser window

* `shareicon`: the default image that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to a page on your site. The option will be overwritten if the page has its own `image` configuration. If left unspecified, this option defaults to the navigation bar icon. *Optional*