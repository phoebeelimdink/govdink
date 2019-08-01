---
title: What Just Happened?
permalink: /tutorial/firstedit/what-happened/
third_nav_title: Your First Edit
---
You've just made your first edit and you might be wondering what just happened, or how Isomer works.

The moment a commit is made on GitHub, GitHub sends the updated content of your site to a service called [Netlify](https://www.netlify.com/) that we use to build Isomer sites. Netlify then downloads the central Isomer theme, weaves your content into the theme, building a complete site. This build process usually take less than a minute for most Isomer sites, but larger Isomer sites can take up to 5 minutes.

You might also remember that you were asked to make sure that you are in the `staging` branch of the repository. Isomer sites will always have at least 2 branches - `staging` and `master`. The `staging` branch is where you can make edits freely without affecting your live site. Your changes can be previewed on the staging URL, which is also separate from your live site.

When you're happy with your changes and want to push them to your live site, open a pull request to the `master` branch. A pull request is essentially a request to update the content of the `master` branch to be in sync with the `staging` branch. To prevent defacement or other security incidents, we have instituted a policy where your pull request must be approved by at least 1 other user who can edit your site.