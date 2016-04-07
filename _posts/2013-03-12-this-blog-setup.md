---
title: This Blog Setup
date: 2013-03-12 08:03 PM
category: This-Blog
---

## Setup

This blog uses [Wordpress](http://www.wordpress.org) which is one of the most popular blogging platforms available. When talking about Wordpress you need to be careful because there are 2 options. Wordpress.com and Wordpress.org. Both use the Wordpress blogging system but [Wordpress.com](http://www.wordpress.com) is a hosts solution as well. Wordpress.org provides the free software to self-host a site. I'm using the Wordpress.org software to host my site using [Blue Host](http://www.bluehost.com) shared hosting.

## How to Install
Installing Wordpress is extremely straightforward.  With most shared hosting options you have two installation options, install it yourself or use the SimpleScript option.   Check out [BlueHost Help](https://my.bluehost.com/cgi/help/wordpress) for an explanation of using SimpleScript to complete the install.  Because I want to be able to install multiple sites within the same shared hosting account, I installed Wordpress within a subdirectory of the public_html folder.

Wordpress has very [detailed instructions](http://codex.wordpress.org/Installing_WordPress) for installation.  You'll need to access your shared hosting through an FTP client and a text editor (I use  [Cyberduck](http://cyberduck.ch/) and [TextWrangler](https://itunes.apple.com/gb/app/textwrangler/id404010395?mt=12), both are free).  You'll also need to create a new SQL database.  Check with your shared host provider for how to do this.  I used the Bluehost instructions found [here](https://my.bluehost.com/cgi/help/6).

## Choose A Theme
The next task was deciding on a theme.  Wordpress has the great feature of keeping the content separate from the appearance.  The appearance is defined by the theme, and it can be changed without fear of affecting any of your content.  There a lots of theme options, both free and paid, so it's easy to get lost in the decision process.  

I knew for this blog I wanted to keep it simple and evolve it over time.  I also knew I wanted the theme to use [Twitter Bootstrap](http://twitter.github.com/bootstrap/) to make the site responsive and to start working with the Twitter Bootstrap framework.  I used a list at [OSTraining](http://www.ostraining.com/blog/wordpress/bootstrap/) to help narrow my search.  To keep things simple I decided on [The Bootstrap](http://wordpress.org/extend/themes/the-bootstrap) because it required the least work to get up and running and since it was available through Wordpress.org it's easily to update the theme if it's updated from the developer.

## Child Themes
The best way to modify a theme is through the use of a [child theme](http://codex.wordpress.org/Child_Themes).  This allows you to modify the theme without being destructive so that you can easily download updates to the base theme.  This is important because themes are constantly being evolved with both features and security updates.  The child theme process is very easy to setup, only requiring a style.css file to get started.  The only initial change I wanted to make was to make the header text in the sidebar smaller.  I just found it overwhelmingly large.   Making this change was easy:
>h2 { font-size:20px; margin:0 0 0 0;}

## Up and Running
And with that I was ready to start writing posts.  Another feature of self-hosted Wordpress blogs is plugins.  Plugins allow you to add extra capabilities to your blog with little modification.  In my next post I will outline all the plugins I'm using and why.