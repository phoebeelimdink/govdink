---
title: Hero Banner
permalink: /configuration/home/hero/
third_nav_title: Home Page
---
![Screenshot of the hero banner on the home page with the components labelled](/images/config/home-hero.png)

The hero banner is the main banner on the home page. It includes a background, a call to action button or dropdown, as well as up to 4 key highlights (optional) that you can use to highlight pages and sites of importance.

The background photo should only contain scenery, people, or a pattern. It should **not** contain any text as the image will automatically be resized to fit different devices, and text included may end up being cut off or blocked by other components on the page, drastically affecting the user experience on your site. Further more, text in images cannot be read by screen readers used by people with visual impairments, affecting the accessibilty of your site.

The hero banner must be the first section in the page. Furthermore, only 1 hero banner is allowed on the home page.

The configuration options available are:

* `title`: the title that will be displayed in large font in the middle of the banner

* `subtitle`: the subtitle that will be displayed in smaller font in the middle of the banner. *Optional*

* `background`: the path to the background image in the hero banner. We recommend a resolution of 1920x720 pixels

* `button`: the text in the central call-to-action button in the hero banner. *Optional* if dropdown menu is present

* `url`: the URL linked to by the call-to-action button. *Optional* if dropdown menu is present

* `dropdown`: a dropdown menu with sublinks that *replaces* the call-to-action button. *Optional*. The options available for the dropdown menu are:

  * `title`: the title of the dropdown menu, visible when the menu has not been clicked
  * `options`: a list of `title` and `url` that form the options under the dropdown menu

* `key_highlights`: a list of up to 4 links placed at the bottom of the hero banner that you can use to highlight pages of importance. *Optional*. The options available for each key highlight are:

  * `title`: the title of the key highlight
  * `description`: the subtitle/description of the key highlight. *Optional*
  * `url`: the URL the key highlight links to

Sample configuration that includes a button without key highlights:

```yml
- hero:
    title: Ministry of ABC
    subtitle: We provide Singaporeans with XYZ services
    background: /images/banner.png
    url: /contact-us/
    button: Contact
```

Sample configuration that uses a dropdown menu instead of a button, and also includes 3 key highlights:

```yml
- hero:
    title: Ministry of ABC
    subtitle: We provide Singaporeans with XYZ services
    background: /images/banner.png
    dropdown:
        title: I want to...
        options:
        - title: Sign up for EFG
          url: /signup/
        - title: Learn more about ABC
          url: /learn-more/
    key_highlights:
        - title: ABC services
          description: Find out what ABC can do for you
          url: /services/
        - title: Our Annual Reports
          url: /annual-reports/
        - title: Join ABC
          description: Unleash your passion and be rewarded with a fulfilling career!
          url: /careers/
```