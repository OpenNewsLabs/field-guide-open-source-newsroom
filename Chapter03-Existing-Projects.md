# Chapter 3: Opening An Existing Project

**It's Never Too Late For Now**

## I've Made An Error

![i am error](https://media.opennews.org/fieldguides/open-sourcing/error.jpg)

In [Chapter 2](Chapter02-Starting-New-Project.md), we talked about how to start a new open source project. You had buy-in to open source it from the beginning, and learned a lot along the way about identifying your audience, making sure there wasn't already a better solution out in the world, and the benefits of working in public.

Or not.

Perhaps you or your organization already started working on a software project and *didn't* start working in public from the very start. You're not alone. Most projects start off closed-source.

Other people can still benefit from your work even if you've started off closed-source. More importantly, you can still accrue the advantages of open-sourcing your app, or part of your codebase as a library. All it takes is a little preparation and convincing your organization that it's okay to make this transition.

## What To Expect

In this chapter, we'll walk through the decisions you need to make when open-sourcing your existing project. We'll talk about the different benefits you might receive and others might get. We'll also discuss the concrete steps you need to take to sanitize or refactor your app. And finally, we'll walk through some specific objections you might hear and how you can address them.

## How Others Have Dealt With This

Karl Fogel's excellent "Producing Open Source" [has an entire section](http://producingoss.com/en/opening-closed-projects.html) just on open-sourcing closed projects. Karl's work isn't specific to newsrooms but is globally useful for any open-source software project.

# Practical Considerations Before You Start

## Do you need to open source the entire project? 

Many projects that start closed-source have parts in them that are either so specific to your company's workflow that they are not useful to others or proprietary bits that you don't want to expose to the internet. However, this shouldn't be a reason to skip open-sourcing your project. For example, you can remove the bits that are specific or proprietary and incorporate them as a separate module that only your developers can see.

## Is your project sanitary? 

![clean clean clean](https://media.opennews.org/fieldguides/open-sourcing/sanitary.png)

While it's generally good practice to [separate your configuration from your code](https://12factor.net/config), close-sourced software makes it easier for developers to break this rule. Does your app have keys or configuration in the repository that should be exported to the environment or managed in some other way?

A few resources: 

* Use a [project like Git Secrets](https://github.com/awslabs/git-secrets) from AWS to make sure you're not accidentally committing secrets to the open internet. And since your Git history could contain old instances of secrets in the repository, consider squashing your commit history before making your project public. 

* Sanitize personally identifying information—use [https://github.com/emanuelfeld/poirot](https://github.com/emanuelfeld/poirot), a tool to search a repo's revision history for text patterns (e.g. passwords, tokens, configuration data, IP addresses, phone numbers, and names)—including sample data you are shipping with the code

If you're open-sourcing data, you absolutely want to be careful of this too, especially in the case of user data. Even when data *looks* like it's been anonymized, it can frequently be deanonymized (that is, matched back to the original user). 

> * In 2000, Latanya Sweeney demonstrated that 87% of the US population could be uniquely identified with just their zip code, gender, and date of birth ([Source](http://dataprivacylab.org/projects/identifiability/paper1.pdf)). 

> * Even if the dataset doesn't include location, age, or gender information, it can still be deanonymized by factors as seemingly broad as favorites and search queries.

>    * For example, in 2006, a dataset of AOL web searches led to a user being deanonymized just through her search queries ([Source](http://www.nytimes.com/2006/08/09/technology/09aol.html)).

>    * In 2008, Narayanan and Shmatikov were able to use deanonymization techniques to re-identify 500,000 Netflix subscribers, where the dataset only included dates and movie ratings ([Source](https://www.cs.cornell.edu/~shmat/shmat_oak08netflix.pdf)).

## Is the project in a working state or is it still mid-development?

![making it fit](https://media.opennews.org/fieldguides/open-sourcing/makeitfit.gif)

You might find yourself in the position of open-sourcing a project that has been started but isn't in a working state yet. Do you have a roadmap for your upcoming work on the project? Making a development roadmap public can give potential contributors an understanding of what you're planning on building so that they can focus on other areas of the codebase. And it can help you focus your attention on just the features necessary to get the project in "working" condition. 

[TODO: link to roadmaps section]

## What form of collaboration are you interested in?

Different projects require different forms of collaboration from the community. Perhaps your project is mature and you're really only looking for bug reports. But you might also have a project that's still so new that you're looking for help refining the developer interface. Do you expect pull requests for specific pieces? You should make sure to hint about where in the project you'd like people to help out. Are you looking for feedback about the core issues the project is expected to solve? You can make this clear by building a section in the README or making a series of tickets that address this concern. [TODO: link to contributing chapter]

## Treat It Like A New Project

See [Chapter 2](Chapter02-Starting-New-Project.md) for instructions on things like naming, choosing a license, and evaluating the competition.

# Examples

[TODO: add your examples!]

# Finishing Up

Now let's talk about how to set up your codebase and code infrastructure for a better chance of success.

## Checklist

- [ ] Consider your audience and competition
- [ ] Build the case for how your organization can benefit from open sourcing this project
- [ ] Identify the parts of this project that *shouldn't* be open-sourced
- [ ] Sanitize your code to make sure you're not sharing secrets and keys with the world
- [ ] Share your development roadmap, or at least the status of the project, to inform potential users and contributors
