---
title: YAML Syntax
permalink: /tutorial/front-matter/syntax/
third_nav_title: Front Matter
---
Like all languages, YAML has its own 'grammar', known as syntax. Syntax are a list of rules that you have to follow in order for the YAML to be properly understood. There are quite a number of rules in YAML, but we'll just cover what you need to know.

The most important thing in YAML is the spacing. Certain lines have extra spaces at the front. See this sample extract from a home page's front matter:

```yml
resources:
  title: Media
  subtitle: Learn more
  button: Contact Us
```

In this example, there is a `resources` section. The `title`, `subtitle`, and `button` properties each have 2 spaces at the front. This means that the 3 properties are describing the `resources` section, instead of the whole page.

The next thing you should know about YAML are lists. Here's an extract from a dropdown menu:

```yml
options:
  - title: Option A
    url: /page-a/
  - title: Option B 
    url: /page-b/
  - title: Option C
    url: /page-c/
```

A dropdown menu will have multiple options. This is when we need to use a list. Each item in a list is specified by adding a dash (`-`). Note that `url`, which is part of the option together with `title`, must be vertically aligned with `title`.

This is more or less what you need to know for YAML. Don't worry if you don't know the specific options to use for each page - you can always refer to the [configuration options](/configuration/navbar/overview/) for the details. All you need right now is to understand when the extra spaces are needed, and when lists are needed.

As a final note, if you have special characters like `#` in your YAML, it is a good idea to wrap the entire text in double quotes, like so:

```yml
title: "#hashtags"
```