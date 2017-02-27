# Chapter 2: Starting a New Project

**In The Beginning ...**

Congratulations, now you've got buy-in from your organization! Your internal stakeholders, bosses, and team are totally cool with what you have planned. You do have a plan, right?

Don't be scared.  It is usual to be nervous about putting your code out into the world for anyone to come by and tell you how wrong you are or how tabs are better than spaces.  Open source, emotionally, is not always easy; as with many things on the internet, it allows people to semi-anonymously tell you about your flaws.  It's important to keep in mind that 1) you likely made a mistake or two, and 2) everyone makes mistakes.  Try not to take things personally and view all comments as happy little constructive criticism there to make things better.  As you do more open source, both starting and contributing, you will feel more confident and less concerned with the inevitable mistakes.


> One of my first open source projects was the OpenLayers Drupal module which, unsurprisingly, integrated the OpenLayers javascript library into Drupal, a CMS.  Oddly enough, almost the same exact day that I released a first rough version of the module, another person released a very similar module.  This was a little heartbreaking, but that person and I talked, and we decided we had similar goals and began to collaborate on one single module; this was a very positive experience.  As the module grew and other contributors came onboard, there was a difference in direction of architecture.  Given my emotional attachment to the project, I had a tough time dealing with these changes; that combined with the difficulty in communicating online (in fact most of it is still up in the Drupal issue queue), the experience of collaborating became negative for me, and I eventually did not have the time or emotional energy to commit to the project.  But, it still lives on today with completely different set of contributors.

>The lesson I learned early on when doing open source work is don't take things too seriously.

> *- Alan Palazzolo*


This chapter will talk you through starting a new open source project, discussing first steps and introducing big to-dos and potential pitfalls/challenges.

## The Naming of Things

