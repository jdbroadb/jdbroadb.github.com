---
 title: Ruby Frameworks
date: 2014-11-01 02:00 AM
category: Secret
---

When I started writing Ruby late last year the only framework I knew of was [Rails](http://rubyonrails.org/). In my head Ruby and Rails were practically synonymous. But as I got into Ruby and started to work on [Dais](http://www.coherentiterations.com/series/dais) I quickly learned that Rails wasn't the only game in town.

## Sinatra
[Sinatra](http://www.sinatrarb.com/) is an extremely lightweight web framework for Ruby. You can have a Sinatra project up in minutes. And I found it far less overwhelming and opinionated. I don't know that I would have wanted to write Dais using Rails, but I enjoyed writing it with Sinatra.

## Secret Project
One of the distinguishing features for me when starting my new project was that Rails had builtin support for databases using ActiveRecord. I quickly assumed

> "Rails is for projects with databases and Sinatra is for projects without"

I'm sure your thinking that's a silly generalization and today I would agree with you. But I started learning Rails under that assumption and I'm still happy I did.

Either framework can support databases and I've actually prototyped code using both. I struggled because there were things I liked and disliked about Rails but Sinatra is almost too unstructured. I couldn't decide which route to take and then I heard [Ruby Rogues Episode 170](http://rubyrogues.com/170-rr-padrino-with-dario-cravero-nathan-esquenazi-arthur-chiu/) on [Padrino](http://www.padrinorb.com/). I tested it out and I think I may be hooked. It has a lot of flexibility but also a lot of tools that build on Sinatra, like ORM support (I'm trying [Datamapper](http://datamapper.org/)), different renderers (I'm using [HAML](http://haml.info/)), and a bunch of generators and helpers. It just seems like the right balance for me.