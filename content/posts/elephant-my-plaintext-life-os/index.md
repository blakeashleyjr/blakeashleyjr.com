+++
title = "Elephant: My Plain-Text Life OS"
date = "2023-05-21T17:28:00-07:00"
author = "Blake Ashley Jr."
authorTwitter = "" #do not include @
cover = ""
tags = ["Productivity", "Plain-text", "Elephant"]
keywords = ["Productivity", "Plain-text", "Elephant"]
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
In his excellent book, *The Righteous Mind*, Jonathan Haidt details a metaphor for the relationship between our conscious and unconscious minds: the elephant and the rider. The rider thinks he controls the towering beast because it generally follows his commands, slowly lumbering from side to side at the pull of the reins. Little does the rider know, the elephant could throw the rider to his death or great injury at any moment. If the rider pushes too hard or demands too much, he may lose what he thought was the unconditional obedience of the elephant. Instead, a wise rider must form a mutually beneficial relationship, a friendship, with the elephant, just as our conscious mind must be gentle and loving with our subconscious mind (if we want to get anything valuable out of it.)

When I was younger, I thought of my subconscious as a simple computer. A computer obeys me when I tell it to do something, immediately dedicating everything it has to my command. My subconscious was not so compliant.

And so, I began years of productivity cycles. At first, my rider would excite the elephant, driving him faster and faster. The results were good. My elephant would soon tire, however, and the fun would be over. Eventually, my elephant knew I was a liar. No matter what I promised, he knew I was going to drive him until he gave out. So he stopped obeying, and I don't blame him. 

This created a vicious and painful cycle. The only way I could get things done was if the threat of failure was so great I could rouse my distrustful elephant to action. If there was no meaningful deadline, I did not do *anything.*[^2]

In response to this, I thought the solution would be more and more organization. It was my system that failed me, I would tell myself. My schedule was not planned tightly enough. My will was not sufficient.

Organization, of course, was not the problem. It was a distraction. 

While my elephant lay exhausted or otherwise unwilling to move, my rider spent his days planning the journey. Instead, he should have been tending his elephant.[^3] My subconscious is not a computer. It is an elephant. There is no such thing as an internal command, only requests. Each thing I do is a negotiation with the lumbering beast I depend on.

A rider looks far down the road, guiding the elephant on a path that will lead him to long-term flourishing, but the rider carefully listens to the desires of his trusty mount, tending to his needs with care and swiftness.

And so, the use of the phrase “operating system” is both genuine in the sense that it seeks to dictate the lower-level functions of my brain, but it also is an ironic homage to the foolishness of my younger self, a reminder that I am in-fact human. It also sounds cool.

This philosophical shift in the way I view productivity brought practical changes to my day-to-day life. Instead of constantly looking for new tools and hacks to “optimize” my day or developing increasingly complex productivity systems, my focus shifted down to my elephant. 

My productivity system has since become an after-thought, part of the background as much as possible. It is more like the desk my tools sit on than the tools themselves.

I now focus primarily on *how* I complete tasks, rather than what I complete. My elephant is now my friend, not an object I can squeeze value from.

This led me to develop a basic productivity and knowledge system that is entirely plain-text. I explain why this is important later on. It is a collection of markdown files that I synchronize with Syncthing and Git. I edit them in VSCode or using a text editor on my phone.

As a result, my productivity and my happiness have skyrocketed.

{{< newsletter-form >}}

I organize my system in the root of a directory like this:

```Markdown
/[year]
    /[month]
        /[week]
            /[day]
                daily-review.md
                notes.md
                one-off-task-or-small-projecct.md
/projects
    /[sample project]
        /note.md
        /web-clipping.md
/templates
    daily-review.md
    weekly-review.md
    monthly-review.md
    quarterly-review.md
    yearly-review.md
    state-of-the-union.md
inbox.md
```
     
## Planning / Review

Every morning, I create the day's markdown file by copying the daily-review template into the day's folder, while creating any required folders above it. Note the *state-of-the-union.md*[^1].

Here is a sample of that template:


