---
title: Resource Room
permalink: /page-components/home/resources/
third_nav_title: Home Page
---
The resource room is an Isomer functionality that allows you to easily publish posts periodically, such as speeches and media releases. The resource room section will automatically feature the 3 latests posts on the home page.

To prevent duplication, the number of resource room sections is limited to a maximum of 1. There will be a link that leads to the full resource room page where all posts can be accessed. The location of this link cannot be changed.

The configuration options available are:

* `title`: the title of the section, usually the name of your resource room. *Optional*

* `subtitle`: the subtitle that will be displayed in small font and all caps above the title. *Optional*

* `button`: the text on the link that will lead to the full resource room page. *Optional*, defaults to "MORE" if unspecified

Sample configuration of a resource room section:

```yml
- resources:
    title: Media
    subtitle: Learn more
    button: View More
```