---
title: Moving from Heroku to OpenShift
date: 2015-08-25 06:48 PM
category: Dais
---

A few months ago [Heroku](http://www.heroku.com) sent out a notice that they were changing their pricing. With that change they also let people know that they would be cracking down on the free tier usage. The free dynos are expected to go idle for at least 6 hours out of every 24.

I currently host two websites using my Dais framework, this site being one of them. Both sites have limited traffic and so it's hard to justify paying for hosting. The issue for Heroku is that both sites have RSS feeds and feed reader services ping them regularly for updates. It's not an option to remove the feeds, and I can't control the service ping frequency. So I started looking for alternatives.

One option would be to host both sites on the smallest [Digital Ocean](https://www.digitalocean.com/?refcode=5b9d90caaff6) VPS. It's only $5 a month and would get me started on basic Linux server administration. That's only $60 a year but I'd rather avoid the cost if possible. And while learning Linux administration is on my to-do list, it would be a distraction from the things I am working on right now.

So the preferred option was to find a Heroku replacement. I did some searching and found a few references to [OpenShift](http://www.openshift.com) by RedHat. Given that RedHat is a big name, I decided to check them out. They also have a free tier and it works a little differently, which is favorable for me. You can use up to three small *gears*, which are similar to dynos on Heroku, without providing a credit card. This will allow me to host both sites and have a spare gear. They also idle gears that aren't active, however, I saw no limitations that require idle time. This should hopefully allow me to keep the RSS readers happy.

I was a bit worried about the transition but it couldn't have been easier. Knowing what to do, it can all be done in a few minutes.

1. Create an OpenShift account
2. Create a domain
3. Create a Ruby 2.0 application - I used the web interface
4. Install the command line tools **rhc** - this automatically setup ssh based on my existing keys
5. Add a remote for **openshift** to my local repo of my app - the git url is available on the app settings page
6. Do a git pull and resolve the conflicts - I had two conflicts but I just deleted the OpenShift deltas
7. Commit the changes and push to origin
7. Setup environment variables using **rhc** for syncing with Dropbox
8. Git push repo to **openshift**
9. Site is now live on OpenShift url
10. Add alias to application on OpenShift website for www.coherentiterations.com
11. Update DNS CNAME on [Hover](https://hover.com/D1DyccZQ) to OpenShift URL
12. Site was instantly hosted from OpenShift instead of Heroku
