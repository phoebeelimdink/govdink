---
title: Analytics
permalink: /configuration/analytics/
---

### You've gotten your site up, now what?

You may have questions like these:
- How many people visit my website?
- Which pages on my website are the most popular?
- What content do my visitors like the most?

To give you a better understanding of how your visitors are viewing your site, you need to set up analytics on your site.
Here are two free analytics tools you can use to help you answers the questions above. 

#### 1. WOGAA
WOGAA is a whole of government analytics platform. You can start signing up for it [here](https://wogaa.sg/login). 
Go to **Manage Service** and click on **Add Service** button on the top right hand corner to get started.
![Manage Services](/images/wogaa-manage-services.png)
![Add Service](/images/wogaa-add-service.png)

#### Setting up Sentiments

Sentiments is a tool for you to quickly gather feedback about your site from your visitors.

To set up sentiments, go to **Manage Services** on your WOGAA portal and select **Manage Sentiments**. Follow the step-by-step guide on the portal, you should be able to set it up with a quick toggle of a button.
![Manage Sentiments](/images/manage-sentiments.png)
![Toggle Sentiments](/images/toggle-sentiments.png)

#### 2. Google Anlaytics
Google Analytics is an free analytics tools provided by Google. You can go [here](https://accounts.google.com/) to sign up using your google account.

Next, follow the steps below to configure Google Analytics on your site:
1. Go to your admin page, and under **Tracking Info**, select **Tracking Code**
![tracking code](/images/select-tracking-code.png)

2. Copy the **Tracking ID** on your Google Analytics
![tracking ID](/images/tracking-id.png)

3. Paste it on your **config.yml** file in your repository. You should create a field `google_analytics` if the file does not have this.
![isomer ga](/images/isomer-ga.png)
