# Chapter 6: Working With Community

You're ready to open source your work and you want to get the community involved. Great! Open source tools and data benefit most when they do have strong communities of users and contributors, so it's essential to invest time and effort in spreading the word about your project so it gets in front of people who might use and contribute to it.

> All the emotions. Just because you made something amazing—and we agree, it is—and even if you took all the right steps to making sure people know how to use it, and even though you made it really easy for contributions, and you followed this guide to the letter, people may not care.  

> At least at first.  

> It's hard not to take this personally, but as long as you like your work and you use the code, then it's totally fine.  It happens to us all, we promise.

This chapter covers how to build and manage a community around your work, including how to set clear expectations for conduct and governance, putting guidelines and processes in place to encourage participation, growing and managing your community and handling ongoing support and the public reception of the project.

## Setting expectations

In [Chapter 1](Chapter01-Choosing-Open-Source.md), we talked about how it's essential to set internal expectations early in the planning process. However, by the time the project heads toward being open to a wider public or community than those directly involved in its construction, setting expectations still remains an essential but different task. Developers and editorial team members should specifically confer about what expectations to convey. Some key questions to ask yourselves and each other:

* What are your goals? Are you trying to get other people to use your project? To contribute code to it? To inform the broader community or your funders? To promote your organization's brand?

* Who do you want to contribute? How will you build and maintain relationships with contributors?

* What sorts of contributions are you open to accepting? How much control do you want to maintain over the project?

* How much effort are you (or your team) willing/able to put into all of this?

* How much does a wider community need to be directly involved? Will they simply be using and accessing the data or project or is their involvement directly needed to contribute data/update/moderate it? If the latter, a greater degree of community engagement will be needed to make the project work at this point.

* How much control will the originating org(s) maintain? How much time/resources will be required to do so?

* What are the expectations around ongoing support? How quickly are you willing/able to respond to issues and feature requests?

* How much should we communicate about the philosophy of code for the project? For example, the idea of "Pythonic," or the very specific way of building D3.

* What does the eventual timeline for the project look like, and how does community involvement play a role in that? Does the level of that involvement change over that timeline? (Also see [Chapter 8](Chapter08-Handoffs-Sunsets.md))

## More to consider upfront

In [Chapter 5](Chapter05-Documentation.md), we covered best practices for documenting your code. We've gathered a few other things to think about in preparation to work with the community.

### Working with other orgs/partnerships

Does this project involve multiple organizations? Is it a partnership or other kind of collaboration? While that may cause some logistical and communication challenges earlier in the project (see [Chapter 1](Chapter01-Choosing-Open-Source.md)) it can really come in handy and make things easier here, as each org is more likely to have its own community, network and base of people it can quickly and easily reach out to.

Check in with any existing partners and make sure everyone's on the same page. This is also a time to think about bringing other potential partners onboard. Open up those lines of communication, and clarify strategies for reaching who you need to reach.

### Codes of conduct

Having a contributor code of conduct from the start can help show your commitment to anti-harassment, avoid future rules-lawyering around what is or isn't harassment, and help you shut down toxic behavior fast. More on the importance of a code of conduct and the ways to adopt a successful one can be found here:

* Christie Koehler: [The complex reality of adopting a meaningful code of conduct](https://subfictional.com/2016/01/25/the-complex-reality-of-adopting-a-meaningful-code-of-conduct/)

* INN: [Code of conduct and how to contribute](https://github.com/INN/docs/blob/master/how-to-work-with-us/contributing.md)

* Vox Media: [Contributing to a Vox Media open source project](https://github.com/voxmedia/open-source-contribution-guidelines)

For more example contributor codes of conduct, check out the [Contributor Covenant](http://contributor-covenant.org/) or the examples [listed here](http://geekfeminism.wikia.com/wiki/Code_of_conduct).

### Governance

As [Christie Koehler of Authentic Engine warns](https://subfictional.com/2016/01/25/the-complex-reality-of-adopting-a-meaningful-code-of-conduct/), it's never to early to think about governance. (The [Contributor Covenant](http://contributor-covenant.org/) is a popular starting point.) If you're under the umbrella of a software-related nonprofit, for instance [NumFOCUS](http://www.numfocus.org/), that'll help you make and implement these choices.

### Communication

Is there a central email or method for feedback? Who's in charge of moderation? Who's checking the Twitter hashtag? (If there is one.) Here's an example of what this might look like: [http://wp-cli.org/#support](http://wp-cli.org/#support). Also, Gitter is a chat client designed specifically for projects: [https://gitter.im/](https://gitter.im/).

Also, make it clear who's on the other end of the line, when a community member reaches out. Is it the folks who are the original contributors to the repo? The folks whose names appear on the ReadtheDocs? If they have moved on from the project/organization and different folks now maintain the project, clarify who these folks are.

### Fundraising

Fundraising, especially if a project attracts widespread community interest, is another particularly important aspect, particularly for smaller or non-profit organizations. While funds are important in the initial clearance stages described in [Chapter 1](Chapter01-Choosing-Open-Source.md), it's important to remind those who appreciate open source projects that these organizations and efforts might need funding in the future (to expand the project if it ends up requiring more resources than initially anticipated, for example).

## Accepting Developer Contributions

### Why?

In short, accepting open source contributions allows you to benefit from other people's experience. It may also help you to improve your project faster than you may be able to do on your own, bring in outside expertise, and build a support network to ensure your project lives on even if you're no longer able to maintain it yourself.

Contributors might help you with code review, fixing bugs, building new features, and generally improving the project. But they also help you identify blind spots. Contributions from people with a different perspective may help you identify things you may have simply missed, broaden your perspective and more.

There is also some inherent value in building things in the open. We build trust in journalism when we promote transparency, encourage more community involvement, and generally demystify our work. All these things help make the process of journalism less mysterious and hopefully will, with time, build (or rebuild) trust in our organizations.

### What kind of contributions will you accept?

As a developer, when you open source your work you may be thinking that people will help improve your code, build new features, or check off items on your roadmap. But there are many more ways to contribute to an open source project. When you prepare to release your project, you'll want to think about what sorts of contributions you want and make sure you communicate those needs clearly (see, for example, these [contributing guidelines from INN](https://github.com/INN/docs/blob/master/how-to-work-with-us/contributing.md)).

In general, and particularly as you're just starting to build a community around your project, no contribution is too small. Even submitting bug reports and feature requests is a great way for people to get involved. From there, some people might progress to helping with code review and quality assurance (QA) as a less-intimidating way to contribute to the codebase.

Some projects tag issues that are good starter tasks for someone who wants to help. For example, React has a ["good first bug" tag](https://github.com/facebook/react/labels/good%20first%20bug).

Keep in mind that non-technical people may also want to help with your project, and try to provide ways for them to get involved. Here are a few additional things you might consider:

* **Adding or improving documentation.** It's often helpful to have people who are not familiar with your project try to follow the instructions you've provided and note issues where they get stuck. You might also just need help copy editing or fleshing out your documentation, and this is often a great place for new contributors to get started.

* **Adding support for additional languages.** Depending on the project, you might want to make it available to users and contributors in different languages. This goes beyond just translating your documentation. You might also want to translate user-interface elements, inline documentation in the code or other content that appears in the project.

* **Community building and promotion.** Building and maintaining the community, triaging tickets and feature requests, promoting the project and encouraging adoption, and all of the other pieces involved in running a successful open source project are also great areas for less technical folks to contribute. You may need to provide volunteers with some guidance, instruction and documentation to perform these tasks, but you can to lighten your load by empowering some community members to build and manage the community around your project.

* **Issue triage.** Popular projects often see lots of non-actionable issues opened up. For example, an issue opened up on your project might actually be a problem with a different piece of software the user is using. Or it might be an unconstructive complaint. Or it might be a bug report that's too vague to pursue without more information. A non-technical contributor can help triage these issues by labeling, responding, and/or closing them.

[TODO: more ideas for non-technical contributions]

The most important thing is to make it as easy as possible for people to get involved and make that first contribution, in whatever form.

### Bug reports

Even if you just want people to help with reporting bugs, you'll want to make sure your community members know your preferred method of communication, how to submit bug reports and what a good bug report should contain. You can include a set of guidelines or a sample bug report for clarity.

Example bug report guidelines:

* [npm](https://github.com/npm/npm/wiki/Contributing-Guidelines)
* [D3](https://gist.github.com/mbostock/370b737ce71bed0749e103b01ce1bfaf)

If you're using GitHub, you can include your bug report template in the repo using the filename `ISSUE_TEMPLATE.md` and it will automatically populate for users opening new issues.

Example issue templates:

* [Bootstrap](https://github.com/twbs/bootstrap/blob/master/ISSUE_TEMPLATE.md)
* [Electron](https://github.com/electron/electron/blob/master/ISSUE_TEMPLATE.md)

Depending on the size and scope of your project, you'll likely handle bug reports and other community contributions a bit differently.

For smaller projects, you may be able to just accept occasional bug reports to your regular email address, but for a larger project (or if you manage a lot of projects), you may want to use a dedicated email address or even implement a bug tracking system to manage the volume of requests you receive.

[TODO: add recommendations for bug tracking systems, tips for different size/scale of projects/teams, etc.]

For very large projects you might even need a dedicated support person or community manager.

Whichever tools you choose to use, if you're hoping to see people pick off improvements or todo items, make sure you share your roadmap in a public place and lay out clearly defined issues with enough direction for a newcomer to jump in and work in a way that meshes with your team's process. You might also want to include flags (such as GitHub labels or tags) for things like "help wanted" or "good for beginners" to give new community members a sense of where to contribute.

Read more on recommendations overall in this [blog post by Sumana Harihareswara](https://www.harihareswara.net/sumana/2015/08/09/0).

### Promoting your open source project

So how do you promote your project, so that others will actually contribute? Open source projects succeed because they have strong backing and connection from the communities they involve. This applies even more so with open source news projects, which often involve issues affecting a larger community, from a neighborhood to a city or country.

Many news organizations already have close ties to their community, and by virtue of being a media company, they have a number of possible means of outreach readily available to them. In planning an initial release, it's worth thinking through which of these existing methods might work for promoting and marketing a particular project. Does the audience for your editorial content include designers, developers, and other potential contributors? Can they help you make connections with other members of your local tech community or help to spread the word about your projects? Are there existing news dev mailing lists (e.g. [NICAR-L](https://www.ire.org/resource-center/listservs/subscribe-nicar-l/)), conferences (e.g. [SRCCON](http://srccon.org/), [Mozfest](https://mozillafestival.org/), [NICAR](http://ire.org/conferences/nicar2017/)), Slack channels ([News Nerdery](http://newsnerdery.org/), [Lonely Coder](http://lcc-slack.herokuapp.com/), etc.), or meetups (e.g. [Hacks/Hackers](http://hackshackers.com/)) that might be interested in hearing about your project?

While these may be great places to start promoting your work, you'll also want to be proactive and seek out the communities of potential users and contributors most likely to be interested in your project. Think about your project's audience broadly:

* Are there similar news organizations who might benefit from your work?

* Is there a community around the language you're using who might be interested in how you're using it? (Some languages have more active communities than others.)

* Does your tool address needs beyond the newsroom context? (For example, a tool that helps clean and dedupe data might be useful for news developers, but it could also be useful for the broader community of data visualizers or data scientists.)

* What groups are intended to use/contribute to the project?

* What are the best ways to reach them? (Twitter, Github, Facebook, direct meetings with community leaders)

If you haven't made connections with these organizations, this can be a great opportunity to make those introductions and hopefully start an ongoing relationship where you'll be able to share and learn from one another for years to come.

Although a broad approach and technical platforms can be useful, don't forget to connect, one-on-one, with real potential community members who you might want to reach. Their input is key to developing an approach that will mesh with the reality. Consider what societal divides you might encounter, along lines of class, race, gender, and language. Make sure you don't unintentionally alienate potential community members from your project.

And, of course, a great way to draw interest and support from the open source community is to contribute to other open source projects yourself. Having a track record of being helpful in the open source community will make others more likely to help you.

In fact, for connecting with communities of all kinds, here's something big to keep in mind: Relationships are built over time, so do the work before you need it.

### Maintaining code quality

[TODO: info on how to say "no" politely, turn down PRs, etc. without chasing away well-meaning contributors]

### Crediting Contributors

Open source projects are often the product of contributions by many individual humans, often volunteering their free time. It's important to acknowledge their contributions and make them feel like valued members of your community. People may want to be recognized in different ways (or may not even want to be recognized at all), so make sure to ask people what they prefer. Here are a few ideas for how to recognize your contributors:

* Say thank you (publicly and/or privately)

* Add a GitHub label for community contributions

* Recognize people who contribute to each release in the release notes

* Send them stickers or other swag

* Consider giving regular contributors more responsibility/ownership/input

* Offer to write them letters of recommendation for their job/academic applications

* Check if people you know might want to hire them

* [TODO: more ideas on crediting contributors]

### In-person get-togethers

If your project includes contributors (paid or unpaid) from different cities, you should consider having in-person get-togethers a few times a year. [Here's why, and how to make them productive](https://modelviewculture.com/pieces/software-in-person).

## Accepting Editorial Contributions

For editorial projects, there are often other ways to get the community involved in your project. In these cases, it is important to focus on what the members of the community will directly gain from the project. What aspects of their community will be revealed? What problem will be dealt with or lessened? What information can they glean?

In doing so it's essential to remember that few communities, especially those served by news organizations, communicate just in one way. Consider a wide range of communication methods and narrow from there, but don't narrow too much or a potentially appealing project might not take off due to simple lack of awareness.

If the project needs the involvement of a particular part of a community (say, a neighborhood or workers in a certain industry), reaching out face-to-face to a community group or key individuals is essential in a way that it sometimes isn't when dealing with a primarily online community. Knowing which types of media, especially social media, are preferred by the groups in question and the best ways to reach them will help in both cases.

> **Case study:** For over three decades, Burton Street, a primarily African-American neighborhood in Asheville, has been threatened with devastation by a proposed interstate. In 2009, a local newspaper worked with a local photographers' organization and community members, shooting photos of spots they directed and setting up ways for them to submit stories and information about the homes that would be lost and the effects of the demolitions to create an online map and photo project that was easily navigable and searchable (and open to new contributions of information after it went public), and was later combined with video and a series of articles on the neighborhood's story and potential future. Because it gave the residents an opportunity to directly tell their story after decades of feeling that the larger city was ignoring them, most residents participated or contributed in some form and the project got widespread community support, in turn helping it get attention beyond the newspaper's primarily white readership.

> Shortly after the project's release and the ensuing public pressure, the state Department of Transportation committed to drastically scaling back the number of homes that would be demolished in Burton Street and the topic has remained much more prominent in local discussions and politics ever since, in the process raising awareness of the area's de facto segregation. That's led to recognition by local government of the Burton Street Community Association and funds for them to develop their own plan for the future of their community. The project won some state and national multimedia awards.

> For more on the Burton Street Project's coordination of multiple groups in a single effort, see [Chapter 1](Chapter01-Choosing-Open-Source.md). For more on its eventual long-run problems due to lack of sunset planning, see [Chapter 8](Chapter08-Handoffs-Sunsets.md).

### Verification

One particularly unique aspect for some open source news projects is the need for verification. If contributors are submitting data or information that requires verification for legal and ethical reasons, developers and editorial need to work closely together on a clear and coherent process that makes sure information is valid, but can allow for protection of a source's anonymity if necessary. [TODO: examples of verification]

## Dealing with the dark side of community

We want to also acknowledge that as with any community there exists the possibility that people will behave badly.

### Enforcing a Code of Conduct

Earlier in this chapter, we talked about agreeing on a code of conduct. Here's more on that. First, why have one? It's tempting to think that just because you haven't experienced harassment personally, or that your project hasn't yet had any hostile behavior, you don't need to adopt one—or that you can wait to adopt one until something happens. But in order to help ensure that the community around your project stays safe, welcoming, and open to people from all backgrounds, you'll want to have a contributor code of conduct that lays out what constitutes inappropriate behavior, and how the project team will handle it.

That said, simply having a contributor code of conduct isn't enough: You'll need to figure out who enforces it, and how. As you write or adopt a code of conduct, think about how you will practically and logistically address the following three points (adapted from the [Ada Initiative](https://adainitiative.org/2014/02/18/howto-design-a-code-of-conduct-for-your-community/)):

* Specifying which behaviors or kinds of behaviors are not okay

* Providing detailed directions for people to report CoC violations

* Coming up with a defined and documented complaint handling process, with people who can handle the reports, investigate whether they constitute violations of the CoC, and implement any punishments or responses applicable (from written warnings to permanent bans)

### Dealing with Opposition

In addition, sometimes institutions or interests may oppose an open source project because of the information that may be revealed and their beliefs about how that affects their political interests. It is important for all involved in the project to coordinate ahead of time and be aware of the political terrain in a given community so they can take a resolute and coordinated stance. This allows those involved, especially on the editorial side, to anticipate what will happen when it goes public so all the organizations involved can be ready to respond with points and defenses. Especially in the immediate aftermath of a project's release to the public, this can help shape perception in its favor and tie in with encouraging community involvement.

> **Case study:** Recently released records about the federal government's 1035 program supplying military surplus equipment and weapons to local police departments reveals that the police chief of a small Western NC town with a 7-person department received major amounts of equipment, including a grenade launcher. This was highlighted in a local newspaper. Said police chief resents this and accuses the press, loudly, of prying into law enforcement's business. The newspaper that published the information quickly defends their use of the open records as essential to protecting the public's right to know and draws more public support for delving into the records in the process.

> **Case study**: A coalition of local media are preparing a project where local workers, after verification, can submit info about their actual pay rates anonymously. A lobbying group representing restaurant owners attacks the project as hurting local business. The local media have anticipated this and have a joint statement ready asserting the project is necessary to decrease the stigma on talking about pay and compensation, especially in underpaid professions, and to possibly expose issues of pay discrepancies or discrimination, as well as reminding locals that these workers have a legal right to talk publicly about pay and conditions.

### Spam

Dealing with issue/ticket spam? [TODO: examples of orgs who open sourced editorial projects that had spam problems]

## Support

* [TODO: further information on support here]

* Managing support

* Paid vs. free

* Self care + dealing with burnout

> **Case study:** After coordinating with local election services, media and local developers, Code for Asheville convenes a meeting to work directly together on a voter tool for the 2016 elections, especially the lesser-known state and local races that may still have a big impact and be closely contested (one eventually came down to 300 votes). All parties have communicated in advance about what they intend to do, but discuss it further at the meeting to double-check that they're all on the same page. The media members and some local citizen activists write up descriptions of the local and state offices that aren't mired in legalese and convey the importance of the positions while recommending links for "read more" to local or state media that have covered the issues extensively so the reader can make their own decisions. Election services provided quick access to key data and tools they had developed. CoA handles the coding aspects. The result is a voter tool that gets wide local distribution, partly because of the cooperation with media and local election services. While there are multiple factors at play in any election, Buncombe ended up having considerably higher turnout than the state average.

## Checklist

- [ ] Have a code of conduct
- [ ] Discuss who will enforce the code of conduct and how they will do it
- [ ] Share your project's styleguide if you use one
- [ ] Work with editors to develop a verification process, if needed
- [ ] Have and publicize channels of communication (IRC channel, Slack, mailing list, issue tracker, etc.)
- [ ] Write a contribution document (e.g. CONTRIBUTING.md)
- [ ] Make sure your community members know your preferred method of communication, how to submit bug reports and what a good bug report should contain.
- [ ] Credit contributors
