# Chapter 5: Documentation

![whyyyyy document](https://media.opennews.org/fieldguides/open-sourcing/why.gif)

Most of developers have run into the situation where they have to update or upgrade an existing project and quickly discover the cost of figuring out how that code works. Documentation is key to reducing this cost. And many of us will admit that even working on code we wrote previously is like working on another person's code.

Documentation is like a user manual for your project—when to use it, how to use it, and how to fix it if it breaks. It might also include information on how to contribute to the project or who to contact with questions.

Good documentation is the best way to convince others to use your open-source project. It breaks down barriers to access and empowers users to troubleshoot on their own. Documentation is searchable, which means that it's discoverable even if it's not well-organized. It doesn't need to perfect in order to be usable.

Documentation can be found in unlikely places, too. For instance, code comments and commit messages are a form of documentation.

The process of writing documentation can be a useful way of ensuring the quality of your code, too. By reviewing project components and use cases, you have the opportunity to spot weaknesses in your code. Think of it as helping out your future self, plus all the others who'll use your code in the future.

## How to get started

Before you start documenting your project, it might be helpful to answer these questions.

*The what?*

One of the initial steps in documentation is to define the scope of the documentation—what will be documented, what is out of scope and better explained elsewhere, what is the right level of detail, etc.

*The where?*

There are many choices for where your project's documentation could live—GitHub, your project website, Read the Docs ([https://readthedocs.org/](https://readthedocs.org/)), etc. Here's an example of Tarbell on Read the Docs, for example: [http://tarbell.readthedocs.io/en/latest/](http://tarbell.readthedocs.io/en/latest/).

[TODO: more about hosting documentation]

*The who?*

The audience for your project could be more than just your users. They could be editors or managers evaluating the project for future use or developers contributing to your project. Identifying your audience will shape the way you approach your documentation in terms of technical vocabulary and examples.

A few things to keep in mind: 

* **Setting expectations is always better if it's done early**—in life, and in your open source project. Upfront, your documentation should answer the question: "What do I need to know to use this project?" It is also helpful to give a time estimate of how long it will take to set up and get the project running. Here's a great blog post on setting expectations: [https://pantheon.io/blog/still-maintained](https://pantheon.io/blog/still-maintained)

* **Avoid or define jargon.** Link to documentation for dependencies, external libraries and technical terms. A glossary (eg: Github's glossary: [https://help.github.com/articles/github-glossary/](https://help.github.com/articles/github-glossary/)) can also ease the need to explain terminology. It is always a good practice to stay away from inside jokes and very deep cultural references that everyone may not get. While all the Arrested Development jokes in your documentation can make it refreshing for fans of the show, it could be confusing to others. That is not to say that all documentation and examples need to be bone dry. But being aware of the audience is great.

* **Think through the community's needs.** Good documentation acknowledges that the audience have different levels of need for detail. It may be a helpful exercise to identify the various audience groups for your project's documentation and separate them. For instance, documentation sections for users and administrators could be separated. E.g.: Panda Project: [http://pandaproject.net/docs/](http://pandaproject.net/docs/)

* **Recommend infrastructure.** Running code on your development machine is very different from running in production. A separate section about recommended infrastructure, deploying code to production, setting up caching, etc., could help. See Kinto project for an example of this: [http://kinto.readthedocs.io/en/stable/configuration/production.html](http://kinto.readthedocs.io/en/stable/configuration/production.html).

* **Note prerequisites.** If you have very specific prerequisites for your project, describe a way to check them. And do not assume that the reader knows their own machine setup. (For instance if you need a particular version of the library installed and your setup script does not handle it, document how to check it.)

A few more notes on how to approach documentation:

* **Be specific, but friendly and inviting** and don't make too many assumptions about potential contributors and their skill levels (or state these assumptions).

* **Remember that your project is not just code**, and people can contribute more than code—they can contribute ideas and perspective, too.

### Write a README

A common starting place for documentation is a README file—a file that lives in the project's root folder that contains the information users need to get started using the project. It's often a Markdown file (a type of text formatting, which we'll go into later) or a plain text file.

For the most part, every open source project should include a README. It's the first place most developers will look to familiarize themselves with a project. (And if you're new to open source, checking out project READMEs is a great first step.)

Here's what information a README generally contains:

1. What the project is and what it does

2. How to install the project

3. How to run the project

4. Future plans for the project and how to contribute

5. Credits and references

This [post by David Prager Branner](http://dpb.bitbucket.org/what-goes-in-a-readme.html) is a great concise guide to writing a good README. There's no single standard format for READMEs, but it helps to at least touch upon the information listed above.

> Many projects use Markdown, a lightweight text formatting language, to provide some semantic structure to their READMEs. To get started with Markdown, check out [this guide from Github](https://guides.github.com/features/mastering-markdown/).  It is suggest to rename your README to README.md if you are using markdown, as service like Github will parse and display the contents better.

There's no hard and fast rule that says your documentation has to live in a README, though–just think of the README as a starting point for the information your users will need. Some projects host their documentation on the project website or a site like [Read the Docs](https://readthedocs.org/), which provides structure and searchability. Should you host your documentation elsewhere, however, we strongly recommend that you link to the documentation from your README. The library [agate](https://github.com/wireservice/agate) is a good example of a project with a minimal README that links out to the project's crucial information.

### Make a CONTRIBUTING.md file

This file explains how people can contribute to your project. Put it in the top of your repo's file hierarchy. Here are some examples: [https://github.com/nayafia/contributing-template](https://github.com/nayafia/contributing-template)

* A great benefit of this approach when using GitHub is that [GitHub will add a link](https://github.com/blog/1184-contributing-guidelines) to this document when someone opens an issue or pull request.

* Example: [https://github.com/swcarpentry/git-novice/blob/gh-pages/CONTRIBUTING.md](https://github.com/swcarpentry/git-novice/blob/gh-pages/CONTRIBUTING.md)

### Comment wisely

Project documentation falls into three buckets—documentation for yourself, for others who work on the same project, and for everyone else who might want to use your code.

Code comments and sensible variable naming are often the best way to document for yourself. Every developer has at least once asked themselves, "What was I thinking?" when reading code they wrote in the past. Your future self will thank you for the time you put into adding comments to the code.

In addition to explaining what, the best commit messages also explain *why*. They do not rely on your memory of the context or repeat what the code does without adding any additional information.

```
// Bad comment
// Dividing time by 24.623 and converting to integer
var days = parseInt(time / 24.623);

// Better code and comment
const HOURS_IN_MARS_DAY = 24.623;
// Calculate the number of full days spent on mars
var daysOnMars = parseInt(timeSpentOnMars / HOURS_IN_MARS_DAY);
```
Above: Example of code comments acting as documentation

Code comments also help others working on the codebase with you use it better. It can be used to establish clear code reuse guidelines and set expectations at a granular level in the program.

It can be tempting to leave brief comments in your code, but make sure they are descriptive enough to be helpful to someone unfamiliar with the project. For example, you might want to label a section of your code `// parser function`, but that doesn't tell us much. A concise but descriptive comment like `// parses user-input string into first and last names` will be more valuable to people trying to understand your code.

### Prepare groundwork for multiple languages

Writing documentation in multiple languages will increase the reach. But most of us are not fluent in more than a couple languages at the most. Document how someone could contribute documentation in a different language.

## Examples and tutorials

Comprehensive API specifications can be helpful for users trying to debug or accomplish specific tasks, but they don't provide much of a jumping-off point to users unfamiliar with your code. Real-world applications of your project can give users a sense of what your tool can accomplish and familiarize them with how your code works.

Some projects, such as [csvkit](https://csvkit.readthedocs.io/en/540/tutorial/1_getting_started.html)) include a simple tutorial as an introduction to the project. Others, [such as d3](https://github.com/d3/d3/wiki/Gallery), might include a list of possible use cases alongside the code that powers them. [Elex provides examples](http://elex.readthedocs.io/en/stable/index.html) on multiple levels of complexity: an [introductory tutorial](http://elex.readthedocs.io/en/stable/tutorial.html)), brief ["recipes" of code](http://elex.readthedocs.io/en/stable/recipes.html) for common usage patterns and links to full-blown [implementations](http://elex.readthedocs.io/en/stable/index.html#elex-projects-and-implementations).

### Best practices for example code

The best examples usually illustrate a single concept or clearly explain the individual steps of a process. We recommend describing the goal or expected outcome at the start of the example code, like in [this jsFiddle tutorial](http://doc.jsfiddle.net/tutorial.html#first-fiddle-hello-world-goodbye-world).

Example code should be easy for the user to execute on their own. Any data or assets used by the example code should be easy for users to access. Many open source repositories [include example files](https://github.com/nprapps/mapturner/tree/master/examples) so users don't have to come up with sample assets of their own.

When a project has an elaborate setup or requires purchasing external licenses, setting up a demo server allows potential users to try it out before committing time and money to it. When Vox Media added a demo server [for Autotune](https://github.com/voxmedia/autotune), they noticed an increase in interest in the project.

A demo server like the one [for Mozilla's Kinto project](http://kinto.readthedocs.io/en/stable/tutorials/first-steps.html) can make it easy to write example code for API endpoints that users can run easily. Similarly: [Zulip](https://github.com/zulip/zulip-gci/blob/master/request-remote-dev.md) and [Dreamwidth](http://hack.dreamwidth.net/) offer hosted installations, for free, to new contributors.

### How do I decide what examples to show?

It's impossible to anticipate and document every possible use case of your project—the key is to build enough of a foundation for new users to work off of. Start by describing a typical use case for your project. [Census Reporter](https://github.com/censusreporter/censusreporter#getting-data-from-our-api-the-basics) anticipates some of the commonly used endpoints of its API and describes how to construct variations on the queries.

Don't be afraid to encourage your user base to contribute examples, too. The [d3.js example gallery](https://github.com/d3/d3/wiki/Gallery) includes hundreds of examples created by users and covers a variety of subjects, concepts and experience levels.

## Testing your documentation

If you have the time and resources, you might conduct some user testing to determine what examples will be most helpful to show. While developing a tool at the Washington Post, project maintainers wrote an initial draft of the documentation and observed "beta testers" as they followed the documentation to accomplish certain tasks. This revealed different user assumptions and use cases that could then be incorporated into future versions of the documentation.

## Document code debugging

What do you do when your code doesn't work the way you expect it to work? Look at error logs? Turn on verbose logging? These are all great tips to pass on to users of your project. A good section on debugging should contain the following:

* Where do the logs live?

* Are there various levels of logging? If yes, how do you switch between them

* Are there errors that you might encounter frequently?

Debugging sections, like most other documentation, should not be prescriptive. While providing your tooling and setup details as an example could be helpful, the documentation should not assume any specific tooling or environment setup. 

## Consider the style guide

Additionally, many news organizations have a style guide (AP, NYT, etc.) and these should be familiar to the originators of the project in setting the format for any text or prose involved, if necessary. Your team may also have style guides for code, design and documentation. Make sure you share them and set the expectations for contributors. It's much easier to review and merge a new feature if it already conforms (or nearly conforms) to your existing standards.

[TODO: add style guide examples]

## Managing documentation debt

As your project grows and code changes, your documentation and code may get out of sync. As new people start using your code, you might realize documentation gaps. These pending tasks around documentation is called documentation debt.

At Vox Media's Storytelling Studio team, documentation debt is tracked as Trello cards and when they have accrued about 30 cards, the team[ sets aside a day](https://storytelling.voxmedia.com/2016/7/29/12299564/on-building-a-culture-of-documentation) to update documentation. Establishing a system for updating documentation that fits into your working mode is important in making sure that documentation is still usable.

The NPR Visuals team and the Institute for Nonprofit News both use onboarding as an opportunity to address documentation debt. NPR Visuals asks new team members to follow the team's [setup document](http://blog.apps.npr.org/2013/06/06/how-to-setup-a-developers-environment.html) and update it with any changes they encounter along the way. INN invites new employees to review [team documentation](https://github.com/INN/docs/blob/master/staffing/onboarding/sample-onboarding-plan.md) and submit pull requests when they see areas for improvement.

> At my job, there's a project I work on in which every other Tuesday I devote time to making fixes and updates. It streamlines the process and sets expectations for the whole team on when the project gets updated. *— Mallory Busch*

## Checklist

- [ ] Decide on the scope of the documentation
- [ ] Decide where you will host your documentation
- [ ] Decide who you're writing your documentation for (users, new contributors, experienced contributors, etc.)
- [ ] Write a README that contains: 
    - a project summary
    - installation instructions
    - how to run the project
    - future plans for the project 
    - how to contribute to the project (or a link to your CONTRIBUTING file)
    - credits
- [ ] If documentation is hosted elsewhere, put a minimal README that links to it with the code
- [ ] Use code comments
- [ ] Write clear commit messages
- [ ] Document differences between running development code and production code
- [ ] Write example or tutorial code
- [ ] Document debugging resources (logging, frequent errors, how to run tests)
