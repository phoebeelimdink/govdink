---
title: Markdown Cheatsheet
permalink: /tutorial/markdown/cheatsheet/
third_nav_title: Markdown
---
This is intended as a quick reference and showcase, to aid you as you draft your site's pages. If you're looking for something that isn't covered here, we encourage you to refer to other more comprehensive Markdown guides on the internet. If you still feel you need more assistance, feel free to reach out to us for help through Slack or email.

### Text

```markdown
This is some normal text. *This sentence is in italics.* This **word** is in bold.
```

The above Markdown will produce:

This is some normal text. *This sentence is in italics.* This **word** is in bold.

### Headers

Headers are the big titles and subtitles on your page. For example, the headers you have seen so far on this page are "Text" and "Headers". Headers come in levels, with a level 1 header (aka `H1`) the biggest level usually used only for page titles.

```markdown
# This is a level 1 (H1) header!

## This is a level 2 (H2) header!

### This is a level 3 (H3) header!

#### This is a level 4 (H4) header!
```

The above Markdown will produce:

# This is a level 1 (H1) header!

## This is a level 2 (H2) header!

### This is a level 3 (H3) header!

#### This is a level 4 (H4) header!

### Lists

```markdown
1. First ordered list item
2. Another item
  * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the 3 leading spaces which align the raw Markdown.

* Use asterisks for unordered lists, aka bullet points
```

The above Markdown will produce:

1. First ordered list item
2. Another item
  * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces which align the raw Markdown.

* Use asterisks for unordered lists, aka bullet points

### Links

Links come in several flavours:

```markdown
[I'm a link within the site](/configuration/navbar/overview/)

[I'm an link to an external site](https://www.google.com)

[I'm an link with title - hover your mouse over me!](https://www.google.com "Google's Homepage")

URLs must be wrapped in angled brackets to turn into links: <http://www.example.com>
```

The above Markdown will produce:

[I'm a link within the site](/configuration/navbar/overview/)

[I'm an link to an external site](https://www.google.com)

[I'm an link with title - hover your mouse over me!](https://www.google.com "Google's Homepage")

URLs must be wrapped in angled brackets to turn into links: <http://www.example.com>

### Images

To place an image in your Markdown file, first [upload the image](/github-repository/uploading-a-file/) into your `/images/` folder. Then use the following Markdown syntax:

```markdown
![alt text - this is a description of what is in the image for people with visual impairments using screen readers](/images/isomer-logo.svg)

![just like links, you can include titles which appear when hovered](/images/isomer-logo.svg "Isomer Logo")
```

The above Markdown will produce:

![alt text - this is a description of what is in the image for people with visual impairments using screen readers](/images/sample-image.jpg)

![just like links, you can include titles which appear when hovered](/images/sample-image.jpg "Sample Image")