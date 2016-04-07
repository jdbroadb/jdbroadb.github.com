---
title:  Let It Go - Late Initialization of Let in Swift
date: 2015-08-09 10:23 AM
link:  http://natashatherobot.com/late-initialization-of-let-in-swift/
---

I was just playing with this the other day for defining class variables during init. Traditionally most values in a class would have been vars, despite knowing that I would set the value once when initializing the class. Now that can be a let and *should* be a let. But it's definitely a challenge rethinking how we use constants in our code.