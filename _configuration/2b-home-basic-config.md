---
title: Basic Configuration
permalink: /configuration/home/basic-config/
third_nav_title: Home Page
---
The configuration of the home page all lies in what is known as the front matter (the YAML located between the set of triple dashes `---`). To get started, specify `layout: homepage` to let Isomer be aware that it is a home page instead of a normal page. This is required for the home page to work.

The options available are:

* `title`: the title of the home page which will be visible in the browser window

* `description`: a brief writeup (<20 words) that will appear on social media such as Facebook and WhatsApp when the home page is shared

* `permalink`: the URL of the home page. In almost all cases, this value will be `/`

* `notification`: a blue banner that will appear in the hero banner that can display any notification you would like to show users, such as urgent updates. The content here can be written in HTML. *Optional*

* `sections`: a list of sections on the home page. Further details on the sections are covered in the following pages. You can refer to the sample configuration for the specific syntax of the configuration

Partial sample configuration (without sections) of a home page:

```yml
---
layout: homepage
title: Ministry of ABC
description: The Ministry of ABC is the ministry in charge of XYZ
permalink: /
notification: Initiative A will be launching soon! <a href="/register/">Register now</a>
sections:
    # Sections have been omitted, see the following pages for more details
---
```