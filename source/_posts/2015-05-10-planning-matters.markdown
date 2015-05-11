---
layout: post
title: "Planning Matters"
date: 2015-05-10 18:26:03 -0400
comments: true
categories: 
---
At this point in my Flatiron journey, I am rapidly approaching the deadline for my first presentation and project mode is just around the corner.  Man, I wish it was still week 2!  Anyway, the more I’ve thought about building an app the more I’ve thought about where and how to start, beyond of course, an idea for the app.  Based on the brief research I’ve done, planning the models and database seem to be the place to start.  

One major concept that has come up in Rails lectures is the idea starting with a vertical slice(thanks Steven) and in doing research on the internet, I came across an acronym, MVP which stands for Minimum Viable Product.  From the beginning of Rails, I have been very concerned with the idea of planning before implementing during project mode and have been reluctant to accept how flexible and modular Ruby on Rails is in practice.  Now though, after spending some time reflecting on what we have done so far and researching on my own, I am beginning to develop a sense of how to approach development and planning and I’m ready to take the plunge.
<iframe src="//giphy.com/embed/Y3qPuKds1LgL6?html5=true" width="480" height="159" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

If I’m not mistaken, vertical slicing and MVP are very similar in nature.  Vertical slicing  means to create one model from top to bottom as opposed to trying to build out horizontally an entire collection of models.  This is very similar to MVP in that the theme is to get the app up and running first and then build out the entire scope of the app.  An example of this might be in a generic app getting the user registration finished before trying to build anything else.  I’d start by creating the view, model, and controller and creating the routes and actions to create a user database and then get the routes fully functional in the browser before expanding the app.  It’s useful for me to be aware of this kind of approach as I am the type of person to start out thinking I’m building a simple app only to draw up some crazy collection of tables on a whiteboard and decide to build them all at once.  

<img src="/images/vertical_slice.png">

Planning out associations at this point is also essential.  One critical question I learned from research is:  Is this feature necessary?  This applies to both models and associations.  In getting the app up and running, every model and association should be very intentional and the build process should be methodical.  Using the MVP strategy is especially important when working on a deadline.  Before starting a project, having the specific goal of what the app should do at a minimum allows for more focus on creating the app as opposed debating what to include and being forced to pare down features at  a later point in time.  Like any significant undertaking, I imagine this is much easier said than done.    

<iframe src="//giphy.com/embed/SMZ6QqHuTWxZm?html5=true" width="480" height="270" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

As I started to write the blog post and reflect on process, I am beginning to think perhaps there should be two separate diagrams drawn up in the early stages of an app’s development.  Having two physical diagrams to compare is useful for communication between team members and building consensus about what are the absolutely necessary features to to be added to the app.  

<img src="http://placekitten.com/g/200/300">

It’s all too easy to get caught up in trying to build and do everything.  Having distinct stages allows for more dialogue and shared purpose as the development progresses.  The first, and most important stage is the initial brainstorm/discussion about what the idealized image of the app could be.  At this stage no idea is a bad idea and the discussion can hopefully avoid conversations about what can’t be done.  In other words, think "And" here, not "But."  Also, knowing that there will be a second more focused diagram of the app allows this stage to be about inspiration and vision.  

<img src="http://www.fillmurray.com/g/600/400">

The second stage can then focus on exactly what will be built, what features are absolutely essential, and in what order features will be built into the application.  At this stage the process can be about paring down the app using the principal of MVP to work towards exactly the app will do after initial development.  Focusing on the minimum number of models needed to get the app up and running allows for a more thorough discussion about associations and the order in which models will be built, employing vertical slicing.  Also by separating this stage from the first, the team can now focus on building a consensus about the stages of construction of the app and how tasks will be distributed to team members.

<iframe src="//giphy.com/embed/rOScDjyggnKNy?html5=true" width="480" height="269" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Hopefully, this reflection on planning will help me get off to a more effective start to building an app and that I'm less likely to get stuck even though I'm sure I will at some point.

<iframe src="//giphy.com/embed/IaQssc2zhYaze?html5=true" width="480" height="360" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>         

