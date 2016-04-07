---
title: Web Project: Ruby Blog
date: 2014-05-20 07:45 PM
category: Dais
---

For the second of my [new projects](/2014/05/07/starting-projects/) I said I wanted to

> Deploy a server side app on a self-managed VPS

That's pretty vague and could get pretty complicated depending on the app so I need to strive to keep it simple to start. Especially because I have **zero** experience deploying VPS's. But it should be something I can expand upon and grow over time.

When I started blogging a couple years ago I settled on [Wordpress](http://wordpress.org) after much research because of the large userbase and large plugin capabilities. I knew very little about blogging or web programming so it gave me a good starting point.

After working in Wordpress's code base and trying to customize aspects of my blog, I've learned I don't need everything Wordpress offers. It ultimately makes the code harder to work with and me less likely to try things out. Also, [despite recently supporting markdown](http://jetpack.me/2014/01/31/jetpack-2-8-introducing-markdown-and-improving-monitor/), the markdown is still stored in a database which is far less portable. With those thoughts in mind, I've wanted to create my own blogging engine for some time.

So I've decided to create my own blogging engine to meet my specific needs. My list of desired features:

1. **Markdown** - must support parsing of raw [markdown](http://daringfireball.net/projects/markdown/) files
2. **RSS** - I doubt anyone subscribes right now but having an RSS feed is important
3. **Ruby** - I have no strong attachment to PHP so I want to use/learn something new. I've chosen Ruby since it's a mature language that I would definitely consider for the future but have never used.
4. **Bootstrap** - I've played around with [Bootstrap](http://getbootstrap.com) in the past and think it's a solid front-end framework. This is an opportunity to get better at using it.
5. **Self-Managed VPS** - to keep with the learning theme and to truly have portability and control, I want to deploy my new blog on a self-managed VPS
6. **Series** - a specialty feature I want is the ability to group posts into series, for example all posts associated with this project

I think that's it for now. It will probably be extremely basic and I may forgo #6 at initial launch to reduce complexity. But it's something I want to keep in mind throughout the design.

One thing I'm missing is a name which I'll be trying to come up with soon since I gotta name the directory something to get started!