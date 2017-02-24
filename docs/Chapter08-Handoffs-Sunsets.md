# Chapter 8: Handoffs and Sunsets

**Hello darkness, my old friend**

![nothing lives forever](https://media.opennews.org/fieldguides/open-sourcing/yorick.jpg)

It is almost certain that you and your open source project will need to part ways. It's a perfectly natural part of the open-source lifecycle, and you shouldn't feel bad about it. But that doesn't make the process any easier. Endings don't write themselves, and your preparations for the end are like writing a will: They are not fun, but they will make a difficult time much smoother if you can prepare in advance. If you don't actively end your project or separate from it, you can leave current and potential users in the dark. This can lead to confusion or mistrust in you or your organization. Think about how much work you put into getting your project off the ground; shutting down your project should take about this much work, possibly more. But fear not, planning for succession can make a big difference in how easily the transition occurs. 

## Why you might part ways with your project

Anyone who starts an open-source project will probably need to end that project, or at least stop being involved. Is it normal for you to love your project like crazy in the beginning but later lose time, lose interest, ... or even start to resent it? Yes. Yes. Affirmative. Some reasons you might part ways with your project: 

* You have no more time to commit to the project, e.g., you've retired from software development and now run a goat farm in Wisconsin.

* Your original needs have changed, e.g., you don't need a scraper of Federal Election Commission filings anymore because you've transferred to the desk that matches readers to Hogwarts houses.

* A group of contributors are largely running your project and you'd like to permanently hand off control to them.

* It doesn't spark joy. You've burned out and need to shed some responsibility. You have unevaluated pull requests. You have open tickets and don't want to close them. You don't really use your project anymore.

## What path I should take?

![you are standing on a path](https://media.opennews.org/fieldguides/open-sourcing/telnet.gif)

There are three paths to separating yourself from an open-source project. 

* You can hand off your project to new maintainers. 

* You can archive or preserve your project for future code archaeologists. 

* You can remove your project from the internet, e.g., kill it. 

## How should I decide which path to choose?

Do you have maintainers to pick up the slack? Consider handing it off, especially if you'd like people to keep using your project.

Could someone benefit from seeing your approach, even if it was wrong? Consider preserving or archiving your project. You could note that the project is no longer being maintained but still encourage forks, so long as it's not dangerous for someone else to keep using the code.

Does the project somehow do harm to you or people who might use it or read about it? You might be interested in removing it from the internet, especially if you don't want to be affiliated with it anymore.

Only the first path means that your project will still be updated/maintained.

> A few reasons your project may not be worth updating or maintaining:

> * It costs you more than it's worth, either in maintenance or community-building and public relations.

> * You or your users have decided to use another tool instead, e.g., Kenneth Reitz has released FECless.py, Federal Election Commission data for humans, and it's much better than your open-source series of Perl scripts.

> * A core assumption behind the project has changed materially, or some important part of the process has changed, e.g., the FEC has a new API that obviates the need for your scraper.

## Treading Down Your Chosen Path

Here's more about the three main paths to take as your project dies or your involvement as the lead goes away. 

### Handing Off Your Project

![handoff](https://media.opennews.org/fieldguides/open-sourcing/handoff.gif)

Ideally, your project is successful and there is an active community around the project, so changing leadership is the best move. If your project is not that busy, then don't worry, skip ahead to the **archiving your project** or **killing your project** sections.

#### Choosing new leadership

Depending on the level of community involvement, you may already have other people who are heavy contributors and taking the lead on things.  These will be the best candidates to take a handoff.

If you do not have these heavy contributors in your community, then it may be difficult to find someone.  Hopefully you have a forum, list, chat channel, etc., to be able to communicate to your users and contributors as a way to make a call for new leadership.  An important consideration is whether you trust that new maintainers will do as good of a job maintaining the project as you did. Ultimately, handing off the project to them (when the project has been associated with you or your organization) can be interpreted as an extension of trust.

#### Setting expectations for a new administration

In discussing a handoff to new maintainers, it's important to communicate the expectations of what it means to lead the project. And if you've followed the guidelines from previous chapters, most of these things will already be coded into documentation and the community!

It's usually easy enough to communicate the mechanics of code and the mechanics of the project. Although it is more difficult, it's often even more important to communicate the ethos of the project and your leadership.

#### Items to discuss with new leadership

* The top level goal of the project

* Who the audience is

* Code of conduct

* Conflict resolution

* Code philosophy

#### Communicate with your users

With new administration, there will likely be changes, and it is important to communicate these changes, or even lack of change to the people that use your project. Make sure to explain changes to your users with as much advance notice as possible. Send out notices often enough to make sure people are reminded but not bothered.  And send out notices through multiple channels whenever possible.

#### Things that need to be handed over

There are some mechanics of handing off, mostly around access and ownership of code and project resources.  These things may be split amount other people, or may already be held responsible by others.

* Ownership of the repository

* Ownership of communication channels, e.g., Slack, email lists, Twitter accounts

* Keys to servers

* Intellectual property like logos

### Archiving Your Project

![they named the dog Indiana](https://media.opennews.org/fieldguides/open-sourcing/indy.gif)

If there isn't a natural set of maintainers for your project, you might consider archiving it. The main goal with archiving a project is communication.

#### What do I need to communicate to existing users?

* You should explain that there will be no more updates to the project.

* You should encourage your existing users to fork the project if there are features waiting to be implemented.

* You should point to alternative projects.

#### What do I need to communicate to future users?

* Tell them: "What you see is what you get."

* Create a pinned tweet about the project's status, if there's a Twitter account.

* [TODO: more communication principles]

#### How do I demonstrate that my project is unmaintained?

* Update the README with a clear indicator of the project status:

    * Badges: [https://github.com/badges/stability-badges](https://github.com/badges/stability-badges)

    * A "this is no longer actively maintained" message.

    * Implications for lack of maintenance, e.g., might not install, returns bad data, etc.

* Python: In PyPi, set the development status to 7 -- Inactive

* Python: How to deprecate a module [https://www.python.org/dev/peps/pep-0004/](https://www.python.org/dev/peps/pep-0004/)

* Ruby: [https://www.ruby-toolbox.com/categories/Deprecation_Tools](https://www.ruby-toolbox.com/categories/Deprecation_Tools) (ironically, one of the most-used Ruby deprecation tools has itself been abandoned)

* [TODO: further advice for other languages and platforms]

### Killing Your Project

![he sure was a crazy, wonderful dog](https://media.opennews.org/fieldguides/open-sourcing/yeller.gif)

In some instances, you may want to remove your code from the internet.  Here are some things to think about before you make this decision.

#### Should I just archive my project instead?

If you answer yes to any of these questions, then you might want to archive your project.

* Are people actively using it?

* Is it linked to and used from a package manager?

* Is it useful as an example or other learning opportunity?

* Is it important to yourself or organization for the purposes of transparency?

* Can it serve as a warning to others?

#### Why would I want to kill my project?

If you didn't answer yes to any of those questions, you might consider killing off your code. Here is a list of questions to consider:

* Do you no longer want to be associated with the code?

* Does your organization want the code down, maybe due to license issues?

* Does the code harm, or not have value as described above?

#### Removing your project from popular package managers

<table>
  <tr>
    <td>Language</td>
    <td>Package Manager</td>
    <td>Command</td>
    <td>Link</td>
  </tr>
  <tr>
    <td>Python</td>
    <td>PyPi</td>
    <td></td>
    <td>http://stackoverflow.com/questions/20403387/how-to-remove-a-package-from-pypi</td>
  </tr>
  <tr>
    <td>Node.js</td>
    <td>NPM</td>
    <td>npm unpublish</td>
    <td>https://docs.npmjs.com/cli/unpublish</td>
  </tr>
  <tr>
    <td>Ruby</td>
    <td>Ruby Gems</td>
    <td>gem yank</td>
    <td>http://blog.rubygems.org/2015/04/13/permadelete-on-yank.html</td>
  </tr>
</table>


## This Is The Form Our Grief Has Taken

Here are some examples of how developers have sunsetted or handed off their code.

### Case Study

[TODO: CSVKit case study suggested]

### Case Study

[TODO: Sunlight Foundation case study suggested]

### Case Study

[TODO: ProPublica case study suggested]

## It Is Finished

![white shores, and beyond, a far green country under a swift sunrise](https://media.opennews.org/fieldguides/open-sourcing/sunset.gif)

Now that you have passed on your project, take a moment to feel good about the work you accomplished and what more you can do in the future.

You may feel guilty or irresponsible for letting go of a project, especially if this is one of your first open source projects or one you were heavily involved in, but rest easy. This happens all the time, and the world continues to spin.

### Case studies

> The 2009 Burton Street Project worked, thanks to all the alliances and collaborations that emerged, despite limited resources at the newspaper where it originated.  This collaborative  structure also made it unstable in the long run, though. About a year after the project won awards, some of the developers approached the newspaper about using the code and creating a similar project for a neighborhood facing a comparable situation, further east in North Carolina. Even though the publication was willing, those developers' personal circumstances changed, and the project faltered. The code remained with the newspaper, and the project was hosted on its site, despite the promises to release the code publicly to anyone who asked.

> In 2014, the Burton Street Project completely disappeared from the newspaper's site, in the midst of the publication's hasty redesign. This happened after a period of considerable turnover at the publication due to mismanagement, and team that had originally put the project together had turned over. The project, and the code that made it possible, were completely lost because there was no clear way to preserve it or hand it off to another entity.

> The lesson: Clearer planning for the open source aspect of the project would have made a huge difference. While some projects have natural ends, this one could have been far more useful, for far longer. It helped provide a direct platform for a marginalized area in Asheville and could have helped do the same in other places. Its end was premature and not due to any intentional plan, but simple negligence, poor planning and lack of clear prioritization. It's what can happen without a clear handoff/sunset plan.

> For more on the Burton Street Project's use of collaboration among multiple groups to complete a project with limited resources, see [Chapter 1](Chapter01-Choosing-Open-Source.md). For more on it as an example of successful community communication, see [Chapter 6](Chapter06-Community.md).
