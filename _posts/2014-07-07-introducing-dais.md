---
title: Introducing Dais
date: 2014-07-07 09:55 PM
category: Dais
---

When I [announced](/2014/05/20/web-project-ruby-blog) I was working on a ruby based blogging engine I listed 6 goals for the project. I'm getting ready to move my blog over to using my new blog engine and I'm happy to say I met 5 of the 6 goals.

## What'd I Miss
Let's start with what I did. My blog engine does the following:

1. **Markdown** - All posts support markdown formatting through the use of [RedCarpet](https://github.com/vmg/redcarpet)
2. **RSS** - The engine generates a RSS feed that's accessible through /rss or /feed
3. **Ruby** - The engine is completely in Ruby
4. **Bootstrap** - I used [Bootstrap 3](http://getbootstrap.com/) as a CSS framework that makes the site responsive
5. **Series** - The posts have the option of being a part of a series and there is a series archive that lists the series and their posts

The missing item is the **Self-Hosted VPS**. I [was pretty clear](/2014/05/26/ruby-project-conscious-decisions) this was an important goal for me. And so I still have every intention of experimenting with VPS's but in my research I learned how easy it is to deploy a project to [Heroku](https://www.heroku.com/).  Bonus: It's also free for the low amount of traffic my blog gets.

## But Wait There's More

Along the way there were a lot of other things I learned and incorporated into the blogging engine.

1. **Dropbox Sync** - Since I decided to deploy to Heroku, I couldn't FTP files to the blog and I didn't want be limited to posting from my computer through Git pushes. The most logical option was to build in Dropbox syncing so I could write in any Dropbox accessible program on phone, tablet, or computer.
2. **Sinatra** - [As mentioned before](/2014/06/06/ruby-project-web-frameworks), I decided to use the Sinatra as the web framework.
3. **HAML** - Sinatra supports the use of templates and so I used it as an opportunity to try out [HAML](http://haml.info)
4. **Threads** - I used a continuous thread to periodically re-sync with Dropbox to capture any changes.
5. **Bigfoot** -  I incorporated [Bigfoot.js](http://www.bigfootjs.com) for all my footnotes
6. **Link Posts** - There is a URL field in the markdown file meta header for any post that is actually a link post.  This results in the title linking to the provided URL on both my page and in my RSS feed.
7. **Editorial Workflows** - While not really a feature of the engine, since it uses Dropbox for the content I was able to setup some simple Editorial workflows to create new posts and add images.

## The Name

I brainstormed quite a bit on an appropriate name and finally settle on **Dais**.  The [Meriam-Webster](http://www.merriam-webster.com/dictionary/dais) definition is:

> a raised platform in a large room or hall that people stand on when performing or speaking to an audience

Dais is the platform on which I speak to the world.

## Using Now

With any luck the DNS routes are updated and Coherent Iterations is officially hosted on Heroku using Dais.  I plan to continue this series of posts with lots of details on the technologies I decided to use and what I learned while writing Dais.  I'm also considering putting it up on GitHub as my first official open source project.
