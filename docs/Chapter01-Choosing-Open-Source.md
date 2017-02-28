# Chapter 1: Choosing Open Source, and Getting Buy-In

Before your project even begins—before you start thinking about documentation, languages or contributor guidelines—figure out whether you need to get support for your open source project within your newsroom. Establishing buy-in creates a culture where open source projects, big and small, are valued and supported. And it builds a solid foundation for ambitious open source projects to succeed in the long term. 

Often this means convincing people in different levels of leadership that your involvement in open source software is worth both time and resources. Specifically, you'll need to convince other people that the upsides are greater than the downsides. When making your case, you can clearly identify both, and determine a time period after when you'll evaluate your involvement in the project.

## Who needs to be on board? 

From the beginning, it's good to assume that everyone in your organization has some level of stake in your project and will need to be on board. If you're at a larger organization, this might mean the legal team, PR department, or the executive editor. At a smaller organization with fewer staff members, this might mean just a handful of colleagues, even though the same legal or PR concerns apply. 

## What's the value of open sourcing?

In order to get buy-in for making something open source, it's important to know why people open source their work in the first place. There is a range of benefits that come with open sourcing (though, of course, there are some tradeoffs that you should be aware of, too). Understanding the question of "what's the value of open sourcing, anyway?" from many different angles will help you talk about it with people who may have different priorities than you. 

