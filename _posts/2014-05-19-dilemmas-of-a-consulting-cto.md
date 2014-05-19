---
layout: post
title: Dilemmas of a consulting CTO
---

Companies will often come to a consulting CTO because they find themselves (or are worried about ending up) in a tricky situation with their technology. Often these are small companies with very limited financial resources that are having difficulties aligning their product and their technical team with their business. Maybe there are bugs that urgently need fixing and the code is in a bit of a state and they don't know how to fix it all.

There is a huge amount that someone like me can do to help these organisations but with limited budgets, realistically I have to do what I can to move them forwards. Sometimes this means moving them towards increased revenue and sometimes it means helping them secure additional funding.

So what are the right things to do? The temptation is to get the product into shape. Start to document things that are hidden in the code and the developers' heads. Start to make sense of the architecture and identify problem areas. Make sure all dependencies are fully understood and that new development environments can be set up quickly without expert knowledge. Get to grips with the devops, ensuring that deployments are trustworthy and repeatable. Look into test coverage introducing integration tests if there are none, to give confidence that the most important aspects of the site don't break when changes are made.

All this takes time, and equally importantly, money that the company often does not have. And fixing those things, while setting the company up for a more stable and successful future isn't usually moving them directly towards more revenue or more funding.

To spend a very limited budget on fixing all those important things could be catastrophic for the business's success. If they're losing customers due to a frustrating bug in a key operation or failing to sign up new customers because the payment mechanism is't working, the company might go out of business before you deploy a fix.

The flip side would be to focus on the immediate issues, try and fix the bugs without getting deeper into the codebase, stop losing users and start allowing new ones to sign up. While this may well be the best immediate use of the budget, it would probably involve making the codebase worse and not moving the product on. It is also likely to be the same approach that the existing or previous team have been following for some time – fighting fires and never getting to grips with the problems in the codebase.

This "quick fix" approach also overlooks the likely fact that the condition of the codebase, the technical debt and the lack of tests are contributing to the unstable product and blindly fixing one bug may well lead to several others.

Over the coming weeks I will post in more detail my thoughts on how best to approach this situation.

[This article will be update with links when new articles are posted].