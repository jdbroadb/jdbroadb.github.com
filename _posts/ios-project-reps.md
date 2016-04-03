%% Title: iOS Project: Reps
%% Date: 2014-05-12 08:32 PM
%% Type: Blog
%% Slug: ios-project-reps
%% Series: Reps

I [recently decided](/2014/05/07/starting-projects/) that I wanted to complete two projects to ramp myself up on both app and web development. I've been coming up with app ideas for the last 4.5 years and so I've really struggled with what iOS app I want to create. I want to make sure it's limited in scope but useful to me (and hopefully others). I've decided to steer away from an app that involved web services but want to be able to incorporate a lot of Apple frameworks and software methodologies.

## Reps

Based on the above criteria, I've decided on developing a workout log app which I've tentatively named **Reps**. I've done some searching and haven't found a good, general purpose workout log that doesn't have one of the following issues:

* Bloat of exercise instructions that I don't need
* Upselling to annual subscriptions that I don't want
* An unintuitive interface during workouts
* Deep integration with social platforms such as Twitter or Facebook

Not all apps I've found have all these problems but I haven't found one yet with none. I'm sure if I kept searching I might find something but it seemed like a good option for my project.

## App Scope
It's important to define the app scope early to stay focused, avoid feature creap, and not get distracted. Here is a list of the items I'd like my app to address.

* **No instructions** - I know my exercises, I just need to keep track of what I've done
* **Tagging** - as of now my plan is to use general purpose tagging instead of built in categories for organizing exercises and workout routines
* **Quick Start** - I want to be into a new or saved routine as quickly as possible from launch
* **In-App Metrics** - I'd like to have access to basic metrics through the app. Candidates for future releases would be advanced metrics, graphing, and exporting
* **Minimal Setting** - I don't want a lot of settings at first, it's ok for the app to be opinionated to meet my needs

From this list I've developed the following [App Definition Statement](https://developer.apple.com/library/ios/documentation/userexperience/conceptual/mobilehig/Process.html):

>Reps is a workout log for people who know their exercises but want to vary their routines and track their progress.

This may evolve over time but I think it's a good start.

## Development Scope
I also want to set some ambitions for technologies and methodologies I'd like to use and learn about. This will help me maximize the value achieved from the project.

* **Source Control** - all code will be controlled through Git and will be stored in [Bitbucket](https://bitbucket.org)
* **Unit Tests** - I will strive to write unit tests and take advantage of the updates in Xcode 5
* **Minimize Custom UI** - I'd like to use the stock UIKit unless it will truly enhance the app experience
* **Core Data** - I've played with Core Data in some if my projects and I think it suits this app well
* **Interface Builder** - I've played around with IB but haven't embraced it to date
* **Auto-Layout** - I've also used some auto-layout but I plan to use it as much as possible
* **Animation** - I definitely want to use animations and take advantage of some of the view controller transitions in iOS 7
* **CocoaPods** - I won't use any open source project unless it really makes sense but if I do I'll use CocoaPods
* **Document Design** - since I do this part time it's important to maximize my efficiency when I'm in front of the computer. To aide that I'll plan and document the design as best I can with my other free time away from the computer. (Hopefully most of that content will make its way here)

I think I have a pretty clear picture of the desired product and a lot of good goals for the development process. As always I'm sure they'll evolve and change over time but they will help me maintain focus and will be fun to reflect on *when* the app ships.
