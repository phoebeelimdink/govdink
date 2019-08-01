---
title: Information Section
permalink: /configuration/home/infobar/
third_nav_title: Home Page
---
![Screenshot of infobar with components labelled](/images/config/home-infobar.png){:style="box-shadow: 5px 10px 8px #888888"}

The information section, or `infobar`, can be used to provide additional information to users, and also serves as another opportunity to direct users to pages of interest. The infobar does not support images - if you require images, use [`infopic`](/configuration/home/infopic/) instead.

The infobar consists of the following options:

* `title`: the title that will be displayed in large font in the infobar

* `subtitle`: the subtitle that will be displayed in small font and all caps. *Optional*

* `description`: a brief write up you can add to provide the user with more information. *Optional*

* `button`: the text on the link that will appear on the bottom on the infobar. *Optional together with `url`*

* `url`: the URL the link points to. *Optional together with `link`*

Sample configuration for infobar:

```yml
- infobar:
    title: Work for the public good
    subtitle: Careers
    description: Start a fulfulling and rewarding career with the Ministry of ABC!
    button: Join Us
    url: /careers/
```