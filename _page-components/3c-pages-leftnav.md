---
title: Second and Third Level Pages
permalink: /page-components/pages/leftnav/
third_nav_title: Content Pages
---
Often, you will have a series of pages that fall under a common subcategory. For example, this page is part of a collection of pages on Isomer configuration. Pages like this is where second and third level pages, also known as "leftnav pages", shine.

Leftnav pages all fall under what is known as a [collection](https://jekyllrb.com/docs/collections/). Think of a collection as essentially a folder for your pages. The folder name must begin with an underscore (`_`), followed by the collection name. Similar to [permalinks](/page-components/pages/config/), a collection name should only consist of lower case letters, numbers, and dashes. The collection name will appear in the breadcrumbs on your leftnav page, with dashes (`-`) and underscores (`_`) in the collection name replaced by spaces. Just like all breadcrumbs on Isomer, they will appear in all caps.

If you have given us a sitemap, this structure and configuration should have been configured for you. If not, you can create a new collection by creating the collection folder, then adding the following configuration in `_config.yml`:

```yml
collections:
  collection-name:
    output: true
```

If you have multiple collections in your site, the section in `_config.yml` should look something like this:

```yml
collections:
  collection-one:
    output: true
  collection-two:
    output: true
  collection-three:
    output: true
```

Once the folder and configuration has been done, you can create and configure pages in the collection just like [normal pages](/page-components/pages/config/)! The items in the second level navigation bar on the left will be added automatically as you create new pages. For the second level navigation to appear on the main navigation bar at the top of the page, refer to the [navigation bar configuration](/page-components/navbar/overview/).

The pages will appear in alphabetical order based on their Markdown file names. Hence, the file name of each Markdown file in a collection should be prefixed with a number such as `1-` for the first page in the collection, `2-` for the second page, and so on. If there are 10 or more items in the second level navigation, add a zero in front of the single digit numbers (i.e. `01-`, `02-`, ..., `10-`, `11-`, ...)

Isomer also supports third level pages. To create a third level page, create a Markdown file just as you would for a second level page, but with the file name prefixed with a number and a letter. For example, if the third level navigation is fifth in the second level navigation, and the page is first in the third level navigation, the prefix should be `5a-`. Once the file has been created, configure the page's front matter just as you would for a normal or second level page, but with an additional option: `third_nav_title`. This title is the header that will appear on the second level navigation as well as the breadcrumbs.

The result is that when the file names are sorted alphabetically, third level pages with the same `third_nav_title` must run consecutively. Any breaks in the middle will result in breaks in the second level navigation.

Sample configuration of a third level page with file name `5a-initiative-a-overview`:
```yml
---
title: Overview
permalink: /initiatives/initiative-a/overview/
third_nav_title: Initiative A
---
```