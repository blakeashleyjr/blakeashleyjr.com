+++
title = "Elephant: My Plain-Text Life OS"
date = "2023-05-15T17:28:00-07:00"
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
license = true
content-license = "CC BY-NC-SA 4.0"
content-license-link = "https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode"
code-license = "Apache License 2.0"
code-license-link = "https://www.apache.org/licenses/LICENSE-2.0.html"
+++

In the excellent book, *The Righteous Mind*, author Jonathan Haidt details a metaphor for the relationship between our concious and unconcious minds: the elephant and the rider. The foolish rider thinks he is in control of the towering beast because it generally follows his commands, slowly lumbering from side to side at the pull of the reins. Little does the arrogant rider know, the elephant could throw the rider to his death or great injury at any moment. If the rider pushs too hard, demands too much, he may lose what he thought was the unconditional obedience of the elephant. Instead, a wise rider must form a mutually beneficial relationship with the elephant, just as our concious mind must be gentle and loving with our subconcious mind (if we want to get anything valuable out of it.)

When I was younger, I thought of my subconcious as a simple computer. A computer obeys me when I tell it to do something, immediately dedicating everything it has to my command. My subconcious was not so compliant.

And so, I would begin years of productivity cycles. At first, my rider would excite the elephant, driving him faster and faster. The results were good. My elephant would soon tire and the fun would be over. In response to this, I thought the solution would be more and more organization. It was my system that failed me. My schedule was not planned tightly enough. My will was not sufficent.

My subconcious, however, is not a computer. It is an elephant. And so, the use of the phrase "operating system" is both geniune in the sense that it seeks to dictate the lower-level functions of my brain, but it also is an ironic homage to the foolishness of my younger self, a reminder that I am in fact human.

An [operating system](https://en.wikipedia.org/wiki/Operating_system) is low-level software that manages hardware and software resources while scheduling tasks for efficent use of those resources. A rider looks far down the road, guiding the elephant on a path that will lead him to long-term flourishing, but the rider carefully listens to the desires of his trusty mount, tending to his needs with care and swiftness.

This philsophical shift in the way I view producivity brought practical changes to my day to day life. Instead of constantly looking for new tools and hacks to "optimize" my day, the focus shifted down to my elephant. My will has always known what I wanted to accomplish, but I didn't know how to work with my elephant. Efficenceny was not my problem, neither was motivation.

My productivity system has since become an after-thought, part of the background. It is like the desk my tools sit on than the tools themselves.

I now focus primarily on *how* I complete tasks, rather than what I complete. My elephant is now my friend, not an object I can squeeze value from.

This led me to develop a basic producitvity and knowledge system that is entirely plain-text. It is collection of markdown files that I syncronize with Syncthing and Git. I edit them in VSCode or using a text editor on my phone.

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
/templates
    daily-review.md
    weekly-review.md
    monthly-review.md
    quarterly-review.md
    yearly-review.md
    state-of-the-union.md[^1]
inbox.md
```

Every morning, I create the day's markdown file by copying the daily-review template into the day's folder, while creating any required folders above it. 

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


This template is organized from most important (and usually first in the day) to least important. This is crucial, because I usually don't complete the whole thing, certainly not every day. That's okay. I go as far as the elephant wants to go, perhaps with a reasonable amount of prodding.

First thing in the morning, I do a few things to center my day on the things that matter. I try to frame the day during my prayer and meditation. I ask God to help me work. My body also needs some attention to give me what I need during the day, so I stretch and have a protein shake.

Before I begin working, I review two important concepts: rules and goals. Rules are the guiding principles of my life and work that I want to remind myself of. These are easily forgotten truths that need reminding and will (hopefully) inform my thought, word, and deed throughout the day. These are what keep the elephant walking.

Goals are things that I want to do, usually by a certain date. The examples are abbreviated for privacy reasons, but I try not to overdo it in general. These are where the elephant is going.

## Tasks

So now that I have convinced my elephant to walk, what route should we take to our destination? I said earlier that I no longer focus primarily on what I do, instead focusing on how I do it. That is true, but I still need a simple list to get me through the day.

I looked a few of the leading plain-text todo systems and saw pros and cons in each. In the end, I developed my own, heavily inspired by [xit](https://github.com/jotaen/xit). 

Here is my daily list:

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

My todolist is specifically designed not to spook the elephant. Most tasks do not have a due date. I avoid them unless they are necessary. The potential stress of them outweighs their benefit, especially for me.

You will not even find a "today" section. Before, I would always end up with 20+ tasks due "today," no matter what I tried. Instead, I focus on *now.* Now might change throughout the day, depending on how much I accomplish, or it may stay the same for a few days over a weekend or as I work on a big project. So I only have "now" and "next" for tasks that have to be done soon. Otherwise, they go into the "dated" or "undated" sections.

I find this combination of plain-text, simpleness, and pressure avoidance really works wonders on my day. Most days, I am able to make progress on what I need to do. Ocassionally, I won't get much done, and that's okay. It'll still be there when I get back, only without any warnings or red text telling me how much of a failure I have been.

## Why Plain-Text?

[^1] My wife and I do a twice-weekly "state of the union" in which we do the following:

    - budget
    - discuss upcoming events, make sure the other is available, etc.
    - discuss the state of our marriage, what could be improved, things we could do for each other, etc.

This practice has done wonders for us and I highly recommend it.