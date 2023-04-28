+++
title = "Why I Didn't Choose Wordpress For My Blog, Despite Being a WordPress Pro"
date = "2023-04-18T13:29:35-07:00"
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["WordPress", "Hugo", "Blogging", "Opensource"]
keywords = ["WordPress", "Hugo", "Blog", "Opensource"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
draft = false
lastmod = ["lastmod", ":git", "date", "publishDate"]
license = true
content-license = "CC BY-NC-SA 4.0"
content-license-link = "https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode"
code-license = "Apache License 2.0"
code-license-link = "https://www.apache.org/licenses/LICENSE-2.0.html"
+++

I have made a career out of WordPress. I am personally responsible for the security, stability, and updates of 500+ active WordPress installations (not including the few multi-sites.) Collectively, they receive hundreds of thousands of unique visitors *per day*.

I have grown to love WordPress over the years, wholeheartedly recommending it to friends, family, and clients for all sorts of use-cases, and I don't regret it. WordPress is the closest thing we have to an open website Swiss army knife. It can do pretty much anything you need from a website just fine.

Because it is opensource, it is so much better than any of the proprietary hosted alernatives. SquareSpace or Wix could jack their prices at any moment. Meanwhile, I could have a fleet of WordPress sites up on a different host within the hour.

WordPress is also relatively easy to grasp by everyday people. People who do normal work can be quickly trained on how to make posts and edit pages. This is advantageous for the developer who doesn't want to get called every time a post needs to go up, and for the user, who just wants to get back to their regular job.

That being said, if the operator knows what they are doing, *WordPress is overkill for most sites,* especially informational sites and personal blogs. That is coming from a guy who has used WordPress every day for over 10 years.

And so, I decided to go a different direction for my personal blog: Hugo, a fast, fun, simple static site generator and CMS (content management system) written in Go.

I outline my reasons in more detail below:

## WordPress's greatest strength and fatal flaw: The plugin and theme ecosystem

### Too much flexibility

I can't quite put my finger on what is wrong with the WordPress plugin and theme ecosystem. On paper, it is the best there is (perhaps of any project). There is a WordPress plugin for *everything*. I once built a hotel booking system all inside WordPress, and I still bring it up in confession from time to time.

It's that flexiblity that can often lead to problems. WordPress can easily be twisted into unrecognizable Frankensteins. WordPress should not be used as forum software. WordPress should not be used as hotel booking software. WordPress (probably) shouldn't be used for anything but small E-Commerce builds. Sure, the operator bears a good portion of the responsiblity for installing these plugins, but it is hard for people to draw the line when they don't think about these things all day long.

It is clear these popular, expensive, and purpose-transforming plugins have pushed the development of WordPress towards this jack-of-all-trades software we have today. What started as hyper-focused blogging software, has become a bloated site-builder, capable of anything, good at nothing.[^1]

### Too much commercialization

While I am not against commercialization of software in general, there is something quite tiring and even icky about the WordPress ecosystem's relationship with its revenue. Do not get me wrong. There are hundreds of excellent, professionally developed plugins and themes out there that deserve to be compensated for their labor.

Unfortunately, this quickly leads to ads, upsells, annoying banners, strategically limited functionality, etc. Unbiased analysis of WordPress plugins and themes are difficult if not impossible to come by because of the aggressive affilate marketing of the key players. Some hosts offer hundreds of dollars *per conversion* to a hosting plan.

While I understand, again, I miss the opensource-focused spirit of the early days. When users were creating websites mostly for themselves, their friends, or their clubs and would release those improvements back to the community.

Hugo seems to have that spirit to me. Themes (including this one) are abundant and available under permissive opensource lisenses. Though it is quite a mature project, it feels like you are on the ground floor of something.

## The root of all WordPress pain: the database

### It's finicky

This is the root of most of the complaints that will follow. WordPress requires a database. This allows for the great breadth of its functionality, stores comments, allows for complex plugins to accomplish bascially anything. It also introduces an order of magnatitude more complexity to the maintence of the site and its environment.

You probably just want to get a site and a few posts up. Now you have to worry about the database, backing it up, what effect changes will have on it, etc. It can also cause downtime or content freezes when switching environments or performing updates.

Instead, Hugo and other static CMSs treat content as a file, stored on your hard drive and in git. While this does limit the breadth of its possible functionality, it is a much better way to handle 95% of what websites and blogs need to do: display text and images to the user.

Those files can now be managed through any process that the author sees fit. Because content can now be easily tracked in git, it allows for natural version control and collaboration. Version controlling content on WordPress is difficult and efforts to track WordPress content using git (or git-like systems) have been regretably abandoned.[^2]

The content is no longer tied to the platform. I can write the content for this blog using any software that can handle Markdown. While WordPress is opensource, unlocking content from the WordPress database requires expertise and time. Meanwhile, if I want to move my content off of Hugo, I simply copy some markdown files.

It also simplifies migration and backup strategies. I've got all my Hugo content stored as Markdown files in git, on a flash drive, and anywhere else I choose. My content is in a format that is exteremly interoperable.

{{< newsletter-form >}}

### It is (often) slow

Because WordPress is *dynamic*, it is slow. Everytime a user loads a page, at least most of the time, a call goes out to an SQL database. Without careful planning and tuning, this will quickly cause performance problems.

WordPress users must become experts on a half-dozen forms of caching, possibly purchase expensive performance plugins, and set up a CDN in order to provide reasonable service to their visitors.

Common WordPress plugins can cause massive performance pains in ways that are difficult to understand for professionals, likely impossible for everyday people.

Meanwhile, serving a file is as performant as it gets. That's what Hugo does, it combines everything into a single (or at most, a few) files and delivers them as soon as the request is received from the visitor's browser. There are no dynamic requests, which makes Hugo *static*.

Being static makes Hugo much easier to spread around via a CDN, because the site doesn't rely on a database and can be scaled horizontally without any issues. Hugo can even be served via s3 for a few pennies a month (depending upon the traffic).

This static approach comes with major drawbacks though. That database, as it turns out, is pretty useful. It stores comments, user accounts, and other convient things. On Hugo, if you want to do much more than display some text or images, you'll need to embed an external, often costly, or privacy-invading service on your page. You can always choose to self-host alternatives, but now you are dealing with a whole other can of worms.

## WordPress's treats writing as a second class citizen

I am saddened by the state of the WordPress editor. While Gutenberg is *okay* for basic pages, anything beyond simple columnar layouts quickly becomes overwhelming and unmanagable. The designers have chosen a flashy design over simplicity and clear presentation of the layout.

There are other WordPress editors out there. They all have major drawbacks, by definition, however, because they are all walled gardens. Want to switch editors? You're starting over. They also add bloat to your site.

I have used Elementor since it first came out, and it is more powerful and much better at handling complex layouts. Elementor, unfortunately, starts at $59 per year per site (with discounts the more you purchase), which quickly kicks it out of the budget of many projects and approaches the cost of WordPress's hosted competitors.

Worst of all, Gutenberg makes it a pain to write. Each paragraph is treated like a block (similar to Notion). This makes it relatively easy to embed a YouTube video or Tweet between your text, but writing is overly clunky. For me, writing posts in Gutenberg consists of pasting in Markdown from a real editor and going through each paragraph seperating them out into their own blocks.

This is especially tragic considering WordPress's beginnings and stated purpose: a blogging platform. How can you blog if writing sucks?

### Conclusion

I have a tricky relationship with WordPress. On the one hand, it is one of the most successful open-source projects of all time, running half the websites on the planet and making website administration accessible to everyday people. On the other, it is a clunky behemoth that has lost its way. When it is not down due to a database issue, failed update, or other issue, you are wrestling with performance issues or chopping off your left arm to purchase a new plugin.

Sure, Hugo can't do *everything* I could want a website to do, but that is the magic. It forces me to stay on target. Instead of tuning performance and wrestling settings, I can get back to writing.

[^1]: Blogging isn't what it used to be, so I understand why Automattic (the corporate sponsor and maintainer of WordPress that offers the most popular WordPress hosting) has guided WordPress towards the more marketable generalist space.

[^2]: I am speaking here about efforts to track WordPress content in git, such as [VersionPress](https://github.com/versionpress/versionpress), but there are mildly complicated ways to track WordPress plugins and themes via git, such as a [composer workflow](https://roots.io/using-composer-with-wordpress/) or plugins like [WP-Pusher.](https://wppusher.com/)
