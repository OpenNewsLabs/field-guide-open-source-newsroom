# Chapter 4: Code: Getting To The First Release

In this chapter, we'll talk about how to set up your open source project and write code in ways that:

* Make it easy for you and others to track progress and help each other

* Keep private data out of stuff you publish

* Reduce and prevent bugs

* Reduce unnecessary work

* Increase the chances people will use the software

## So what are we doing here?

**We aren't just making code.** We're working in a shared workplace—even though it's an online place rather than a physical newsroom or laboratory, making stuff together. The work includes not just writing functions and classes, but experimenting and planning and coming up with "we ought to do this" ideas. And so we should try to make sure anyone coming into our shared workplace can take a look at what we've already said and done, and reuse the work that's been done already. 

**Let's say it again: we aren't just making code.** We're making history—a usable history, one that you can use, and one that the contributor next year can use. This is why we'll talk about how to use a [source control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) (a.k.a. [version control](https://en.wikipedia.org/wiki/Version_control)) system that tracks who's done what and why. This is why we suggest you use a public bug tracker for your TODOs. And it's why it's important to be careful about what you publish (as code or in places like the bug tracker), because once you publish something on the Internet, it's impossible to completely erase.

First, though, one side note: it's important to keep in mind that everything in this chapter is the ideal. Given your time and resources, doing all of them (well) may be difficult.  It's hard to say what the bare minimum is for a successful open source project, but keep in mind that not all open source projects will have everything here.

## Version control

There are several version control systems you can use to host your repository, but we recommend Git and GitHub, which is the most popular system among open source and newsroom communities. Here are a few resources for every level, whether you're familiar with Git yet or not.

### Git

Especially if you're going to be the maintainer on a code level, [learn to use Git beyond just push and pull](https://www.harihareswara.net/sumana/2014/10/31/0). 

Here's a basic Git lesson: [https://openhatch.org/missions/git](https://openhatch.org/missions/git) 

Clone a repo of a project you don't care about and try the more advanced commands as you make little changes to the code, so if you ruin everything you haven't actually set your own work back. 

Learn to branch and merge and work with remotes and cherry-pick and bisect. Read [this super useful explanation of the Git model](http://web.mit.edu/nelhage/Public/git-slides-2009.pdf), which articulates what's actually doing what—it helps.  

More resources:

* Why you want to work in branches and how to do so: [http://producingoss.com/en/vc.html#branches](http://producingoss.com/en/vc.html#branches)

* A successful Git branching model: [http://nvie.com/posts/a-successful-git-branching-model/](http://nvie.com/posts/a-successful-git-branching-model/)

## Helping others contribute

Help people figure out how to contribute to your project.  One of the many benefits of open source is getting others to look at and improve your code.  It's important to make this process as easy as possible by specifically documenting how to do it.  A few ways to make this happen:

* **Focus on good documentation and contributor's guidelines.** See Chapter 5 for lots more about this.

* **Things like dependency management**, Docker, etc., are good technologies to help people get contributing faster. [TODO: more examples here]

## Tracking issues

Use a public bug/issue tracker.  Your code is probably going to have some issues in it or need improvements, and it's important for people to be able to communicate these issues to you.  It's also really beneficial to have these issues in the public so that others who may have the same issue can find it and possibly solve the issues themselves.

* If you are using GitHub, you can utilize GitHub issues.

* It's probably a good idea to note where people can report issues in your README or main documentation.

* Consider avoiding using GitHub issues for support, to mitigate being overwhelmed by support questions.

Help people see how to ask questions/contribute bug reports.  To help make issues more efficient for you and your users, you can also add things like how to [search for existing issues](http://wp-cli.org/docs/bug-reports/) and questions.  

GitHub allows you to make [issue templates](https://help.github.com/articles/creating-an-issue-template-for-your-repository/), which are really helpful for efficiency:

* Example issue template:

```
### What were you trying to do? Please include the version of the software you were using.

### What did you expect to happen?

### What happened instead? If you saw an error message, please also paste it here.
```

## Versioning

Each release of your software should have a version associated with it. This is often a 3-digit sequence, like 1.2.3 and the most common scheme for this is [Semantic Versioning](http://semver.org/), which attempts to communicate some level of compatibility with specific number and placements.

## Packaging/distribution

If you want other newsrooms to use your project, then in each release you need to give them a version they can install (like a downloadable app or a "package").

Use what your users need-if it's an app, put it in the Apple App Store or the Google Play Store.  Most common software languages have a centralized package manager, which makes getting and managing code modules easy.

<table>
  <tr>
    <td>Language or tool</td>
    <td>Package manager</td>
  </tr>
  <tr>
    <td>Javascript</td>
    <td>NPM</td>
  </tr>
  <tr>
    <td>CSS or HTML</td>
    <td>NPM (and less so Bower)</td>
  </tr>
  <tr>
    <td>Python</td>
    <td>PyPI</td>
  </tr>
  <tr>
    <td>Ruby</td>
    <td>RubyGems</td>
  </tr>
  <tr>
    <td>PHP</td>
    <td>Composer</td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
  </tr>
</table>


More details on how to deal with rare cases and little questions of procedure: [http://producingoss.com/en/packaging.html](http://producingoss.com/en/packaging.html)

## Dependencies

Work with the frameworks and dependencies that are popular within your users' community and known to be stable.  Using unstable or unmaintained dependencies may cause your project to become unstable.

For example: If your users are using Python 2.7 and haven't moved to Python 3 yet, you should probably make it so your application runs on Python 2.7.  If your users are on Windows mostly, make sure that your thing runs on Windows.

Use the most appropriate package manager for dependencies. (See "Packaging" below).  This will make for an easy, predictable install or development process.

Sometimes it may be best to try to avoid dependencies because they are not stable, or maybe you simply want to avoid a cumbersome install.  (For instance, installing dependencies for frontend interfaces that use a browser can be difficult, or too varied, and may not be worth it.)

## Is your project sanitary? 

Flip back to [Chapter 3](Chapter03-Existing-Projects.md), where we talk about really important considerations to keep important information and data safe and private. 

## Automated testing and continuous integration

More automated tests in/for your codebase are better, because they reduce regressions so you can move faster and merge others' code faster (and let others review and merge code faster), but don't sweat getting to 100%, because there's definitely a decreasing marginal utility to this stuff. [Travis CI](https://travis-ci.org/) is pretty easy to set up for the common case.  

Some resources on debugging:

* Systematic Debugging: [http://akaptur.com/blog/2013/07/24/systematic-debugging/](http://akaptur.com/blog/2013/07/24/systematic-debugging/)

* Rough Notes for New FLOSS Contributors On The Scientific Method and Usable History: [https://www.harihareswara.net/sumana/2016/10/12/0](https://www.harihareswara.net/sumana/2016/10/12/0) 

Here are some document generation tools for different languages:

* Doxygen - Java, 

* Pydoc

* Swagger

[TODO: identify more documentation tools]

[TODO: info on identifying common bugs, errors, and user errors]

Here's a great overview of getting to the first release:

* Releasing Open Source: [http://wiki.civiccommons.org/Releasing_Open_Source/](http://wiki.civiccommons.org/Releasing_Open_Source/) 

## Finishing Up

[TODO: checklist]
