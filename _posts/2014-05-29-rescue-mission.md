---
layout: post
title: Rescue mission
---

Following on from my earlier post about [the dilemmas of a consulting CTO](/2014/05/19/dilemmas-of-a-consulting-cto/), I now want to look at what are the most important things to do for a company when a single day of your time represents an appreciable percentage of their available budget?

It's important to strike a balance between addressing any business critical issues and moving the company in the right direction. This balance can be hard to find if there is no way of knowing if fixing the issues will break things further.

## First steps

If at all possible, it is best to stop making changes to the codebase until you've got things into a better state. This can be a difficult thing to achieve as at any one time, a tech business is usually focussed on any number of bugs, features and enhancements. But if your technology is unreliable and causing problems, developing it further will just make things worse.

That said, sometimes a single issue is causing serious problems to the business and so exceptions can be made to fix these things under the acceptance that it will ultimately lead to more problems and more work down the line.

The business owner will probably already know these issues but they may need help determining genuinely business critical issues from plain old really important ones.

It is a good idea to go through each issue and establish the impact they are having. Is it regularly costing or losing the business money? Can you quantify how much? What would be the cost if we fix it in 1 week, 1 month, 1 year? Ultimately, can the company continue with this problem in place?

A strong, external voice can really help here to provide perspective and to not be afraid to tell uncomfortable truths. It also helps to have experienced technologists involved who can speak on behalf of the product, explaining the value to the business of a well-built, maintainable codebase.

## Fixing critical bugs

If you absolutely, categorically must fix one or two bugs before getting things in order, you're going to have to play it by ear. Whichever way you do it, it's going to be painful. Making fixes in an undocumented codebase you don't understand with no automated deployments etc, you're going to need a lot of luck. 

If the existing team can make these fixes, it's going to be a lot easier. That said, there's a lot of value an experienced, external person can make: documenting everything, reviewing changes, enforcing testing and improving the deployment. Making sure that the minimum of changes are made and watching out for any issues that arise along the way.

## Getting things in order

There are a whole host of blog posts hidden in here and I hope to write much of this up in future posts. For now though, here's an overview of the things that should be done to improve your codebase.

The first thing to consider is the existing team if there is one. How has this product grown and who has been in charge of that? A constant, internal team or a non-overlapping series of freelancers (or something in between)? It's vital to try to work with the existing team to put things right. The reasons for the current situation are bound to be a combination of business pressure, inexperience and lack of knowledge rather than incompetence or negligence.

The first step towards improving things is to understand the current situation. Start documenting everything from the technology being used, what components make up the system, how to create a new development environment, what are the main known issues both in terms of the user's experience and in terms of technical debt and known hacks that need addressing. 

Then think about deployments. How do new code changes get into production? How do they get tested? What other environments are there (e.g. staging) and how closely do they model the production environment? How many manual steps are there to deploy changes to new environments? Is there any automation in this process to give confidence and reliability to the process.

## Building for the future

Once the system has been fully documented and understood in a communicable way, new developers can get started easily and new changes can be reliably deployed to staging, tested and then pushed to production, you can start thinking about the actual product itself.

Automated test suites can be a pain to create and maintain but give a great deal of confidence when making changes. At the very least a small set of scripts that test the main end-to-end journeys through the site and can be run after each change is worth its weight in gold, ensuring you don't introduce new business critical bugs. Combined with continuous integration, you can start to get some trust into the development process.

Now you can start to think about fixing some of those important bugs. Strongly encourage developers to write tests for the new functionality. It is very good practise to write additional bugs to cover related areas of the code at the same time to gradually improve coverage. 

## Ongoing improvements

There are of course lots of other things to be done but its important to get things moving forward as quickly as possible.

These things would involve reviewing the specific technology choices to make sure they're supporting rather than hampering development; thinking about performance and scaling issues, introducing analytics and metric tracking etc.

Ultimately, all of this is about increasing the trust that the entire team has in the codebase, in the product and in the team's ability to make changes safely and move the product and the business forward. 

Hopefully this is useful to anyone finding their startup in a difficult situation. Please [get in touch on Twitter](https://twitter.com/kpopper) if you have any questions or want to challenge any of this.
