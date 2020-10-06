---
layout: layouts/post.njk
title: Why hacktoberfest is bad for everyone, not just devolopers.
date: 2020-10-06T04:00:00.000Z
description: Hacktoberfest is supposed to get new developers to make pull
  requests, but that might not help anyone
featuredpost: true
tags:
  - hacktoberfest
---


So, a few days ago something called "Hacktoberfest" designed to help get developers new to GitHub or who are uncomfortable with making Pull Request (PRs) get started making Pull Requests.

This might sound good, but, they are giving rewards to everyone who make 4 pull requests on GitHub. People will make small edits to try to trick the system. So this:

```
console.log("Hello world")
```

would become:

```
console.log("Hello World!")
```

this kind of change would be what the spammer would do to try to win a prize This causes a bunch of spam.



Ok, this doesn't affect me. Why should I care?

You should care and this **can** affect you. How? Say the repo "securitytool" contains a bunch of tools for securing your password. The maintainers are too busy to fix exploits that can leak passwords. A hacker finds a exploit and uses it to steal your password. Then they have access to your accounts and they can pretend to be you. They can steal your money. They could trash your reputation. They could do almost anything that they want to.

This is why Hacktober is bad for everyone.
