---
title: Carousel
permalink: /page-components/home/carousel/
third_nav_title: Home Page
---
The carousel is a series of images and text that will rotate throughout the page. You can use this section to showcase various aspects of your agency, programs, or initiatives.

However, we advise you to use this section judiciously and avoid adding too many images as they can increase they can more than double the page load time. To avoid overuse of the carousel section, we have made the decision to limit the number of carousels allowed on the home page to a maximum of one.

The background alternates between cyan, sky blue, and red. Hence, we strongly recommend that the whitespace background, if any, be made transparent instead of white or any other colour. The PNG file format supports transparent backgrounds. You may follow [these instructions](https://go.gov.sg/k9m2bc) to edit your image to have a transparent background.

The carousel takes in a list of items. The configuration options available for each item are:

* `title`: the title of the item, which will appear in bold text

* `subtitle`: the subtitle which will appear in small font and all caps above the title. *Optional*

* `description`: a brief writeup about the element. Note that due to space constraints, the description will not be visible on mobile devices. *Optional*. If omitted, the title and subtitle will be positioned in the bottom-center instead of the bottom-left of the carousel

* `image`: the path to the element's image. 

* `alt`: a description of what is in the image. Screen readers used by people with visual impairments will read this text aloud, allowing them to understand more fully what is on your site. If left unspecified, this field will default to the title. We strongly recommend you fill in this field to maintain a high standard of accessibility

Sample configuration of a carousel:

```yml
- carousel:
  - title: Initiative A
    subtitle: services
    description: Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet asperiores dicta distinctio enim harum labore libero magni non tempora ullam.
    image: /images/initiative-a.png
    alt: Employees taking part in Initiative A
  - title: Initiative B
    subtitle: services
    image: /images/initiative-b.png
    alt: Employees handing out hampers to underserved citizens
  - title: Initiative C
    subtitle: services
    description: Maecenas nec pretium eros, sed gravida tortor. Cras suscipit a dolor vel vehicula.
    image: /images/initiative-c.png
    alt: Citizens providing their feedback to grassroots leaders
```