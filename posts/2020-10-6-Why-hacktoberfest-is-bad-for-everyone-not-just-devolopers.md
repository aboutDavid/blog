---
layout: layouts/post.njk
title: Why hacktoberfest is bad for developers and open-source projects.
date: 2020-10-06T04:00:00.000Z
description: Hacktoberfest is supposed to get new developers to make pull
  requests, but it really just causes spam.
featuredpost: true
tags:
  - hacktoberfest
---
So, a few days ago something called "Hacktoberfest" designed to help get developers new to GitHub or who are uncomfortable with making Pull Request (PRs) get started making Pull Requests.

This might sound good, but, they are giving rewards to everyone who make 4 pull requests on GitHub. People will make small edits to try to trick the system. So this:

```
console.log("Hello world");
```

would become:

```
console.log("Hello World!");
```

The only thing that changed was a exclamation mark. This kind of change also would be what the spammer would do to try to win a prize. This causes a bunch of spam. That same spam also comes to your project. Now you are behind and they are preventing you from fixing crucial bugs. [Click here to see some example of spam on GitHub.](https://github.com/search?q=imporve+docs&type=issues)

And get this, it's not just GitHub. It's was also [DEV](https://dev.to), but the issue was [fixed](https://twitter.com/ThePracticalDev/status/1313515828810186752).

Learn more about Hacktoberfest spam [here](https://twitter.com/shitoberfest) and [here](https://github.com/shitoberfest/spam-pullrequests)