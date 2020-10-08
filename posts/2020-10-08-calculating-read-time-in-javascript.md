---
layout: layouts/post.njk
title: Calculating Read time in JavaScript
date: 2020-10-08T01:51:48.715Z
description: Today, I will show you how to calculate read time in JavaScript.
tags:
  - javascript
---
This is a very simple task. First, we need a sentence to try this out. Let's use "The quick brown fox jumps over the lazy dog".  A few thing we need to know is:

- The average word is 5 in the English dictionary.
- The average Words Per Minute for reading (WPM) is 200-250, which averages to 225 WPM. ([https://archive.is/FRfWJ](https://archive.is/FRfWJ)).

So, we have to split the text every 5 letters and divide it by 225 WPM. This can easily be done with JavaScript:

```jsx
"The quick brown fox jumps over the lazy dog.".match(/.{1,5}/g).length/225;
```

Which should return a value of `0.04`. So are we done? No. We also need make it human readable. First we need to round to the nearest whole number by using `Math.round()` :

```jsx
Math.round("The quick brown fox jumps over the lazy dog.".match(/.{1,5}/g).length/225);
```

Which should return `0`. Now we are almost done. Let's make it human readable. We can give it summaries using if/else statements. 

Lets use:

- Less than a minute read - for read times under a minute.
- `n` min read - for read times that are over a minute.

as statements.
```jsx
var rt = Math.round("The quick brown fox jumps over the lazy dog.".match(/.{1,5}/g).length/225);
  if (rt <= 0) {
  rt = "Less than a minute read."
  } else if (rt === 1){
  rt = `${rt} min read.`
  } else if (isNaN(rt)){
  rt = "Failed to calculate readtime!"
  } else {
  rt = "Failed to calculate readtime!"
  }
```
which returns `Less than a minute read.`

Let's make it ready for "production" by wrapping it around a function and compressing it using [JScompress](https://jscompress.com/). I put the source code on [P2Pbin](https://dev.to/aboutdavid/p2pbin-a-peer-to-peer-paste-sharing-site-with-no-servers-2f8c), which you can find [here.](https://p2pbin.glitch.me/?id=QmSUskuMStqUSb4huDVDWc94UPE3v5AyX2aNp4nUoWw9tp)