+++
title = "My Journey to Tech Independence in 2023"
date = 2023-12-30T11:24:13-06:00
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["Security", "Privacy", "Autonomy", "De-Googling"]
keywords = ["Security", "Privacy", "Autonomy", "De-Googling"]
description = ""
showFullContent = false
readingTime = true
hideComments = true
color = "" #color from the theme settings
draft = true
lastmod = ["lastmod", ":git", "date", "publishDate"]
license = true
content-license = "CC BY-NC-SA 4.0"
content-license-link = "https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode"
code-license = "Apache License 2.0"
code-license-link = "https://www.apache.org/licenses/LICENSE-2.0.html"
+++
In an era where digital dependence is commonplace, I moved towards personal tech independence in 2023. This blog post details my transition away from mainstream tech giants and towards more secure, private, and autonomous alternatives.

## Breaking Free from the Norm

In 2023, I finally broke free from the likes of Google, Facebook, and other tech giants—a commitment I'd long made to myself but never fulfilled. Like many of you, Google and Facebook had been my internet cornerstones for years, offering convenience, cost-effectiveness, and entertainment.

On a professional level, I've always been cognizant of the threat of 'vendor lock-in'. How reliant am I on a single service, and what's the fallout if it vanishes overnight?

A personal turning point came with a widely-reported [incident](https://web.archive.org/web/20231220165251/https://www.nytimes.com/2022/08/21/technology/google-surveillance-toddler-photo.html): a father wrongfully accused by Google's algorithms of possessing child sex abuse material in his private messages. This automated and erroneous finding led to the freezing of his account and immediate notification to law enforcement.

Realizing the extent of my dependence on a few major players like Google was a wake-up call. My goal for 2023 was clear: to minimize my dependency on any single platform or service.

## Improvements I Made This Year:

### Email/Calendar
My first step was to address my email and calendar dependencies.
- **Migrated away from my 15-year-old Google account**
  - Switched to [Proton Mail](https://proton.me/) for enhanced privacy and security.[^1]
  - Transitioned to using my own domains for email.
  - Set up PGP using my own keys for secure communication.
  - Moved scheduling to Cal.com for opensource scheduling.
  - I setup [SimpleLogin](https://simplelogin.io/) to use my own domain (a throwaway) for private email forwwarding. Should SimpleLogin disappear, I could keep all these emails flowing.
- **Todo:**
  - Implement an automated [email backup system](https://proton.me/support/proton-mail-export-tool).
  - Figure out a solution for calendar synchronization.[^2]
  - Transition away from Google Photos (Currently locked-in due to family use).
  - Permanently delete my Google account after a few more months of email forwarding.

### Messaging
- **Moved (almost exclusively) to [Signal](https://signal.org/) and [Simplex](https://simplex.chat/) for private and secure messaging.**
- Successfully convinced many friends and family to switch to Signal.
- Using Simplex as a secure alternative to email for communications with strangers. 
- **Stopped using Discord**
  - I've enjoyed Matrix for quick questions and community building, despite not being a big fan of chatrooms for most use cases due to their lack of external searchability, synchronicity, etc.[^3]
- **Todo:**
  - Get the remaining friends and family on Signal.
  - Consider self-hosting my own Simplex infrastructure.
  - Migrate to a self-hosted Matrix server.

### Social Media
- **Embraced the fediverse by switching to [Mastodon](https://joinmastodon.org/) and [Lemmy](https://join-lemmy.org/).** 
- Deleted my Twitter, Reddit, Instagram, and Facebook accounts, prioritizing privacy and control over my digital social life.
- **Todo:**
  - Plan to self-host my own Mastodon and Lemmy instances.

### Web Hosting
- Migrated to a static site powered by [Hugo](https://gohugo.io/) for enhanced portability and control.
- **Todo:**
  - Move away from Cloudflare hosting for greater independence.
  - Enable Tor access to my site for increased privacy and accessibility.

### Homelab
- Undertook a massive overhaul by moving dozens of services into a self-hosted k3s cluster and Ceph storage.
- Transitioned all my physical media into [Jellyfin](https://jellyfin.org/), supporting DRM-free content and direct purchases from creators.
- Installed security cameras around my home, ensuring they operate exclusively within my LAN and backups are encrypted.
- In the process of migrating all file storage to a blend of [Nextcloud](https://nextcloud.com/) and [Syncthing](https://syncthing.net/), for a seamless and secure file management system.

### MISC
- Now using VPN and Tor exclusively for web browsing, with very few exceptions (like banking).
- Sites that block Tor and/or VPN (including incessant CAPTCHA requirements) no longer receive my patronage.

### Todo in 2024
- Do a full account audit, going through my password manager and updating emails/passwords, adding 2FA, or deleting accounts when not in use.
- Plan to replace my current Pixel device, which has a locked bootloader, with an unlocked device running [GrapheneOS.](https://grapheneos.org/)
- Intend to replace my desktop and laptop with Nvidia GPUs for a setup that fully supports Wayland with AMD or Intel GPU, then move exclusively to a Linux desktop.
- Github still has an iron hold on my code. My plan is to self-host [Forgejo](https://forgejo.org/) and mirror public repos to Github. I hope the [Activitypub movement](https://codeberg.org/forgejo/forgejo/issues/59) can make its way to git and allow us to move off of centralized fit providers like Githubs.
- Switch as much of my financial life over to opensource, private, and decentralized currencies as possible. [Monero](https://www.getmonero.org/) is my currency of choice.
- Break my dependence on YouTube, for personal and privacy reasons. I use privacy respecting frontends and clients, but the service still has a strong grip on me.

Stay tuned for more updates on my journey to tech independence and how you can do the same. Let me know in the comments what you did for your digital life in 2023 and plan to do in 2024!

[^1]: Proton Mail is not perfect, because [email is not perfect](https://www.privacyguides.org/en/basics/email-security/#what-is-the-web-key-directory-standard). I do believe Proton does care about privacy and has made huge strides for consumers however. For paramount security, I use PGP to encrypt messages before they even hit the browser.
[^2]: Currently, I sync my calendars with [reclaim.ai](https://reclaim.ai/), but I'm seeking alternatives that don't require a Google account.
[^3]: I'll elaborate on this later, but my preference for asynchronous communication stems from its ability to slow down life's pace. Discord, in particular, poses privacy and centralization issues and lacks external searchability, making it inefficient for structured support or documentation.