```Markdown
# Daily Planning / Review

## Good morning!

Lay not up for yourselves treasures upon earth, where moth and rust doth corrupt, and where thieves break through and steal: But lay up for yourselves treasures in heaven, where neither moth nor rust doth corrupt, and where thieves do not break through nor steal: For where your treasure is, there will your heart be also.

---

## Daily Planning

### Wake up routine

[ ]  Stretch
[ ]  Meditation and Prayer for 10 minutes
[ ]  Read the Bible for 15 minutes
[ ]  Have a protein shake
[ ]  Take my vitamins

### Planning Routine

[ ]  Make office spotless
[ ]  Review my calendar for the day
[ ]  Make sure there are no conflicts
[ ]  If there are conflicts, develop a resolution plan immediately
[ ]  Review Todolist

---

## Rules for 2023

- God is good.

- Money is a tool to provide for my family, help people in my community, and further God's will on earth, nothing more.

- Work is good.
  - Work makes my life and the life of my family better.
  - Work feels good.
  - Consistently work 8 hour days.

## Goals for 2023

- Write one blog post per week
- Get down to 175lbs by Christmas
- Etc.

---

## Mid-day Journal and Brainstorming

*What’s on your mind?*

---

## 1. Be sure to do the following

[ ]  Clear task list
[ ]  Clear inbox
[ ]  Review the calendar for today
[ ]  Review your events tomorrow
[ ]  Copy all physical notes into Elephant
[ ]  Save copy of all documents into Elephant

## 3. Answer the following questions

- How did you feel today?
- How was your relationship with Christ?
- Were you kind to [my wife]?
- Did you do anything for any other relationship?
- How productive were you in general?
- How organized were you?

## 4. Overview, how was your day? Any lasting thoughts for future you?

## 5. Lastly, any tasks, plans, ideas, tools, etc. come to mind?

## ***Have a great night! You earned it!***
```

This template is organized from most important (and usually first in the day) to least important. This is crucial, because I typically don't complete the whole thing, certainly not every day. That's okay. I go as far as the elephant wants to go, perhaps with a reasonable amount of prodding.

First thing in the morning, I do a few things to center myself on the things that matter. I try to frame the day during my prayer and meditation. I ask God to help me work. My body also needs some attention to give me what I need during the day, so I stretch and have a protein shake.

Before I begin working, I review two important concepts: rules and goals. Rules are the guiding principles of my life and work that I want to remind myself of. These are easily forgotten truths that require reminding and will (hopefully) inform my thought, word, and deed throughout the day. These are what keep the elephant walking.

Goals are things that I want to do, usually by a certain date. The examples are abbreviated for privacy reasons, but I try not to overdo it in general. These are where the elephant is going.

As they day progresses, I begin to reflect on what has happened. I take notes. I review the things I have done. The questions and tasks provide a guideline to facilitate that if I feel like it.

I do something similar at the end of every week, month, quarter, and year. My elephant needs to regularly hear that I care about him, and, in return, he trusts me when I tell him what is important.

If I miss one, I don't stress. It's okay. Keep moving and do it tomorrow.

## Notes

It is easy to over-think notes. They have traditionally been a black hole of my time and energy trying to build a better system *ad infinitum*. So, I decided to keep it as simple as possible.

My notes are written in Markdown and have a single h1 at the top. That's it. I can add more if the thought requires it, but frequently don't.

I divide notes into two categories, those that are tied to a project and those that are not. 

Notes that are tied to a project go into a folder named after that project in /projects. 

Notes that are not tied to a project go into that day's folder.

That's it. It has been freeing not to rely on some advanced system I will eventually drop because it's too much work.

*What about search, tags, categories, mind maps, knowledge maps, embeds, etc.??*

You don't need them. I rely on the search in VSCode and have never had a problem finding something I wanted to remember. I intentionally think about relevant words my future self may use to search and include those in the note.

## Tasks

So now that I have convinced my elephant to walk, what route should we take to our destination? I said earlier that I no longer focus primarily on what I do, instead focusing on how I do it. That is true, but I still require a simple list to get me through the day.

