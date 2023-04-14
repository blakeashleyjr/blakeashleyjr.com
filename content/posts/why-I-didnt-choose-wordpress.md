+++
title = "Why I Didnt Choose Wordpress"
date = "2023-04-13T20:12:33-07:00"
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["WordPress", "Hugo"]
keywords = ["WordPress", "Hugo"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
+++

I have made a career out of WordPress. I am personally responsible for the security, stability, and updates of 1000+ active WordPress installations (not including the few multi-sites.) Collectively, they receive hundreds of thousands of unique visitors *per day*. 

I have grown to love WordPress over the years, wholeheartedly recommending it to friends, family, and clients for all sorts of use-cases, and I don't regret it (mostly.)

As a hard-earned WordPress guy, I

WordPress is overkill for most sites, especially informational sites and personal blogs.

WordPress and its ecosystem are truly magnificent, a great example of what FOSS can do for the internet. WordPress can do anything, from run a hotel booking system, a forum, or, wait for it, a blog. That ability to do anything (accomplished by the most robust plugin and theme ecosystem on the planet) is WordPress's greatest strength, and it's fatal flaw. That unmatched ability comes with great complexity (and lots of broken sites).

And so, I decided to go a different direction for my personal blog: Hugo, a fast, fun, simple static site generator and CMS (content management system) written in Go.

I outline my reasons in more detail below:

### WordPress has a database

This is the root of most of the complaints that will follow. WordPress requires a database. This allows for the great breadth of its functionality, stores comments, allows for complex plugins to accomplish bascially anything. It also introduces an order of magnatitude more complexity to the maintence of the site and its environment. 

Now you have to worry about the database, backing it up, what effect changes will have on it, etc. It can also cause downtime or content freezes when switches environments or performing updates. 

Instead, Hugo and other "flat file" CMSs treat content as a file, stored on a hard drive somewhere. While this does limit the breadth of its possible functionality, it is a much better way to handle 95% of what websites and blogs need to do: display text and images to the user.

Those files can be tracked in git and managed through any process that the author sees fit. Because content can now be easily tracked in git, it allows for natural version control and collaboration. Version controlling content on WordPress is difficult and efforts to track WordPress content using git have been regretably abandoned.

The content is no longer tied to the platform. I can write the content for this blog using any software that can handle Markdown.

It also simplifies migration and backup strategies. Let's say I want to leave Hugo. No problem. I've got all my posts stored as Markdown files in git, on a flash drive, and anywhere else I see fit. My content is in a format that is exteremly interoperable. Meanwhile, WordPress content still belongs to me, but it is locked in an SQL database that will take expertise and time to migrate to another platform.

### WordPress is slow

Because WordPress is *dynamic*, it is slow. (I told you the database was the root of all evil.) Everytime a user loads a page, at least by default, a call goes out to an SQL database. Without careful planning and tuning, this will quickly bring a site with even minimal traffic to its knees. 

WordPress users must become experts on a half-dozen forms of caching, possibly purchase expensive performance plugins, and set up a CDN in order to provide reasonable service to their visitors.

Common WordPress plugins can cause massive performance pains in ways that are difficult to understand for professionals, likely impossible for every day people.

Meanwhile, serving a file is as performant as it gets. That's what Hugo does, it compresses everything into a single (or at most, a few) files and delivers them as soon as the request is received from the visitor's browser. There are no dynamic requests, which makes Hugo *static*.

Being static makes Hugo much easier to spread around via a CDN, because the site doesn't rely on a database and can be scaled horizontally without any issues. Hugo can even be served via s3.

### WordPress is prone to breaking

WordPress breaks, *a lot.* In fact, I've built my career on WordPress breaking, so trust me.

### WordPress's treats writing as a second class citizen

### (related) WordPress's editor ecosytem is a mess

### (Personal Preference) WordPress is written in PHP

### The WordPress ecosystem always has an upsell

I can host this blog in s3 for less than a $1 a month or for free on something like CloudFlare pages!

The WordPress ecosystem is heavily commericalized

### Conclusion

WordPress is amazing software, one of the first I fell in love with.

The WordPress ecosystem is heavily commericalized. In many ways, this is 