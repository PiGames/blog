---
layout: "post"
title: "How does the blog work?"
date: "2017-06-11 21:22"
author: "bibixx"
categories: "General"
---

Hey everyone! I'm glad you are here. After quite some time I finally made myself to write something. Today I would like to show you how I have created this blog in just a few hours (2/3 to be precise).

## What powers this blog?
Some time ago I've heard about [Jekyll](https://jekyllrb.com) – blog-aware, static site generator powered by Ruby. I decided to use it because we aren't rich yet (Yet! :wink:) and we can't afford web hosting so we are using GitHub's Pages that are really easy to setup with Jekyll. All you have to do is make a commit! You don't have to use any sophisticated way to commit only build folder as GitHub does it all for us (I believe it builds Jekyll on its own).

## So is it any good?
Definitely! Especially for a front-end dev that doesn't really enjoy PHP. Creating this page involved almost no coding (actually CSS only but I had already written in while creating <http://pigam.es>) as you pretty much only use HTML and [Liquid](https://github.com/Shopify/liquid/wiki) (template engine). Apart from this Jekyll has built in SASS compiler and creates a local server after typing `jekyll serve` into the console.

## And how do you actually use it?
After setting up ([How to do it?](https://jekyllrb.com/docs/quickstart/)) and creating own template to create a post you simply create a markdown file with a [Front Matter](https://jekyllrb.com/docs/frontmatter/) at the top where you specify attributes of your post (eg. title, date of creation, author, etc.) and then you simply write a post in markdown (actually it is [kramdown](https://kramdown.gettalong.org/) but you can easily change it in `_config.yml`).

This section in code is looks like this:
```markdown
---
layout: "post"
title: "How does the blog work?"
date: "2017-06-11 21:22"
author: "bibixx"
categories: "blog"
---

Hey everyone! I'm glad you are here. After quite some time I finally made myself to write something.

## What powers this blog?
Some time ago I've heard about [Jekyll](https://jekyllrb.com) – blog-aware, static site generator powered by Ruby. I decided to use it because we aren't rich yet (Yet! :wink:) and we can't afford web hosing so we are using GitHub's Pages that are really easy to setup with Jekyll. All you have to do is make a commit! You don't have to use any sophisticated way to commit only build folder as GitHub does it all for us (I believe it builds Jekyll on its own).

## So is it any good?
Definitely! Especially for a front-end dev that doesn't really enjoy PHP. Creating this page involved almost no coding (actually CSS only but I had already written in while creating <http://pigam.es>) as you pretty much only use HTML and [Liquid](https://github.com/Shopify/liquid/wiki) (template engine). Apart from this Jekyll has built in SASS compiler and creates a local server after typing `jekyll serve` into the console.

## And how do you actually use it?
After setting up ([How to do it?](https://jekyllrb.com/docs/quickstart/)) and creating own template to create a post you simply create a markdown file with a [Front Matter](https://jekyllrb.com/docs/frontmatter/) at the top where you specify attributes of your post (eg. title, date of creation, author, etc.) and then you simply write a post in markdown (actually it is [kramdown](https://kramdown.gettalong.org/) but you can easily change it in `_config.yml`).

This file pretty much looks like this:
```markdown
---
layout: "post"
title: "How does the blog work?"
date: "2017-06-11 21:22"
author: "bibixx"
categories: "blog"
---

...

## And how do you actually use it?
After setting up ([How to do it?](https://jekyllrb.com/docs/quickstart/)) and creating own template to create a post you simply create a markdown file with a [Front Matter](https://jekyllrb.com/docs/frontmatter/) at the top where you specify attributes of your post (eg. title, date of creation, author, etc.) and then you simply write a post in markdown (actually it is [kramdown](https://kramdown.gettalong.org/) but you can easily change it in `_config.yml`).
```

## Have you added any additional features?
As it is pretty much a IT blog first thing I thought about was Emojis! Who doesn't like emojis? For sure people that spend most of their time in the internet. So an easy solution to this was [jemoji](https://github.com/jekyll/jemoji). After installing it you simply use it as you would for example on Slack – `:wink:` will show up as :wink: (unfortunately i couldn't find a way to add skin color eg. for :+1:).

Something else? Obviously code highlighting. I have used [Prism](http://prismjs.com/). It offers a lot of languages, themes (we are using atom's One Dark or something that kinda looks like it) as well as some plugins.

## TL;DR
Jekyll is an awesome tool to quickly create static customisable blogs using markdown with a lot of potential and features. (And can have emojis!)