![hello, my name is...](https://media.opennews.org/fieldguides/open-sourcing/hello-sticker.jpg)

Everyone knows there are only two hard problems in computer science: off-by-one-errors and naming things. There are an [infinite](https://pages.18f.gov/open-source-guide/naming-your-project/) [number](http://ivantomic.com/projects/ospnc/) [of articles](http://jerodsanto.net/2014/08/naming-things-is-hard-lets-go-shopping/) [on picking](http://deviq.com/naming-things/) [a good name](http://www.avangate.com/avangate-resources/article/product-naming.htm). Identify your goal when naming your project. Are you trying to make a project that's easy to find? Make the name simple, clear and declarative. Are you trying to be creative? The world is your oyster! Generally, though, good names will be distinctive, descriptive and memorable.

Naming a project can be very important if it becomes a big success, but it's also something you can change down the line (sometimes with headache).  So, take some time to think of a name you can live with, but don't over think it.

## Choosing a License

When it comes to choosing a license, here are a few tips to make this important, legally-binding decision less scary.

* Consider your organization's internal needs. Are you planning to sell this software to other organizations? Do you have strict rules about intellectual property that would prevent you from allowing others to modify and build on your work? You might need to check with your legal team on this, but if it's not already clear, you'll want to walk into their office with a plan.

* Talk to your organization's legal counsel. Your individual license decision might not matter if your counsel recommends a different license for reasons you aren't privy to.

>The NYT's counsel recommended we use the Apache 2.0 license instead of the MIT license not because of something intrinsic to how the licenses worked but because our counsel was more familiar with Apache 2.0.

>*— Jeremy Bowers*

* Take a look around at how similar organizations are licensing their open source releases, or consider the license most commonly used by the software community you expect to contribute to your project. Building a WordPress plugin? Browse through the plugin directory and follow the path that makes sense for you.

* Review a list of common licenses and what protections they have to offer. Check out resources like [choosealicense.com](http://producingoss.com/en/license-quickstart.html), from GitHub, or research popular licenses such as the [MIT License](https://opensource.org/licenses/MIT) and the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) to find the one that fits your needs.

* Think about who is going to use your code.  Though the potential may be anyone, what license you choose can affect how certain groups or organization can use your code.

There are many licenses to choose from, and you should pick the one that is best for you. To help narrow it down, there are essentially two types of licenses.

1. **Copyleft**.  Copyleft license say that anyone who uses the code can reuse it, but the license goes along with the code, usually meaning that [derivative work](https://en.wikipedia.org/wiki/Derivative_work) can only be distributed under the same license.  The main plus of this license is that it continues "open source".  The main negative of these types of licensing is that it can sometimes conflict with internal policies and make it hard to for certain organizations to use (usually commercial).

    1. [https://en.wikipedia.org/wiki/Copyleft](https://en.wikipedia.org/wiki/Copyleft)

    2. The most common of these the is the GPL license, the newest of which is the GPLv3.

2. **Permissive**.  A permissive license is basically a license that says the user can do whatever they want with the code, sometimes requiring attribution.  The main pro of a permissive license is that anyone can you the code regardless of specific restrictions they may have.  The main negative is that not requiring that the use of it remain open source goes against the ideals of open source.

    3. [https://en.wikipedia.org/wiki/Permissive_software_licence](https://en.wikipedia.org/wiki/Permissive_software_licence)

    4. The most common permissive license is MIT.

> **Use the MIT license.** The MIT license is the most popular license used on open source projects.  It is very simple and allows users of the code to do what they want.  If you don't have specific needs in your organization that lead you toward a different license, consider using the MIT license.  In fact, it's so short, we can include it here:

> Copyright (c) <year> <copyright holders>

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Licensing non-code projects 

The licenses talked about so far have been focused on how code can be used, but if you are working with something other than primarily code, there are more appropriate licenses. [TODO: more on why one would use a license for non-code projects]

The most common is [Creative Commons](https://creativecommons.org/share-your-work/), which is a suite of licenses made to be easy to understand and mixed depending on your needs. Creative Commons is mostly used for media or content, such as text, images, or videos.

The [Open Data Commons](http://opendatacommons.org/) is similar to Creative Commons but is focused on data.  OpenStreetMap, a very successful open data project, uses the ODbl license.

### Copyright

It's important to note that licensing a open source project does not mean that you are giving away your copyright to that material, personally or as an organization (depending on how copyright works at your organization).  A license is basically answering the question of "Can I use this? And how?" for everyone.

On the flip side, any contributions by other people or organizations are still copyright to those contributors.  If your project becomes large enough, it may be worth looking into a [Contributor License Agreement](https://en.wikipedia.org/wiki/Contributor_License_Agreement), so that both the project and the contributor have more defined rights/roles.

## Know Your Audience

As with all product releases, news apps, or stories, you should probably have an audience—in this case, we're talking about users—in mind. Who are the users out there in the world clamoring for a thing that does what your thing does? You should keep them in mind throughout this process, not just to build the thing that serves their needs, but to build it in a way that makes it usable!

For example, if you're building a tool that small nonprofit newsrooms might want to integrate into their content management systems, consider the systems many of them use now and the resources they have on hand to vet and install new code.

## Evaluate the Competition

![oh, Wash](https://media.opennews.org/fieldguides/open-sourcing/wash.gif)

The Internet is full of things. So many things. You want your thing to be one of them. Are you sure there's not already a thing that does that thing?

There might be. Consider whether this is a moment to stand on the shoulders of giants, building on an existing open source project, making it your own, and releasing it back into the wild for others to do the same, or if this is a moment to break from the past and build a much, much, better mousetrap. To mix metaphors, this is the moment when you're going to decide whether to reinvent the wheel, and sometimes, you have to do so if you want to get to the flying cars.

Spend some time searching for similar projects in the wider news nerd community, and beyond on GitHub and elsewhere. If you find an amazing repository you might want to build on, take a closer look at open issues, the recency of pull requests and commits, and get a feel for whether it's actively being maintained. Then, get in touch with the owners and find out what they learned along the way.

## More on Getting Started

* "Producing Open Source Software," by Karl Fogel. [Chapter 2: Getting Started](http://producingoss.com/en/getting-started.html) 

## What's Next

We're so excited for you right now. You've started your first open source project!

![ahhhhhhhhhhhh](https://media.opennews.org/fieldguides/open-sourcing/kermit.gif)

But wait, there's more. Skip to [Chapter 4](Chapter04-Code-First-Release.md) to learn more about your first release, writing detailed and useful documentation, growing your community, and the inevitable end of your project. Or, if your task is to open source an existing project, make your way to [Chapter 3](Chapter03-Existing-Projects.md).

## Checklist

- [ ] Name your project
- [ ] Choose a license
- [ ] Identify your audience
- [ ] Evaluate the competition
- [ ] Consider recruiting partners
- [ ] Create or fork a repository
- [ ] Start writing your README documentation
- [ ] Add your license and initial contributors documentation
- [ ] Commit some code!
- [ ] Commit some more.
- [ ] Update that README documentation
- [ ] Build your first release
- [ ] Have a plan for maintenance and support
- [ ] Have a contingency plan for sunsetting + other bad things that might happen