I looked at a few of the leading plain-text to-do systems and saw pros and cons in each. In the end, I developed my own, heavily inspired by [xit](https://github.com/jotaen/xit). 

Each day has a tasks.md. At the end of the day, I copy that tasks.md into the next day's folder, while marking tasks complete or obsolete. In the morning, I check the priorities still make sense and get going.


```Markdown
# Current Tasks

## Now

[ ] Finish blog post on Elephant

[ ] ! Complete work project and email boss about it

[ ] Book Play Tickets -> 5-10-2023

## Next

[ ] Buy gift for brother

[@] Get the flight sim setup #personal

### Dated

[ ] ! File taxes before deadline #chores -> 03-18-2023

### Undated

[ ] ! Audit all accounts in Bitwarden
    - [ ] Delete unnecessary accounts
    - [ ] Change email and personal info in necessary ones

[ ] !! Reach out to accountant for status

## Reocurring

[ ] Do laundry -> every tues

[ ] Check the air filter #chores -> 1st of every 3rd month (last done on 02/01/23)

[ ] Submit my expense report -> 1st workday of each month

### Waiting

[@] Reach back out to contractor

## Someday/Maybe

[ ] !! Learn German

## Done

[X] ! Freeze credit


## Guide

[ ] This is an open item
[ ] ! This is an important task
[ ] !! This is a less important but still important task
[x] This is a checked item
[@] This is an ongoing item
[~] This is an obsolete item
[?] This is an item in question
[ ] This shall be done by -> 2023-08-31
```

My to-do list is carefully designed not to spook the elephant. Most tasks do not have a due date. I avoid them unless they are necessary. The potential stress of them usually outweighs their benefit, especially for me. Most tasks do not need to be done before a specific date if you get to them in a timely manner.

You will not find a “today” section. Before, I would always end up with 20+ tasks due “today,” no matter what I tried. Instead, I focus on *now.* Now might change throughout the day, depending on how much I accomplish, or it may stay the same for a few days over a weekend or as I work on a big project. So I only have “now” and “next” for tasks that have to be done soon. Otherwise, they go into the “dated” or “undated” sections. I use those to backflll things as I complete them.

I find this combination of plain-text, simpleness, and pressure avoidance really works wonders for my productivity. Most days, I am able to make progress on what I need to do, which is a miracle knowing where I came from. Occasionally, I won't get much done, and that's okay. It'll still be there when I get back, only without any warnings or red text telling me how much of a failure I have been.

## Why Plain-Text?

Plain-text is both a practical and philosophical choice. 

It is practical:

    - It is interoperable and readable anywhere. I do not have to rely on any company or tool to access my thoughts, memories, and ideas.
 
    - It is fast and light. I can open this text file on any operable computer on the planet. I do not need to wait on things to load. A decade's worth of thoughts take up almost no space at all.

    - I do not need to be connected to the internet.

    - I have much more control over my favorite text editor (VSCode) than I would any other app.
  

It is philosophical:

    - Apps enforce a philsophy by definition. They are taking my input and organizing them in a specific and opininated way. That can be great, especially if I built the app or the app maker thinks a lot like me. I want freedom. I want to be able to customize my templates and system at will, without enforcing that change on the past.

    - Apps usually control my data. Without special precautions, I could lose my work in the event a company goes out of business, changes their policies, decides they don't like me, misunderstands me.

    - Plain-text is easily private. I control where these files go. I can encrypt them without much trouble. I don't have to give a company access to the most private records of my life.

    - Plain-text is simple. I have a problem with over-complicating systems. There is only so much you can complicate with plain-text.

    - I want to focus on words. Words represent ideas, thoughts, dreams, memories, or plans. I want as little as possible between my brain and words.

*I plan diving into this more in other posts.*

## What about perseverance and self-discipline?

This is a long game. Just like trust with another person takes time. It takes time for your elephant to trust you.

Perseverance is important, when necessary. When I was disordered, everything I did required perseverance, because it was such an event to complete the task. As my elephant began to trust me, he understood that when I asked him to push through, it was actually required.

Self-discipline is important, but it requires a foundation. I need to be healthy before I could “push through” the desire to quit or my lack of energy. I had to build my subconscious (as it relates to work) up from the ground before there was anything to push with. As I become more and more ordered, I naturally develop the ability to work longer and harder. My elephant gets stronger and healthier over time, as I treat him right.

## Conclusion

My elephant is my friend and my companion. If I want to get to my destination (flourishing, success, peace), I must persuade the elephant to get up and start walking. If I abuse my elephant, he will not trust me. He will not obey me. So I will resort to increasingly abusive methods to compel his obedience. Eventually he will be broken and so will I.

As I learn to treat my elephant better, I developed a simple, plain-text “operating system” to govern my behavior throughout the day. It helps me lead my elephant to places that matter.

**How do you treat your elephant? Do you have any advice on how to be kinder to yourself? Please let me know via email or in the comments below.**

[^3]: The tragedy is that, instead of being able to congratulate myself for things I did and accomplished, I was only able to recover from the hell required to complete the task. There was no satisfaction in what I had done, only dread of what was to come.

[^2]: This cycle did two things to me. One, it made my excellent under pressure. I can perform Herculean tasks with extreme focus in order to meet a shortly approaching deadline, as I have trained myself and my elephant to perform this way since elementary school. 

    Two, knowing that I could likely accomplish the task satisfactorily shortly before the deadline, combined with my painful inability to complete tasks when not under pressure, made it impossible to do anything that wasn't forced.

    Because of my ability to complete things last-minute, I have always been able to accomplish things that make it seem like I have my life together.

[^1]: My wife and I do a twice-weekly "state of the union.” This practice has done wonders for us and I highly recommend it. We do the following:

    - budget
    - discuss upcoming events, make sure the other is available, etc.
    - discuss the state of our marriage, what could be improved, things we could do for each other, etc.

  


