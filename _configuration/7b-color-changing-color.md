---
title: Changing Colors
permalink: /configuration/color/changing-color/
third_nav_title: Website Colors
---
![How to change the colors for your website](/images/resources/website-color-change.gif)

The color is set in `misc/custom.scss`. You will find these 3 values in the file: `$primary`, `$secondary`, and `$secondary-hover`. Adjust the [hex codes](https://www.color-hex.com/) for these 3 values accordingly. Note that the semicolon (`;`) is required at the end of each line.

Sample configuration:

```scss
// Website brand colors
$primary: #6031b6;
$secondary: #4372d6;
$secondary-hover: darken(#4372d6, 20%);
```

---

![How to change the colors for your resources page](/images/resources/changing-color-for-your-resources-page.gif)

To change the resource room colors, edit the `$media-color-...` values in the same file (`misc/custom.scss`):

```scss
// Resources page colors
$media-color-one: #49759a;
$media-color-two: #744d9f;
$media-color-three: #00838f;
$media-color-four: #00838f;
$media-color-five: #00838f;
```
