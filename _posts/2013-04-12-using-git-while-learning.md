---
 title: Using Git While Learning
date: 2013-04-12 11:59 AM
---

Over the past few months I've been working my way through Big Nerd Ranch's books on [Objective-C](http://www.amazon.com/gp/product/0321706285/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=0321706285&linkCode=as2&tag=cohereiterat-20) <[AL](/affiliate-disclaimer)> and [iOS Development](http://www.amazon.com/gp/product/0321821521/ref=as_li_ss_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=0321821521&linkCode=as2&tag=cohereiterat-20) <[AL](/affiliate-disclaimer)>. Early on I noticed the checkbox for "Create local git repository for this project" but gave it little thought. But the more I've learned the more thought I've been giving it and I've started working Git into my normal workflow.

![Xcode Git Option](../Images/xcode-git-option.png)

## Source Control
I'm not new to the idea of source control. In my day-job I use Clearcase on a daily basis. It's cumbersome and has a lot of overhead. But the more I've learned about [Git](http://en.wikipedia.org/wiki/Git_(software)), the more I've seen the difference. Git is a distributed source control tool, which means that any directory can be its own version repository without the need for a central server.

## Why use Source Control
It's common in development to have new ideas you want to try to implement. Often we dive right in and try things out before mapping them out on paper or in UML. More often then not the first attempt isn't the best and could probably be refined once we've learned a few things. Source control allows for us to try those new ideas without corrupting our code base. If the new implementation works than we can accept it. Otherwise we can go back an try again.  

## Git with Xcode
The best part is that Git is integrated with Xcode. It's quick and easy to commit our changes directly through the Xcode interface. You can see changes, manage branches, and merge changes. It's a great practice to get into and so I've started using it while I'm still learning.

## Git Conventions While Learning
- Every time the book says "build and run" I attempt to run. If my changes work I commit them. Otherwise once it's debugged and working I commit.
- Challenges: the books have challenges at the end of most chapters. I recommend doing them. But some of them state that you need to copy the project before attempting.  This is because the book builds on these projects and assumes the challenge has not been completed.  Instead of copying the entire project, I simply create a new branch for each challenge.

## Command Line
Gaining command line functionality of Git is very easy because it was included with your Xcode installation.  Simply add the following line into your .bash_profile.  You probably won't need this for Xcode development, but if you do any development for other platforms this could be useful.

    export PATH=”/Applications/Xcode.app/Contents/Developer/usr/libexec/git-core/”:$PATH

## Resources
The following links I found extremely valuable when starting with Git.  I'm still extremely new to Git and reference these sites regularly.

- [How to Use Git Source Control with Xcode in iOS 6](http://www.raywenderlich.com/13771/how-to-use-git-source-control-with-xcode-in-ios-6): Great overview of how to use Git directly in Xcode
- [Git Immersion](http://gitimmersion.com/): Git Immersion is a great tutorial that walks through all the features of Git.  It's not geared to Xcode, so you'll have to use the command line if you want to follow along.

Let me know if you have any great tip or resources for using Git with Xcode.