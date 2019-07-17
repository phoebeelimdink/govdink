---
title: Information Section with Picture
permalink: /page-components/home/infopic/
third_nav_title: Home Page
---
Similar to the [information section](/page-components/home/infobar/), the information section with picture (`infopic`) can be used to provide additional information to users, and also serves as another opportunity to direct users to pages of interest. The photo and text will be placed side by side (horizontally), and the order will alternate with each successive infopic.

As the background also alternates between white and a subdued shade of blue, we strongly recommend that the whitespace background, if any, be made transparent instead of white or any other colour. The PNG file format supports transparent backgrounds. You may follow [these instructions](https://go.gov.sg/k9m2bc) to edit your image to have a transparent background.

The configuration options available are:

* `title`: the title that will be displayed in large font in the infobar

* `subtitle`: the subtitle that will be displayed in small font and all caps. *Optional*

* `description`: a short writeup where you can elaborate a little more about the topic in the section. *Optional*

* `button`: the text on the link that will appear on the bottom. *Optional together with `url`*

* `url`: the URL the link points to. *Optional together with `link`*

* `image`: the path to the image to be displayed in this section. Note that this image is compulsory. If you do not intend to use an image, use the [infobar](/page-components/home/infobar/) instead

* `alt`: a description of what is in the image. Screen readers used by people with visual impairments will read this text aloud, allowing them to understand more fully what is on your site. Hence, to maintain a high standard of accessibility, this field is compulsory

Sample configuration of 2 infopics:

```yml
- infopic:
    title: Integrity
    subtitle: Core Values
    description: Integrity drives everything we do at the Ministry of ABC
    button: Learn More
    url: /core-values/
    image: /images/integrity.png
    alt: Members of the Ministry of ABC shaking hands
- infopic:
    title: Professionalism
    subtitle: Core Values
    description: We strive to deliver work of the highest calibre
    button: Learn More
    url: /core-values/
    image: /images/professionalism.png
    alt: Members of the Ministry of ABC in suits
```