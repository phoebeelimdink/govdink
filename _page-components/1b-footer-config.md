---
title: Configuration
permalink: /page-components/footer/configuration/
third_nav_title: Footer
---
```yaml
contact_us: /contact-us/
show_reach: true
feedback: https://form.gov.sg/#!/5a9ce876b3a3b6006e6b8335
faq: /faq/
privacy_policy: /privacy-policy/
terms_of_use: /terms-of-use/
copyright_agency: Your Agency Name
social_media:
    facebook: https://www.facebook.com/YourFBPage
    twitter: https://www.twitter.com/YourTwitter
    youtube: https://www.youtube.com/YourYoutube
    instagram: https://www.instagram.com/your.insta/
    linkedin: https://www.linkedin.com/company/YourAgency
links:
  - title: Sample Collection
    collection: sample-collection
  - title: Resource Room
    resource_room: true
  - title: Single Page
    url: /some-page/
  - title: Custom Sublinks
    url: /some-page-a/
    sublinks:
      - title: Subitem 1
        url: /some-page-a/
      - title: Subitem 2
        url: /some-page-b/
      - title: Subitem 3
        url: /some-page-c/
```
The footer configuration file is located at `_data/footer.yml` and consists of the following configuration options:

* `contact_us`: the URL to the page with your agency's contact information. *Optional*

* `show_reach`: set this value to `true` to show a link to [REACH](https://www.reach.gov.sg/). *Optional*

* `feedback`: the URL to the feedback form for the site. The [Digital Service Standards](https://www.tech.gov.sg/digital-service-standards/) requires all web-based digital services and mobile applications to provide a mean for users to provide feedback. We strongly recommend you create a feedback form using [FormSG](https://form.gov.sg/)

* `faq`: the URL to your site's frequently asked questions page. *Optional*

* `privacy_policy`: the URL to your site's privacy statement. The privacy policy URL defaults to `/privacy/` if left unspecified. We strongly recommend you prepare a privacy statement prior to site launch. Your agency's legal department should be able to provide you with the necessary assistance.

* `terms_of_use`: the URL to your site's terms of use. This URL defaults to `/terms-of-use/` if left unspecified. We strongly recommend you prepare the terms of use prior to site launch. Your agency's legal department should be able to provide you with the necessary assistance.

* `copyright_agency`: the name of the agency to be displayed in the copyright notice on the bottom right of the footer. *Optional*, defaults to your site title in `_config.yml` if left unspecified

* `social_media`: a list of links to your agency's social media profiles. *Optional*. The supported social media platforms are:

  * `facebook`
  * `twitter`
  * `youtube`
  * `instagram`
  * `linkedin`

* `links`: a list of links to display in the footer, in the same format as that of the [navigation bar](/page-components/navbar/configuration/). *Optional*, defaults to the same list as the navigation bar if left unspecified. This option should only be used if there are links you do not wish to include in the footer, or additional links you want to include in the footer but not in the navigation bar. Note that links with titles "FAQ" or "Contact Us" are automatically removed as their links are placed separately in the footer (see above).

Optional fields can be omitted entirely if not needed.