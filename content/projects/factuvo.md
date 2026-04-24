+++
title = 'Factuvo'
date = 2026-04-23T10:30:00+02:00
draft = false
+++

## [Factuvo](https://factuvo.fr) -- Link may expire after 2027

I have a family member in France who is an English teacher. In 2026, new regulations were being put into place in France that were complicating the invoicing and reporting process. Having made good progress over the last year or two of development and finally starting to feel confident in my abilities, I decided this was a good opportunity for a startup. That way, I could both help my family members and create an app targeted specifically at independent French teachers that could maybe turn a profit.

Up to this point, I had used LLMs for learning. And done a few tests for development, but had never really used them on any large scale. To me, this sounded like a good project to start with. Due to the need for testing and observability, as well as the large amount of pre-planning. I considered that by the time I actually started writing the code, most of the core decisions would already have been made.

My first priority was selecting a stack to use, and for that, Go, React, and PostgreSQL were the obvious choice, being the tools I was most familiar with. And then Prometheus for metrics, Loki for logs and Tempo for traces. All linked to a Grafana dashboard. I needed to be sure that once in production, if anything ever failed, it was thoroughly documented.

And on the regulatory side, I knew I did not have to budget to navigate the French bureaucratic system, so I decided to offload a lot of it to an existing PA/PDP(platform for e-invoicing) to handle the regulatory parts. Allowing me to focus on the core objective of catering to my specific client. This is actually where one of the first problems happened due to my incomplete research. Being very focused on upcoming regulations, I forgot to do my due diligence for all the rules currently in place, and we will get back to this later.

From that point on, I was doing a lot of database schemas, code review and UI iterations. Surprisingly, everything went really smoothly, far better than any project I had made before. The company got registered (more expensive and painful than it should really be). The project beta got completed and launched, but it was all limited to teachers below the TVA (value added tax) threshold. Everything was going great.

That is until I reached the TVA for the invoices. I really wanted to make sure I was doing it properly so I decided to do some more research. And I found a law that was passed to reduce fraud. It required cryptographic proof of continuity. That was no issue. If anything, it sounded like a fun technical challenge. However, I would also require the NF525 certification, and that was a hurdle that I unfortunately could not surpass. To get the certification, my software would have to undergo expensive and repeated audits, and I did not have the budget for that.

Despite the regulatory hurdles, the project wasn’t dead. Since teachers earning less than 37 €500 do not require TVA, the project still had a change. And if I could get enough users, then maybe the NF525 would be possible in the future.

This is when I hit the second, and even bigger, issue: Marketing. I quickly realised that my personal philosophy was at odds with traditional growth tactics. I find cold emails and unsolicited calls intrusive, so I couldn’t bring myself to subject others to them. Unfortunately, I soon learnt that ‘doing what I would consider acceptable’ was not compatible with the aggressive push needed to launch a new platform solo.

Although it is functional, and many of the features needed for the upcoming regulatory roll-outs are in place and ready to release. I see no way to commercial success for the platform.

The project now sits in a kind of limbo and likely to be shut down once the domain and hosting expire. And possibly worse of all, the family member for whom the project was initially designed actually likes it, but the constant maintenance and upkeep will be too much for it to be possible to keep running. So unfortunately, they will need to find other solutions that will likely be less tailored to their use case.
