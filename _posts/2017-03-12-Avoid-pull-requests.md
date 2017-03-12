---
layout: post
status: publish
published: true
title: 'Avoid pull requests'
author:
  display_name: Vicenç García Altés
  email: vincentredrum@gmail.com
  url: 'vgaltes.com'
author_login: vgaltesc
author_email: vincentredrum@gmail.com
categories:
- Teamwork
tags:
- Teamwork
comments: []
---
[Pull requests](https://help.github.com/articles/about-pull-requests/) are a common way to integrate your changes in another repository or branch in an Open Source project. They allow the receiver of the pull request to easily view and review the changes you made. Pull requests are great, especially when your team is not event not colocated, but in different time zones. It seems that their popularity has extended to enterprise projects as well, even when the team is co-located. Is in this situation when I consider pull requests a bad smell of team dynamics.

Our story starts after the sprint planning. Every member of the team chooses a story to begin working on and creates a branch. After several days working in this branch (and maybe in other ones), he decides is a good time to create a pull request. The pull request can be something like this:

![giant pull request](/images/giant-pull-request.png)

The poor team member that takes responsibility of merging the pull request spend the whole day reviewing the changes. You can imagine the quality of the review.

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">10 lines of code = 10 issues.<br><br>500 lines of code = &quot;looks fine.&quot;<br><br>Code reviews.</p>&mdash; I Am Devloper (@iamdevloper) <a href="https://twitter.com/iamdevloper/status/397664295875805184">November 5, 2013</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

So, what can you do to improve this situation?

The first option is to avoid the necessity of reviewing changes. Work in pairs when you develop a new story. I know that you can't [pair](https://www.thoughtworks.com/insights/blog/pairing-are-you-doing-it-wrong) all the time but use this tool as much as you can. The results will be much better because pairing is much better than reviewing. Talking with your partner about design decisions, naming, etc. is much better than just reviewing some code with much less context.

If you can't pair, at least review the code with its creator. Take a seat next to her, use your favourite remote pair programming tool or start a hangout/webex/whatever and go through the code. Ask for explanations of the decisions, test new approximations, discuss naming. But have a face to face conversation with her.

If for some inexplicable reason you can't pair or review the code with its creator, use tiny pull requests. Obviously, this is a general advice, please define small and incremental stories that involve the less code possible. The code will be better and the life of the teammate that will review the pull request will be much happier.

![I approve this pull request](/images/chuck-norris-pull-request.jpg)
