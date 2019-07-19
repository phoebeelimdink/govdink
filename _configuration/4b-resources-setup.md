---
title: Setup
permalink: /configuration/resources/setup/
third_nav_title: Resource Room
---
If you have provided us with a sitemap, the setup of the resource room and its categories would have been completed for you. However, if you would like to create new categories or edit/rename existing ones, then you should refer to the following instructions.

To create a resource room, first create a folder (without a preceding underscore in the folder name) that will contain the whole of your resource room. Within that folder, create the file `index.html`, and add the following content:

```yml
---
layout: resources
title: Your Resource Room Name Here
---
```

Head to `_config.yml`, and set the configuration option `resources_name` to the resource room folder name.

For each resource room category, create a folder inside the resource room folder with the category name, with dashes (`-`) replacing spaces in the folder name just like permalinks. Within this folder,

1. Create a new copy of `index.html` with the following content:

   ```yml
   ---
   layout: resources-alt
   title: Your Category Name Here
   ---
   ```

2. Create a new folder named `_posts`

If you would like a resource room section to appear on the home page, follow [these instructions](/configuration/home/resources/). For the navigation bar setup, refer to [these instructions](/configuration/navbar/configuration/).

Your resource room setup is now complete and you're ready to start writing posts for your resource room! The category will be visible and functional once you have at least one post in the category.

At this stage, your directory structure for the resource room should look something like this:

```
.
└── media
    ├── category-a
    |       ├── _posts
    |       └── index.html
    ├── category-b
    |       ├── _posts
    |       └── index.html
    ├── category-c
    |       ├── _posts
    |       └── index.html
    └── index.html
```