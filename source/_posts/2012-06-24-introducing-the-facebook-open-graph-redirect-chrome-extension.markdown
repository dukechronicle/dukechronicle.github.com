---
layout: post
title: "Introducing the Facebook Open Graph Redirect Chrome Extension"
date: 2012-06-24 02:23
author: Joe Levy
comments: true
sharing: true
---

How many times has this happened to you? You're on Facebook, browsing around, minding your own business, and you spy the 'Trending Articles' box in your news feed:

![Facebook Trending Article](/images/embedded/facebook-trending-article.png)

Or maybe, while checking up on a friend, you notice on their timeline an article they recently read:

![Facebook Recent Activity](/images/embedded/facebook-recent-activity.png)

You say, "Hey, that looks interesting," and you click on the article. Surprise! Instead of the article popping up you get this lovely dialog box:

![Facebook Application Sign Up](/images/embedded/facebook-og-redirect.png)

No article for you! With Facebook's recent updates, it is now possible to see what your Facebook friends are reading and watching on many websites, including Yahoo, The Washington Post, MS NBC, Social Cam, The Guardian, and Viddy, right on Facebook. However, to actually view any of the things your Facebook friends are reading / watching yourself, many websites currently force you to install their Facebook apps. Once installed, these apps will then post whatever you watch or read on their sites to Facebook! Looking at some reading material or videos that you're less than proud to say you viewed? To bad! On to your timeline it goes!

Obviously this user experience is less than ideal. I wanted to be able to click on any of these "Open Graph" links on Facebook without having to give anyone read access to my Facebook info, let alone write access! Luckily, I noticed that the urls of these facebook links always seem to contain the url to the actual piece of content they describe, even if they refuse to take you there unless you sign up for an app.

So, naturally, I made a Google Chrome extension that turns every Facebook Open Graph link into an actual link to the article -- no signing up for apps required! This extension runs seamlessly in the background -- just click any link on Facebook like you normally would, and you'll skip the app install page and go straight to the link you clicked. Just so no one gets confused, this extension does not prevent Facebook apps you install from posting content to your Facebook feed. It only prevents the dialog box asking you to install the app from appearing.

I think its pretty cool, and if you dislike the many Facebook apps that force themselves down your throat as much as I do, I encourage you to [try it out](https://chrome.google.com/webstore/detail/facebook-open-graph-redir/pgkmcdneclgkflnhdeccboiholnedeci).

I know installing anything that accesses your Facebook introduces some privacy concerns, so I also open sourced the code behind this Chrome extension, so you can take a look and see its not doing anything malicious: [https://github.com/jodoglevy/open-graph-redirect](https://github.com/jodoglevy/open-graph-redirect). If you have any improvements, feel free to issue a pull request!

So now when I click on an article about parrots on Facebook:

![Facebook Linked Article](/images/embedded/facebook-linked-article.png)

I get an article about parrots, not a sign up page! Huzzah!

**Update**: This plugin is now available for Firefox as well at [https://addons.mozilla.org/en-US/firefox/addon/facebook-opengraph-redirect/](https://addons.mozilla.org/en-US/firefox/addon/facebook-opengraph-redirect/).
