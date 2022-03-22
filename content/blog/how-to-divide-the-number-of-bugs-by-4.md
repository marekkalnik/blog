---
title: "How to divide the number of bugs at your company by 4"
date: 2021-11-10
description: "Sharing BAM defect analysis template that I was talking about on Tech.Rocks Meetup"
---

In September we have organized a [Tech.Rocks](http://www.tech.rocks/) [meetup](https://www.youtube.com/watch?v=C9IhY_h1h_Y) around quality. We met with [Celine Gilet](https://twitter.com/celinegilet) and [Dimitri Baeli](https://twitter.com/dbaeli) to discuss different metrics and reactions to quality problems.
During this meetup I have shared a method that helped me to divide the number of client-impacting defects at BAM by 4.
I wanted to share the template with you so it may help you gain some insights.

## Putting quality first

First, I realized that quality was a strategic subject, meaning I had to have a global quality indicator in my company, shared with the rest of the leadership team.
This was not an easy task, because it meant putting in place a global indicator and creating a relevant information flow.
As with every such subject, there is a lot to do:

- clarify and align a team about what a defect is
- create relevant tools to make reporting easy

The first part was actually an opportunity to change our culture from tech-centric (a bug is a problem in the code) to user-centric (a bug is when a user encounters a problem).
We later event started to call them "defects" instead of "bugs" to reinforce this message.

> A defect is when a feature in the app productes an unexpected or incorrect result or behaves in a way not anticipated by the user or Product Owner

Given that the subject was given a strategic visibility, it was now my job as a CTO to understand what was causing defects at BAM and how we could prevent them.
So I started asking the teams in which we were observing bugs to analyze them. At first the answer I was getting were low-effort: "we are getting bugs because we are not testing enough".
It's true that testing prevents bugs from arriving at users, but the lack of test is never the cause of a bug. There is a line of code somewhere that is written incorrectly, let's find this one.

These discussions helped me understand that my job was training teams on how to react to bugs, how to investigate where they are coming and take corrective actions, so the team can improve its quality level.
I have spent countless hours analyzing bugs, I stopped counting at 100 bugs analyzed. What helped us a lot was applying a template with common questions that we were asking each bug to understand where they come from.

So here is the [template on Notion](https://m33.notion.site/PUBLIC-BAM-QRQC-TEMPLATE-2021-ad3ae8eba3bb49f9895c960dc1f9b2f1).

## BAM Defect Root Cause Analysis template

As to how I applied it:

- made sure that the analysis was done with the team/person that created the bug instead of the one that found them (do NOT delegate it to the Q&A)
- taught each Tech Lead to do it first (10-ish hours of analyzing together) before the Tech Lead is considered autonomous on doing it with his/her team
- periodically take a random sample for analysis and a discussion with a Tech Leader to help them go deeper in their understanding

Further down the line, I have created 2 events that helped people progress on quality:

- a Bugbuster meeting, where Tech Leaders would meet and analyze together some interesting bugs from their teams
- a Yokoten meeting, where a team would share with others a success story of a change that has been introduced to improve quality bug (in a PDCA format)

# Errors to avoid

I have also made some errors down the route, mostly because I was focused too much on the details of each bug.

Here are some things I wish I had done better from the beginning:

- Scaling: Analyzing bugs is a hard skill to master, and it requires constant exercise. To learn it you need to apply an apprenticeship-like model. Which means that scaling is requires a support system that will help new generations of Tech Leaders to acquire it. I did not think it through in time, so after the first generation of trained people we got a bit of a dip in applying the practice. We are refocusing back to it right now.
- Maintaining focus: the initial results were fabulous, so I got the feeling that we started a trend. But quality is something that requires constant focus, and as soon as I stopped seeing the teams regularly, the Yokoten and Bugbuster disappeared and the quality level plateaued. Quality needs to make part of everyday discussion between the manager and the managee, and it's the manager's job to encourage people to share their learnings publicly.

Hope this article and template serve you well. Would be great to get feedback from you!