The following lists have been paraphrased from community suggestions, as well as outside resources like [OpenSource.com](https://opensource.com/life/15/12/why-open-source), [Open Source Everything!](http://tom.preston-werner.com/2011/11/22/open-source-everything.html), and [Why Open Source](http://www.dwheeler.com/oss_fs_why.html).

**Engineering Benefits of Open Sourcing:**

* **Quicker bug detection and bug fixing.** When software is proprietary, the only people who can detect and fix bugs are the engineers on that team. Open sourcing your software means that your code can be reviewed by a much wider group of people, tested in a much larger set of circumstances, and fixed by the huge ecosystem of coders outside your team. Remember [Linus's Law](https://en.wikipedia.org/wiki/Linus%27s_Law): "Given enough eyeballs, all [bugs](https://en.wikipedia.org/wiki/Software_bug) are shallow"

* **Straightforward collaboration.** Open source permits companies to collaborate on common problems, without complicated business partnerships, prior agreements, etc., allowing solutions to be better and arrive more quickly.

* **Encouraging modularity.** Coding in public can lead to code that's cleaner, more secure, and more modularly architected — which is a good thing for internal development as well. By making your code flexible and modular enough for the public to use on a variety of projects, you help future-proof that tool for your internal teams.

* **Higher standard of work**. There is a minimum bar in creating successful open source projects, such as documenting, commenting, not committing sensitive information, that make for good code projects in general. Even assuming a project could be open source will help drive better practices.

**PR/Business Benefits of Open Sourcing**

* **Intersection of commercial needs.** Open source permits companies to collaborate on common problems, without complicated business partnerships, prior agreements, etc.

* **Good press from good projects.** Successful open source projects generate publicity and public goodwill. It also gives the company a chance to put a stake in the ground and shape the conversation around a particular piece of technology or service.

* **You get to make the wheel, not reinvent it.** Giving other people access to your code means they don't have to reinvent the wheel, and it also means that they can spend that energy improving your wheel instead. For example, [Resque](https://github.com/resque/resque) has been cited as an example of this: In addition to being improved by outside developers, the tool also had hundreds of developers providing third-party plugins to extend the tool's functionality for free. Rather than an ecosystem of related but different and incompatible tools, the community effort went toward porting Resque and making it broader and more extendable, making Resque more valuable in turn.

* **Recruiting and funding.** Quality open source projects help attract developers who can inspire the work you're doing and get inspired by it. For those newsrooms supported by community funders, it can be helpful for them to see your organization as a leader in the industry. 

**Ethical, Transparency, and Accountability Benefits of Open Sourcing**

* **Giving back to the community.** If you use computers at all, there's a good chance some open source is involved. If you're a developer, you're probably dependent on dozens of open source tools. Give back to future developers by open sourcing your own work as well.

* **Maintaining a consistent attitude towards transparency across the company.** In the same way that journalists cite their data sources and explain their methodological processes, open sourcing software makes it transparent to readers and users. It pushes the organization to interrogate its own processes and reflect on them.

* **The value of redundancy and distributability. **The more we open source—especially data—the more resources we're able to give journalists to do their jobs. Further, the more distributed one particular resource is, the less likely it is to be deleted or entirely censored by some outside force.

To round out this list, here are a couple more resources:

* [On the value of working in the open](http://www.poynter.org/2011/6-reasons-journalists-should-show-your-work-while-learning-creating/150243/)

* [How open source infrastructure added value to Instagram](https://medium.com/@nayafia/open-source-was-worth-at-least-143m-of-instagram-s-1b-acquisition-808bb85e4681#.opxzo84x0)

## Questions and misconceptions about open sourcing

Here's a list of questions and misconceptions that we've encountered while open sourcing projects, especially when first introducing the open source concept to an organization. Some of these concerns have straightforward answers, while others require you to think long-term about the scope of your project. Mix and match from the scripts below as you find them useful.

If you come across questions or concerns not listed here, always remember that there's a good chance that someone or some other organization has dealt with the same thing, and reaching out to the community at large might turn up a good response. (And you can always reach out to the people behind this Field Guide at [fieldguide@opennews.org](mailto:fieldguide@opennews.org))

### Legal/PR

These departments are generally concerned with the public face of the organization, especially regarding liability and potential press (positive and negative). They might be concerned about any legal rights a contributor might have to an open source project, the project failing in public, or about how having unfinished code might look to outsiders.

*If they ask "What's our liability here?"*

You can say:

* "Let's talk through the license options and figure out which one is best for our needs" (See [Chapter 2](Chapter02-Starting-New-Project.md) for more information on choosing a license.)

* "The [license we chose] gives us cover for _______ and ______. That should assuage any concerns about liability."

*What risks come with each of these licenses?*

* "[This is a great resource](http://wiki.civiccommons.org/Choosing_a_License) on the pros and cons of various open source licenses."

* "Since these licenses are well known and have been used on many projects, we can learn from people who have gone before us."

* Some resources on open source case law: 

    * [https://poststatus.com/thesis-automattic-and-wordpress/](https://poststatus.com/thesis-automattic-and-wordpress/)

    * [http://wpandlegalstuff.com/category/gpl/](http://wpandlegalstuff.com/category/gpl/) 

*How will open sourcing incomplete code make us look?*

* "Contributing to the open source community increases the visibility of our work, and demonstrates a net good added to journalism. Our PR people can talk about our contributions to the community, as well as promote projects that are using our tools."

* "Open sourcing a project helps us stake a claim to our idea early. It shows that we're leaders in our field and we help move the industry forward."

* "We'll establish a clear set of guidelines for both code contribution and community conduct, in order to make sure the project maintains the rigorous standards of our organization." (See [Chapter 6](Chapter06-Community.md) for more information on how to do this.)

*How do we make sure proprietary information is not part of the open source release?*

* "We'll follow established practices for sanitizing codebases before we release them to the public eye." (See [Chapter 3](Chapter03-Existing-Projects.md) for more information on how to do this.)

* "We'll make sure you're in the loop about our releases so you can flag any concerns about proprietary information."

* "Here are specifics about what we'll be open sourcing and what will remain internal/proprietary:" 

### Newsroom leaders

How do you sell a project to top editors, technology leaders, project managers and others who have decision-making power around newsroom priorities? Here are some common questions and concerns that might come up as you pitch an open source project to these high-stakes stakeholders.

*If they ask "What if someone takes our code and does our idea first?"*

You can say:

* "It's always a risk that competitors are working on similar projects and ideas. What we'd be releasing is the tool, not the content or the specific story ideas."

* "We can collaborate on tools/data and compete on the stories/execution."

* "We can plan our release schedule to coincide with launching our [story/project]. That way people can build on our coverage moving forward, but we don't have to worry about getting scooped because we post our code/data."

*What's the actual good that comes out of this (for the community and for us)? Why should we spend time/energy/resources on this?*

* "Open sourcing will allow us to maintain our competitive advantage. We get to drive a larger conversation about how to solve problem X instead of sitting alone in a corner trying to solve it by ourselves."

* "Being involved in this project marks us as a leader in our field, and allows us to move journalism forward (while also moving our organization forward)."

* (potentially) "Free user testing!"

* "We have run into challenges with ____ and ____ time and again. By devoting resources to this project, we'll be solving [specific problem in the newsroom] and freeing up time for our developers in the long run."

* "Open sourcing our work will make us design elegantly and exercise discipline in our development, and in so doing, help us minimize technical debt." ([paraphrase of](http://opensourcebridge.org/wiki/2010/The_Second_Step:_HOWTO_encourage_open_source_work_at_for-profits#LEGAL_POLICY) Sumana Harihareswara)

* "Opening data/software has become even more important as data becomes less transparent." 

* "Open sourcing code is a lot like explaining our methodology on an investigative piece—it allows our readers to understand how we built something, the assumptions we made, and encourages greater transparency in our processes."

* "Along those lines, open sourcing encourages us to interrogate our assumptions about how we built a tool, analyzed data, or approached a problem."

* "We benefit from open source (data/tools) and have a responsibility to contribute back to the community."

* "Given the prevalence of open source, we become more competitive/attractive for hiring potential developers. The highest quality developers quite frequently tend to have some experience creating or maintaining open source projects, and those developers are attracted to companies that have some sort of open source culture."

*I don't want to work with/help the competitor.*

* "By working with partners, we'll be more likely to find funding for long-term maintenance and future projects."

* "This project doesn't compromise our unique mission or goals, but it will give us the foundation to do that work more readily."

* "They have resources we need, and this allows us access to those resources without having to hire."

* "Some of the most successful media companies—places like ProPublica, Vox, and the New York Times—work collaboratively and share open source tools. They've proven that collaboration is good for business."

*Are we going to end up footing the bill for this when everyone else can use it for free?*

* "Investing our resources now will be rewarded in the long term, because we continue to confront [this specific issue] and this tool will address those problems."

* "Partnering with others and releasing this open source will allow us to get contributions from people outside our newsroom—we benefit from other people's donated time and experience."

* "Software is never free—even if someone is using our open source software, they will need to devote resources to it, same as us."

* "Though there are costs to open sourcing, we still need to spend resources to write this code."

*Last time we did this, it was a spectacular failure. Why will this be different?*

* "You're right, [past project] ran into some very real obstacles. Here's how we plan to learn from that and make this project more successful: _______"

* Talk about why a previous project "failed," what went *well*, and how you are planning to avoid those obstacles this time around. 

* Present a clear timeline and roadmap, along with contingency plans for when issues inevitably arise.

* Post-mortems are a good place to start planting the seed for the next project. Invite key stakeholders to discuss projects after the fact, *especially* if they didn't go particularly well.

### Your immediate boss

By "immediate boss," we're speaking primarily about the people who manage your (and/or your team's) day-to-day schedule and resources. These people are concerned with how an open source project will affect everyone's workload, both over the short term and the long term as the project enters maintenance mode.

*If they ask "How much time is this going to take? How long are you going to be working on it?"*

You can say:

* "Here's how much time I plan to spend on this every week. (Share a detailed plan and a roadmap for first phase of the project.)" (Don't have this yet? See [Chapter 4](Chapter04-Code-First-Release.md) for advice on scoping this out.)

* "Part of open sourcing will be defining what sort of maintenance we plan to have for this tool, and communicating that to our audience. We can explain whether the project is maintained, if it's supported, and if we're accepting contributions upfront, which will help us manage those expectations." (More advice [here](https://pantheon.io/blog/still-maintained).)

* "Here's the value I think this project will provide: [give specific examples that tie into your bigger organizational goals]."

* "Given the value this will add, how do you think I should prioritize this with my other projects?"

*How are you going to balance this with other projects?*

* "This project will make our work on ______ and ______ so much easier, and take as much time each week as we spend on [project example/meeting/checking twitter]."

* Seek their input: "Given the value this will add, how do *you* think I should prioritize this with my other projects?"

* "I think I can spend X hours every week on this without my other work suffering. If I send you an update at the end of each week with a progress report, we can evaluate how to prioritize this project as we move forward."

### Clients/Business People

Whether you're dealing with an external client or an internal business team, you'll probably need to justify open sourcing software against your organization's bottom line.

*If they ask "How do we make money on this?"*

You can say:

* "Depending on the license used, you can still sell sponsorships/ads on a particular project."

* "If the project is successful and has proven value, there is the potential for grant funding/support."

* Send them this [handy guide](https://github.com/nayafia/lemonade-stand)

* A few resources for grants:

    * [https://www.opensocietyfoundations.org/grants/open-society-fellowship](https://www.opensocietyfoundations.org/grants/open-society-fellowship) 

    * [https://meta.wikimedia.org/wiki/Grants:Project](https://meta.wikimedia.org/wiki/Grants:Project) 

    * [http://www.knightfoundation.org/programs](http://www.knightfoundation.org/programs) 

    * [https://www.mozilla.org/en-US/grants/](https://www.mozilla.org/en-US/grants/) 

    * [https://www.opentech.fund/](https://www.opentech.fund/) 

    * [https://www.python.org/psf/grants/](https://www.python.org/psf/grants/)

*Why should I/we be the ones to pay for a thing that everyone benefits from?*

* "You will be seen as a leader and contributor to the wider industry, which comes with a lot of recognition. You're investing in something a lot of people will use and your company will be associated with it. You'll be credited with every other org that uses this tool."

* "You may benefit from someone else doing the same thing in the future (karma)."

* "You're getting others' contributions for free going forward. Why pay for one developer to maintain a piece of proprietary software forever when you can have 50* developers contribute for free!"

### Partners

Maybe you have a partnership with another newsroom already, or maybe you think that having one would greatly help your open source project. Different newsrooms have different cultures and different feelings about open sourcing: whether to do it at all, which license to use, and what workflows and community guidelines to follow to keep things running smoothly.

*If they ask "Why should we work with you?"*

You can say:

* "This is a problem we all face and pooling resources will help us solve it more effectively (and avoid solving the problem over and over again)."

* "We have a clear plan, with defined goals and a timeline."

* "By working together, we have a stronger chance of convincing foundations to support our project."

*What do we get out of this?*

* "It's budget-friendly. This is a problem we all face, and pooling resources will help us solve it more effectively (and avoid solving the problem over and over again)."

* "Your name will be on an open source project that's top-notch and well-respected."

*We have different newsroom needs, how will we resolve disputes/conflicts?*

* "We'll identify a lead from each of our teams, and that core group of stakeholders will work together to identify scope."

* "Together, we should identify shared goals and values for this project and refer to that mission statement/project manifesto when we run into problems."

* "We'll set up a team Slack for day-to-day issues and conversations, and have a weekly check in with stakeholders to make sure we're on the right track." 

### Developers

Given the amount of time that maintaining an open source project can take up, you'll likely find developers who are concerned about what open sourcing a project will do to their schedule. They're probably well aware that potential contributors/users will be expecting up-to-date documentation and examples, regular releases and responses to pull requests, and bugfixes as the tool is used more widely.

*If they ask "How much work will this add to my plate (in both the short-term and long-term)?"*

* Have a conversation with your developers and include them in the process of deciding whether a project is worth open sourcing. e.g., Why do you think this is important? What do we stand to gain from contributing back to the community in this way? With the other projects on your plate, can you balance five hours a week for this project? Ten hours?

* Clearly explain the roles of a project: Who will handle support in the long term? Is there a sunsetting plan? Define their responsibilities from the outset.

* "Part of open sourcing will be defining what sort of maintenance we plan to have for this tool, and communicating that to our audience. We can explain whether the project is maintained, if it's supported, and if we're accepting contributions upfront, which will help us manage those expectations." (More advice [here](https://pantheon.io/blog/still-maintained).)

### You!

Before embarking on an open source adventure, it's important to reflect on whether you have the time and resources to contribute.

* Do I even have time for this?

* Is this something I want to work on long-term?

* How much time do I have to give this? How do I scale back (or scale up) my involvement over time? 

* Am I going to maintain this? Or am I just releasing it into the wild?

* Is someone already working on a tool/project like this? Would this be significantly additive to newsroom open source code? Is a better use of time simply contributing to an existing, similar project?

## Case Studies

### CASE STUDY: Collaborating across departments

#### [How Quartz Created Chartbuilder](http://www.niemanlab.org/2013/07/how-to-turn-everyone-in-your-newsroom-into-a-graphics-editor/)

"Of course, getting our staff onboard and using Chartbuilder was not an overnight process. But with the aid of our most chart-reliant reporters, we quickly got everyone trained and using Chartbuilder with a 30-minute demonstration followed by one-on-one troubleshooting as problems arose." 

### CASE STUDY: Collaborating across organizations (recruiting partners, communication, funding)

#### Burton Street Project

In 2009, the Burton Street Project started as a way to help tell the story of the Burton Street Community, a primarily African-American neighborhood in Asheville that was facing multiple demolitions as part of a proposed interstate expansion that threatened to end it. The newspaper was relatively small, and its in-house expertise and resources were limited. Some in its newsroom were absolutely averse to projects beyond traditional print journalism. Eventually three reporters, an editor, a local photographers group, two web staff from the newspaper with development experience (and enthusiasm for open source) and several local open source enthusiasts (different ones at various points) all collaborated to complete the project, communicating with neighborhood leaders and residents and involving them directly.

The idea was to show through multiple fronts exactly what the community was facing, with maps, photographs, traditional stories and directly contributed information from the residents sharing its history and stories while creating an easy way for the public to present and interact with the information.

Because there are no shortage of neighborhoods facing these situations around the country, the idea was also to create a model that could be transferred and quickly used by others who needed it (hence why making the code publicly available was an aspect, though not the primary one I focused on as one of the reporters).

> For more on the Burton Street Project as an example of successful community communication, see [Chapter 6](Chapter06-Community.md). For more on its eventual long-run problems due to lack of sunset planning, see [Chapter 8](Chapter08-Handoffs-Sunsets.md).

### Code for Asheville Voter Education Tool

Code for Asheville (CoA) sought to build an open source voting tool for the 2016 elections that would cover the multitude of races on the ballot, going beyond President, Governor and U.S. Senator to key but far less-covered campaigns like attorney general, county commissioner and local bond referendums. Multiple local media organizations had already had representatives contact or get contacted by CoA, as had Buncombe's Election Services. In this case, the existing connections help quickly make possible discussions and coordination (eventually, deciding to have everyone meet and work face-to-face) to finalize the voter education tool with multiple types of expertise at the table.

### More resources 

* [Building smart newsroom tools by Melody Kramer](https://source.opennews.org/en-US/learning/building-smart-newsroom-tools/)

* [Good Code Runs on Good Communication](https://source.opennews.org/en-US/articles/code-runs-communication/)

* [How The Los Angeles Times Transformed its Publishing Tools with a UX Design Approach](https://source.opennews.org/en-US/articles/how-los-angeles-times-transformed-its-publishing-t/)

* [Four reasons why an open-source newsroom is harder than it looks: Lessons from Al Jazeera](http://www.niemanlab.org/2012/09/four-reasons-why-an-open-source-newsroom-is-harder-than-it-looks-lessons-from-al-jazeera/)

# Conclusion

Obtaining buy-in from the various groups in and around your newsroom can feel overwhelming — but when you're armed with a clear sense of purpose and an achievable roadmap, getting that support is totally within your grasp. Let "no surprises" become your gospel. By communicating preemptively with all stakeholders, you are building a solid foundation for the project. Ultimately, these relationships will make or break an open source endeavor. 

Remember that it's okay to start small. Measure your results with concrete metrics, so that the next time around it's even easier to show folks why releasing an open source project has measurable benefits for your organization.

Now that you've learned some ways to tackle organizational resistance, let's jump right in and learn about starting a new open source project.
