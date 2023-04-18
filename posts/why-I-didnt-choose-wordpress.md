+++
title = "Why I Didnt Choose Wordpress"
date = "2023-04-18T13:29:35-07:00"
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = true
hideComments = false
color = "" #color from the theme settings
draft = true
lastmod = ["lastmod", ":git", "date", "publishDate"]
+++

I have made a career out of WordPress. I am personally responsible for the security, stability, and updates of 500+ active WordPress installations (not including the few multi-sites.) Collectively, they receive hundreds of thousands of unique visitors *per day*.

I have grown to love WordPress over the years, wholeheartedly recommending it to friends, family, and clients for all sorts of use-cases, and I don't regret it. WordPress is the closest thing we have to an open website Swiss army knife. It can do pretty much anything you need from a website just fine.

Because it is opensource, it is so much better than any of the proprietary hosted alernatives. SquareSpace or Wix could jack their prices at any moment. Meanwhile, I could have a fleet of WordPress sites up on a different host within the hour.

WordPress is also relatively easy to grasp by everyday people. People who do normal work can be quickly trained on how to make posts and edit pages. This is advantageous for the developer who doesn't want to get called every time a post needs to go up, and for the user, who just wants to get back to their regular job.

That being said, if the operator knows what they are doing, *WordPress is overkill for most sites, especially informational sites and personal blogs.* That is coming from a guy who has used WordPress every day for over 10 years.

And so, I decided to go a different direction for my personal blog: Hugo, a fast, fun, simple static site generator and CMS (content management system) written in Go.

I outline my reasons in more detail below:

## WordPress's greatest strength and fatal flaw: The plugin and theme ecosystem

### Too much flexibility

I can't quite put my finger on what is wrong with the WordPress plugin and theme ecosystem. On paper, it is the best there is (perhaps of any project). There is a WordPress plugin for *everything*. I once built a hotel booking system all inside WordPress, and I still bring it up in confession from time to time.

It's that flexiblity that can often lead to problems. WordPress can easily be twisted into things that it is not designed to be. WordPress should not be used as forum software. WordPress should not be used as hotel booking software. WordPress (probably) shouldn't be used for anything but small E-Commerce builds. Sure, the operator bears a good portion of the responsiblity for installing these plugins, but it is hard for people to draw the line when they don't think about these things all day long.

While these over-reaching plugins cannot affect the mother project, at least in theory, it is clear they have influenced the development of WordPress towards this jack-of-all-trades software we have today. What started as hyper-focused blogging software, has become a bloated site-builder. Blogging isn't what it used to be, so I understand why Automattic (the corporate sponsor and maintainer of WordPress that offers the most popular WordPress hosting) has guided WordPress towards the more marketable generalist space. As I will get into later, the ability to do anything has made it good at nothing.

### Too much commericalization

While I am not against commericalization of software in general, there is something quite tiring and even icky about the WordPress ecosystem's relationship with its revenue. Do not get me wrong. There are hundreds of excellent, professionally developed plugins and themes out there that deserve to be compensated for their labor.

This quickly leads to ads, upsells, annoying banners, strategically limited functionality, etc. Unbiased analysis of WordPress plugins and themes are difficult if not impossible to come by because of the aggressive affilate marketing of the key players. Some hosts offer hundreds of dollars *per conversion* to a hosting plan.

While I understand, again, but I miss the opensource-focused spirit of the early days. When users were creating websites mostly for themselves, their friends, or their clubs and would release those improvements back to the community.

Hugo seems to have that spirit to me. Themes (including this one) are abundant and available under permissive opensource lisenses. Though it is quite a mature project, it feels like you are on the ground floor of something.

## The root of all WordPress pain: the database

This is the root of most of the complaints that will follow. WordPress requires a database. This allows for the great breadth of its functionality, stores comments, allows for complex plugins to accomplish bascially anything. It also introduces an order of magnatitude more complexity to the maintence of the site and its environment.

You probably just want to get a site and a few posts up. Now you have to worry about the database, backing it up, what effect changes will have on it, etc. It can also cause downtime or content freezes when switches environments or performing updates.

Instead, Hugo and other "static" CMSs treat content as a file, stored on a hard drive somewhere. While this does limit the breadth of its possible functionality, it is a much better way to handle 95% of what websites and blogs need to do: display text and images to the user.

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