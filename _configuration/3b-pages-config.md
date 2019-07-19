---
title: Configuration
permalink: /configuration/pages/config/
third_nav_title: Content Pages
---
The configuration for each page is located in the front matter, and the available configuration options are:

* `title`: the title of the page which will be visible in the browser window

* `permalink`: the path to the page, e.g. `/category/title/`. Except for slashes denoting a category, the permalink should be alphanumeric (consisting only of letters, numbers, and dashes). No special characters such as `?` or `%` should be used. For aesthetic reasons, we further recommend that you avoid the use of capital letters

* `image`: an image that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to the page. *Optional*

* `description`: a short write up that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to the page. *Optional*, defaults to the first 20 words on the page if omitted

* `recommender`: if your site has the automatic recommender system enabled, you can set this value to `false` if you do not want automated recommendations to appear on this page. Defaults to `true` if unspecified. *Optional*

* `breadcrumb`: the text on the breadcrumb link representing this page. *Optional*, defaults to the first 7 words in the title if left unspecified. All breadcrumb links will appear in all caps

* `published`: you can set this value to `false` to hide the page from the generated site. Defaults to `true` if left unspecified. *Optional*

For the vast majority of pages, you will only need to set two configuration options, `title` and `permalink`. Posts and pages with a left navigation bar have their own additional configuration options. See their page in this section for more details.

Sample configuration:

```yml
---
title: Join Us
permalink: /careers/join-us/
---
```