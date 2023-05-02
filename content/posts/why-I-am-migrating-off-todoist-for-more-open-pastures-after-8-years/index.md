+++
title = "Why I Am Migrating off Todoist for More Open Pastures After 8 Years"
date = "2023-04-30T17:18:29-07:00"
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["Todoist", "Open-Source", "Second Brain", "Productivity", "Organization"]
keywords = ["Todoist", "Open-Source", "Second Brain", "Productivity", "Organization"]
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

I am migrating off of Todoist after 8 years and over 12,000 tasks completed. Todoist has been the core of my organization and productivity since I created my account on the service. It got me through college and my professional life so far. Overall, I enjoyed the service and happily paid for the business account.

{{< figure src="Todoist-Screenshot.webp" alt="Screenshot showing over 12,000 tasks completed on Todoist" position="center" caption="My Todist Karma" style="width: 403px;">}}

All was well until a few weeks ago. I changed my email as I continually de-google my life. Todoist being one of my most important accounts, I changed the account email. Logged out. Bitwarden auto-filled the new details for me. Locked out. "Incorrect email or password" for both the old email and the new one.

Luckily, it started working a few minutes later, but I couldn't shake that memory of my heart skipping a few beats when that error message popped up. How bad would it be if I was locked out of my Todoist account? Or worse, Todoist deleted my account? I realized I was completely dependent on this service. Not only were all my tasks for the last 8 years stored here. Priceless information about projects, plans, hopes, and dreams were stored in the comments, attachments, and descriptions of the tasks. I used Todoist to take quick notes, bookmark sites, and even as a makeshift CRM to keep in touch with friends and family. Needless to say, losing the account would be painful.

Beyond the pain of losing the account, this exercise got me thinking about how much I actually had in that account and the privacy concerns related to it. Sure, a hacker, rogue employee, or future acquirer[^1] wouldn't be able to drain my bank account with access to my Todoist account, but they would have access to the inside of my thoughts, plans, and dreams going back almost a decade. The thought of so many people[^2] having access that personal information, even without a malicious actor, makes me uncomfortable.[^3]

So, I decided to make a move.

I came up with some requirements:

- The data had to be stored in an open format.
  - Preferablly, the data would be stored in plain text to allow for unlimited portablity and added freedom when adding texts. This of course, would limit the ability for machines to interact with my tasks.[^4] For team projects and other situations which require collaboration, I use other tools.
- Preferablly, there would be no server.
  - I am willing to sacrifice the convience of a server and the features (like sharing/collaboration) in exchange for it not being able to go down on me.

I had a few options. There are open-source apps like [Vikunja](https://vikunja.io/), [Tasks.org](https://tasks.org) (which looks great but appears to require a in-app subscription to enable syncing, even if it via your own means), or [NextCloud Tasks](https://apps.nextcloud.com/apps/tasks) that I seriously looked at, but each one had its flaws.

[^1]: From the Todoist Privacy Policy: "If we are involved in a merger, acquisition, bankruptcy, reorganization, partnership, asset sale or other transaction, we may disclose your Information as part of that transaction.
    - [https://edit.tosdr.org/points/13293](https://edit.tosdr.org/points/13293)
    - [https://doist.com/privacy](https://doist.com/privacy)

[^2]: Selected vendors and service providers Todoist shares data with, from the [Todoist Privacy Policy](https://doist.com/privacy) (see the full list in the privacy policy).
      - "Cloud service providers who we rely on for data storage, including Microsoft Azure and Amazon Web Services who are based in the U.S."
      - "Analytics providers. We work with a number of analytics, segmentation and mobile measurement service providers who help us understand our userbase. This includes Google LLC, which is based in the U.S."
      - "Communications platform providers, who help us manage and send newsletters to you in relation to the Services. This includes SendGrid, Mailgun and MailChimp which are based in the U.S."

[^3]: There is nothing that Todoist did wrong here, per say. I would love them to open-source their clients and server, but I know that won't happen. The decision to move is more a refusal to rely on centralized apps in general than Todoist in particular. 

[^4]: I decided limiting the ability to interact with my tasks (because they are in plain-text) was a necessary trade-off and even furthers my goal to simplify my relationship with technology (more to come on that later.)