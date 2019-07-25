---
title: Your First Page
permalink: /getting-started/firstedit/firstpage/
third_nav_title: Your First Edit
---
The next step after editing your first page is to create a new page! As you might recall, each Isomer Markdown file look something like this:

```markdown
---
title: FAQ
permalink: /faq/
---
Hello, Isomer! This is my very first edit!
```

The stuff between the 2 sets of triple dashes is called the *front matter*. The front matter is where you configure the options for each page. Most pages will only have these 2 options (`title` and `permalink`), but some pages, like the [home page](/configuration/home/overview/) and [contact us page](/configuration/contact/overview/), have more.

![Screenshot of Isomer page with the permalink and title labelled](/images/page-anatomy.png)

Now that you know about the front matter, let's get started creating your new page! Head to the staging branch, and go into the `pages` folder. Click the 'Create new file' button (it's to the upper right hand corner). Give a file a name, such as `myfirstpage.md`. Note that as a Markdown file, the file name must end in `.md`. GitHub won't be able to automatically add that for you!

![Creating a new file in your repository](/images/resources/creating-a-new-file-in-your-repository.gif)

Now that you have named the file, you're free to add your content. Feel free to copy and paste the Markdown above, or write your own! If your site already has a page with the permalink `/faq/`, remember to change the permalink to something else! One of the 2 pages will not be accessible if they have the same permalinks.

Once you're done, enter a commit message, make sure the 'Commit directly to the `staging` branch.' option is selected, and hit the green commit button. Just as before, your changes are now accessible on the staging site! (you might need to enter the permalink directly into the address bar)