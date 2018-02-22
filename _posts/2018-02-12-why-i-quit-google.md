---
title: Why I Quit Google to Work For Myself
layout: single
author_profile: true
read_time: true
comments: true
share: true
related: true
sidebar:
  nav: main
---

I started working at Google in early 2014. For the first two years, I loved the job. Then I applied for a promotion.

My last day was February 1. I worked at Google for just under four years.

# The first two years

Two years in, I still loved working at Google.

The annual employee survey asked me how much I agreed with the statement, "I expect to be at Google in five years." I enthusiastically clicked, "Strongly Agree." 

Of *course* I'd still be at Google in five years. I was surrounded by the best engineers in the world, using the most advanced development tools in the world, and eating the free-est food in the world.

My most recent performance review rated me as "Exceeds Expectations." If I just kept going, I'd soon be promoted to the next level, Senior Software Engineer. What a great title! Forever after in my career, I'd be able to say, "Yes, I was a *Senior* Software Engineer. At *Google*." People would be so impressed.

My manager assured me that my promotion was close. He felt that I was already capable of senior-level work. I just needed the right project to prove it to the promotion committee.

# Your manager doesn't promote you?

No, managers at Google can't promote their direct reports. They don't even get a vote.

Instead, promotion decisions come from small committees of upper-level software engineers and managers, none of whom have ever heard of you until the day they decide on your promotion.

You apply for promotion by assembling a "promo packet": a collection of mini-essays you write about why you deserve a promotion, your design documents, and written recommendations from your teammates. (TODO: rewrite)

The promotion committee reads your packet looking for evidence that:

* You can manage complexity
* Your work has had a positive impact on Google
* You have strong leadership skills

During my two year honeymoon phase, this system sounded great to me. Of *course* my fate should be in the hands of an anonymous committee who's never met me. They wouldn't be tainted by any sort of favoritism or politics. They'd see past all that and recognize me for my good engineering decisions.

# That's not really how it works

Before I wrote a promo packet, I never thought about I'd communicate my work to the promotion committee. In my head, the promotion committee was this omniscient and fair entity. If I spent each day making the right engineering decisions, making the codebase better, helping my team execute more efficiently, the promotion committee would magically know this and reward me for it.

Unsurprisingly, it doesn't work like that, but it took me two years to figure that out.

My main responsibility until that point was maintaining a legacy data processing pipeline. It had been in maintenance mode for years, but load had increased and the pipeline was buckling under the presssure. It frequently died silently, produced incorrect output, and its failures could take days to diagnose because nobody had kept documentation for it after the initial design document.

I proudly nursed the pipeline back to health. I found dozens of bugs, fixed many of them, and wrote automated tests to make sure the bugs wouldn't reappear. I deleted thousands of lines of code that were either dead or could be replaced by modern libraries. I documented as I went so that the information wouldn't be siloed in my head. None of it was quantifiable or provable.

The pipeline had very few recorded metrics, and the available metrics made it look like I had made things worse. All my bug discoveries caused the overall bug count to increase. Pipeline failures had gone up, partly due to increased load, partly because I had changed the code to fail loudly instead of quietly producing incorrect data. I drastically reduced the amount of developer time required to keep the pipeline running, but there were no metrics that tracked how developers were spending their time.

Other work I had done didn't look so good on paper either. There were several times in my first two years where I put my projects on hold for weeks to months so I could help a teammate whose launch was at risk. It was the right decision for the team, but it looked very unimpressive in a promo packet. To the promotion committee, my teammate's work is big and important. They demonstrated good leadership skills by accepting my work. I'm just the mindless peon whose work is so irrelevant that it can be dropped at a moment's notice.

The promotion committee's response was what I'd feared: they said that I hadn't proved I could handle technical complexity, and they couldn't see the impact I'd had on Google.

# New strategy

The rejection was a tough hit, but I wasn't discouraged. Everyone reassured me that I was doing Senior-level work, but I wasn't conveying it properly to the promotion committee.

Okay, that was solvable.

I decided I was too naive my first couple years. I didn't factor the promotion committee's perspective in how I chose my work. After going through the process once, I could keep doing the same kind of work. I just had to plan better so that I'd have a paper trail I could show at promotion time.

For example, my team was getting tons of alert emails due to false alarms. I could spend some time on that problem because we tracked the number of alerts over time. I'd be able to show the promotion committee a chart of the alerts going down after I started working on the problem.

A few months later, I was assigned a project that seemed destined for promotion. It was a machine-learning project, which is the sexy thing at Google right now. It also required me to lead a junior developer throughout the project, which would show the promotion committee I was capable of leading.

The next performance review would be in four months, so I wouldn't have time to launch anything by then. But surely by the following cycle in 10 months, I'd have an undeniable case for promotion.

# The holiday gift wake up call

