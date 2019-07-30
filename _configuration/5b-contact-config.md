---
title: Configuration
permalink: /configuration/contact/config/
third_nav_title: Contact Us
---
The configuration options available are:

* `layout`: this option must be set to `contact_us`

* `title`:  the title of the page which will be visible in the browser window

* `permalink`: the path to the page, e.g. `/contact-us/`. Except for slashes denoting a category, the permalink should be alphanumeric (consisting only of letters, numbers, and dashes). No special characters such as `?` or `%` should be used. For aesthetic reasons, we further recommend that you avoid the use of capital letters

* `agency_name`: the text that will appear after "Get in touch with". Defaults to the `title` in `_config.yml` if left unspecified. *Optional*

* `image`: an image that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to the page. If specified, the image will also be displayed at the bottom of the page. *Optional*

* `locations`: a list of addresses to be displayed. *Optional*. Each location supports the following configuration options:

  * `title`: the title or name of this location, e.g. "HQ"

  * `address`: the address of the location. See the sample configuration below for an example of a multi-line address

  * `maps_link`: a link to the address on an online map service such as Google Maps or OneMap. If left unspecified, a Google Maps link will be automatically generated from the address. *Optional*

  * `operating_hours`: a list of `days`, `time`, and `description` of the location's operating hours. *Optional*

* `contacts`: a list of contact details to be displayed. *Optional*. Each contact supports the following configuration options:

  * `title`: the title or name of this contact, e.g. "General Enquiries"

  * `content`: a list of `phone`, `email`, or `other` contacts under this title

Sample configuration of a contact us page:

```yml
---
layout: contact_us
title: Contact Us
permalink: /contact-us/
agency_name: Ministry of ABC
image: /images/contact-us.png
locations:
  - title: Main Office
    address:
        - 31 Sesame Street
        - Big Bird Building
        - Singapore 123456
    operating_hours:
      - days: Mon - Fri
        time: 8.30am - 6.00pm
        description: Closed on Public Holidays
      - days: Sat
        time: 8.30am - 12.00pm
  - title: Branch Office
    address:
        - 109 North Bridge Road
        - Singapore 179097
    maps_link: https://goo.gl/maps/C8VfxphGxT2GsfcaA
contacts:
  - title: General Enquiries & Feedback
    content:
    - phone: +65 6123 4567
    - email: enquiries@abc.gov.sg
    - other: Any text here <i>including HTML</i>
  - title: Careers
    content:
    - email: careers@abc.gov.sg
---
```

![Screenshot of a contact us page with components labelled](/images/config/contact-us-labelled.png)