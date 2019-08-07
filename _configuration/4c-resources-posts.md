---
title: Writing Posts
permalink: /configuration/resources/posts/
third_nav_title: Resource Room
---
![Screenshot of a post with the date labelled](/images/config/post-labelled.png)

To create a new resource room post, create a markdown file in the `_posts` folder of the category the post falls under. The file name must be prefixed with the post's publishing date in YYYY-MM-DD format, e.g. `2019-02-28-press-release-by-minister.md`. Posts dated in the future will not be published. Note that posts dated in the future will not automatically be published on the date either - they will only be published together with another edit on or after that date. To publish all posts, including those dated in the future, set `future: true` in `_config.yml`.

> Note: Do not put spaces in the filename of your .md file. Always replace the spaces with dash (-)

The configuration options available for posts are:

* `title`: the title of the post which will be visible in the browser window

* `permalink`: the path to the post, e.g. `/resource-room/category/title/`. Except for slashes denoting a category, the permalink should be alphanumeric (consisting only of letters, numbers, and dashes). No special characters such as `?` or `%` should be used. For aesthetic reasons, we further recommend that you avoid the use of capital letters. *Omit* this field if `file_url` is specified

* `file_url`: the path to the file to be downloaded, for downloadable posts, e.g. `/downloads/form.pdf`. Once this field is specified, the file download will begin immediately once the user clicks on the post in the resource room menu. *Omit* this field if `permalink` is specified

* `image`: an image that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to the page. *Optional*

* `description`: a short write up that will be featured by social media platforms such as Facebook and WhatsApp if a user shares a link to the page. *Optional*, defaults to the first 20 words on the page if omitted

* `recommender`: if your site has the automatic recommender system enabled, you can set this value to `false` if you do not want automated recommendations to appear on this page. Defaults to `true` if unspecified. *Optional*

* `breadcrumb`: the text on the breadcrumb link representing this page. *Optional*, defaults to the first 7 words in the title if left unspecified. All breadcrumb links will appear in all caps

* `published`: you can set this value to `false` to hide the page from the generated site. Defaults to `true` if left unspecified. *Optional*

Sample configuration of a post:

```yml
---
title: Your Title Here
permalink: /resource-room/category/title/
image: /images/title-image.jpg
description: The Ministry of ABC will be launching Initiative A to help Singaporeans...
---
```