A few months later, Google [made headlines](http://fortune.com/2016/12/09/alphabet-donated-its-employees-holiday-gifts-to-charity/) for their holiday gifts. Breaking their tradition of buying lavish gifts for employees, they spent the money on ~~advertising disguised as charity~~ Chromebooks for underprivileged schoolchildren.

Shortly after this, I witnessed the following conversation between two employees:

>**Employee A**: You effectively **are** still getting the gift. Cost cuts like this increase the value of Google's stock. You can sell your stock grants and buy any present you choose.
>
>**Employee B**: If I told my wife that I wasn't buying her a Christmas gift, but she could use the money in our shared bank account to buy whatever she wanted, that wouldn't go over well.
>
>**Employee A**: You're in a **business** relationship with Google. If you're disappointed that Google isn't "romancing" you with gifts like the ones you buy your wife, you have a misguided notion of the relationship.

Oh yeah! I was in a business relationship with Google.

It may sound strange that it took me two and a half years to realize it, but Google goes to great lengths to build a sense of community among its employees. To make us feel that we're not just employees, but that we *are* Google.

That conversation made me realize that I'm *not* Google. I provide a service for Google in exchange for money.

So if Google and I have a business relationship that exists to serve each side's interests, why was I spending time on all these tasks that served Google's interests instead of my own?

# Optimizing for promotion

I took the wrong lesson from my first promotion rejection. I was doing the same work that didn't get me promoted, but I was trying to package it better to satisfy the promotion committee. I should have done the opposite. I should have started from what the promotion committee wanted and just done the work that would look good to them.

My quality bar dropped from, "Will we be able to maintain this for the next 5 years?" to, "Can I prevent this from blowing up until performance reviews are finalized?" I didn't file or fix any bugs unless they risked my project's launch. I wriggled out of all responsibilities for maintenance work. I stopped participating in interviewing and recruiting.

# What am I doing?

Two months later, my project was canceled. It had nothing to do with my work. Management decided to trade it away to our sister team in India. In exchange, we got one of their old, undocumented legacy systems. To a promotion committee, the time I spent on my machine learning project was meaningless because I hadn't released anything.

This had happened several times in various forms.

TODO: Insert cartoon.

The more I thought about the situation, the weirder it seemed. My career advancement was dictated by an anonymous committee who thought about me for maybe an hour or so.

Managers, directors, and VPs above me had their own incentives for picking projects and team priorities. They're optimizing for their own careers, not mine.

There had been several times in my first few years at Google where I was partway through

Even if I got the promotion, what then? Each promotion level was supposed to be exponentially harder. I'd be up against even more risks, more interruptions that were outside my control.

# The final few months

A couple months before the performance cycle ended, my entire team was called into a meeting with managers several layers above us. They had decided to disband our team.

They were generous in helping us find new teams within Google, but it was a tough hit. Anyone who wanted to get promoted had to get it in the next cycle, otherwise they'd basically be starting from zero. We were all going to spend the next several months ramping up on whatever new team we ended up on.

# One Last Shot

Performance reviews only happen every six months, so I made one final attempt at promotion. I took on a new project and did the opposite of everything my engineering instincts told me. My quality bar dropped from, "Will we be able to maintain this for the next 5 years?" to, "Can I prevent this from blowing up until performance reviews are finalized?" I didn't fix any bugs unless they risked my project's launch. I wriggled out of all responsibilities for maintenance work.

My performance rating was "Superb," the highest possible rating, given to only ~5% of employees each cycle.  The promotion committee agreed that my past six months demonstrated that I could do work at the caliber of a Google Senior Software Engineer. But it was the *only* time in my Google career that I showed this, so they didn't think it was enough of a track record to merit a promotion. This was despite ratings of "Exceeds Expectations" or "Strongly Exceeds Expectations" for the past two years straight.

I wish I could say I didn't care because I knew I was leaving, but I would have really loved to get that title.

# Working for myself

I always liked the idea of starting my own software company at some point, but I didn't know how to do it. I didn't like the idea of pitching to venture capital firms. I really didn't like the thought of constantly being under pressure from my investors to constantly pump out new features to drive growth.

In late 2016, I discovered Indie Hackers. It's a podcast and community for people who are interested in starting small software businesses, so they just... start them. No venture capitalists or investors. Generally using savings or as a side project.

The money had always worried me.

# What's next

When I tell people I left Google, they assume I *must* have some brilliant idea or I'd be an idiot to leave such a cushy job. But I am indeed an idiot with no real plan.

My rough strategy is to try different projects for a few months each to see if any of them catch on. Here are some of my ideas:

* Continue working on KetoHub (TODO: link) to see if I can make it profitable
* I've been writing about Sia (TODO: link), a distributed storage network  for several years. Maybe I can build some business on top of that technology.
* Put more energy into blogging, and look for ways to earn money from it