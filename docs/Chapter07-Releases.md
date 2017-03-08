# Chapter 7: Managing Releases

When you're reading a liveblog of a news event, you look at the timestamps of the individual posts, to see whether reporters are still updating it or whether it's finished. Similarly, people who are thinking about using your software want to know whether it's alive (improving consistently) or dead (no longer getting improved). They look for the most recent time you've published an updated version of the software, and they look for a roadmap indicating when and how you're likely to improve it further.

When you publish a new, updated version of the software for other people to install and use, another phrase for that is "releasing a new version" of the software, "pushing a new release".

The work of improving software can be slow and pretty invisible to other people (inside and outside your newsroom). Publishing and updating a roadmap, and pushing new releases of your software, will make your work more visible, help you schedule work collaboratively with others, and persuade other newsrooms to use your software.

## Version numbers

You will almost certainly want to assign [version numbers](http://producingoss.com/en/development-cycle.html#release-numbering) to different versions of your software. This practice sets expectations for users,  developers, and robots and allows people to manage their dependencies without breaking things. As a general rule, you should always update the project's version number when you update the code.

A common version numbering scheme is ["semantic versioning"](http://semver.org/), which uses a sequence of three numbers, like v1.5.2.

The first number is the "major" version, and should increase whenever you change your project in a way that could break someone's existing code if they switched to the new version. For example, if you're currently at v1.5.2 and you rename part of the API, you should bump the version from v1.5.2 to v2.0.0. This new "major" version will signal that a user may not be able to upgrade without also updating other code.

The second number is the "minor" version, and should increase when you add new functionality without modifying existing functionality. So if you add a new helper function, you should increase the version from v1.5.2 to v1.6.0. This will signal that the project has new features, and that a user can safely upgrade with their existing code.

The third number is the "patch" version, and should increase when you fix bugs or refactor things behind the scenes.

Typically a major version of 0 (e.g. v0.5.0) indicates that the project is still in early development and publishing a v1.0 release is a signal that the project is more mature. But there are no particular rules about this. Some projects quickly start jumping through major versions, while others stay below v1.0 for years. Rather than getting too hung up on unwritten rules about these numbers, focus on communicating clearly in your documentation about what's changing and where the project is headed in the future.

For another perspective on version numbering, read [Jeremy Ashkenas' thoughts on the matter](https://gist.github.com/jashkenas/cbd2b088e20279ae2c8e).

## A few pro tips on communicating about releases

* After you push a new release, be ready for an increase in the number of questions and contacts you get—customer support, offers to partner, questions about whether you can add new features, etc. New publicity generates these.

* Maintain a publicly visible web page that prominently points to the release notes and the package and source code for the most recent release, and instructions for installing it, and has (or links to) the important known problems ("known issues"), e.g., stuff for users to watch out for (risks of data loss or "you have to whack it at step 4" stuff especially).

## Roadmap and release planning

Make public announcements about the state of your project! Including if you choose to stop maintaining it (see [Chapter 8](Chapter08-Handoffs-Sunsets.md)); it happens, it's OK, just tell the world. Keeping users up-to-date helps you ask contributors for help that will be effective.

Roadmap examples:

* [Zulip roadmap](https://zulip.readthedocs.io/en/latest/roadmap.html)

* [TODO: more roadmap examples]

Every so often it's a good idea to initiate conversation with some of your users to ask them what should be in the roadmap.

### Using open source in your own newsroom

Don't let the open source edition of your code diverge substantially from what you really use in your newsroom. If you do this, it will:

* Decrease the benefits you get from other people's usage (bug reports and patches)

* Make you more sloppy in keeping a good usable history

This means you should by default be [using the open source version in your own newsroom](https://en.wikipedia.org/wiki/Eating_your_own_dog_food), and that you should build time into your project planning to do code review and to push new releases.

## Consistency versus speed

You may think people want to see a new release every week-and some people may. But if you intend to keep improving a project, it's more important to just demonstrate consistent attention. Consider what makes the most sense for your project and team: time-based releases (e.g. every couple of months), or feature-based (trying to finish a particular feature before the release is done).

> "Deadlines are not arbitrary, they're a promise we make to ourselves and our users that helps us rein in the endless possibilities of things that could be a part of every release. ... The more frequent and regular releases are, the less important it is for any particular feature to be in this release. If it doesn't make it for this one, it'll just be a few months before the next one. When releases become unpredictable or few and far between, there's more pressure to try and squeeze in that one more thing because it's going to be so long before the next one. Delay begets delay." - [WordPress](https://wordpress.org/about/philosophy/)

[TODO: more case studies on release management]

## Checklist

A release checklist could include:

* [ ] Sanitize secrets and personally identifiable information (See [Chapter 4](Chapter04-Code-First-Release.md))

* [ ] Summarize the changes you've made since the last release (refer to logs in the source control system, like Git, and do a search in your bug tracker), emphasizing changes that fix security vulnerabilities or will require your users to change their workflows or software/hardware setups

    * USE MILESTONES! Assigning issues and merged pull requests to milestones make it super easy to review what was changed. ([Example](https://github.com/wp-cli/wp-cli/milestone/48?closed=1))

* [ ] Make a list of important known problems with this release in particular—for each known issue, point to the relevant bug in your public bug tracker

* [ ] Make a list of who all contributed to those changes. Decide whether this includes, for you, people who contributed bug reports, mailing list posts, etc. ([Example](https://github.com/github/hub/issues/1355))

* [ ] Add links for people to get the complete list of changes since the last release

* [ ] Increment the version number

* [ ] Create a new package based on the current version of your code

* [ ] Publish the summary, the known-issues list, the contributor list, and the links (together, the "release notes") to a public webpage (such as your project blog) and publicize it to your user community (via an announcement-only mailing list, Twitter, etc.)

* [ ] Update the roadmap
