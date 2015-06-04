---
layout: post
title: "The Web…What is this !$@%ing Mess?"
date: 2015-05-21 21:24:36 -0400
comments: true
categories: 
---

This past winter, I spent the last week of my Front End Web Dev course with Jon Grover going through a marathon of 7+ hours of video, learning Backbone JS.  I didn’t really understand much of what was going on and was just barely keeping up with the syntax wondering what the point of create, update, and destroy were and how to keep up with all those damn semicolons during the code along exercises. If only I knew then what I know now.  After Wednesday’s lab review, I think I am beginning to put the pieces together. 

First, let’s discuss what is going on between Ruby/Rails on the back end and the web browser/Javascript on the front end.  It’s like juggling  chainsaws keeping track of everything in a Rails app.  Throw in Javascript and jQuery in the browser on the front end and it’s like juggling chainsaws while trying to code along with Steven during a morning lecture!  After the lab review with Steven, I decided it was time to make a diagram of what is going on...

<iframe src="//giphy.com/embed/7jsnB2RRzDGIo?html5=true" width="480" height="259" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Okay, maybe that's not the best description of what's going on, but hey, we're in project mode man.  Alright, all jokes aside, the diagram as promised:

<img src="/images/web_front_back.png">

I think of the server and browser as being two separate containers holding completely unrelated content.  In the middle, is AJAX which functions like a bridge. On the bridge the only possible thing that can cross is a “string” we refer to as JSON.  Even though Javascript is in the acronym, JSON is still just a specifically formatted “string” that can be translated to various programming languages.  AJAX is the channel for passing the JSON through front end events(think mouse clicks) in the browser.

When JSON is passed from the browser to the server, it gets converted in the Rails controller into params that can be read by the Rails action/methods.  Going the other way, the params get converted into Javascript object attributes by Rails through the ‘responds_to’ block.  The one key is to remember the entire time, this information is being passed through in the format of a “string”.

Does that mean creating two sets of objects in models into separate containers?  Yes, yes it does.  I write JS I write Ruby at the same da…

<iframe width="560" height="315" src="https://www.youtube.com/embed/KBb4ZZY2W80" frameborder="0" allowfullscreen></iframe>

They'll probably never read this, but I gotta give a shoutout to my future coders and ALL of my former students from Parkway down in Miramar on the Dade County line.

The database is probably the most important part of a dynamic web app and the database is organized as Ruby objects. Given that the only thing the server and browser containers can share is a simple “string”, both containers need their own objects to keep the app organized.   This dictates how the database will be presented in the browser.   Object oriented Javascript becomes the method for maintaining consistency across the bridge that is AJAX/JSON. 

If the objects get duplicated then the controllers must too.  Controllers with Post/Get internet actions, models/objects for organizing the data, and views for organizing how the data will be presented in HTML have to be created.  One area that I think is confusing is understanding how the erb files work on the internet.  The key to remember is that the browser only uses Javascript so the views must be a composite file of Ruby erb for the database, Javascript/jQuery for the browser, and HTML for markup of the pages.  It gets pretty crazy keeping track of 3 different languages in the file that a person visiting the site experiences as the entire web app! 

THIS, pun intended, can be very confusing.  Given how effective Rails is at abstracting away a lot of the clutter, why not do the same on the front end?  What if I told you…no just kidding.  I won’t go into too much detail in this blog post, but there is NO “what if I told you” in this blog post or in the real world.  I am still figuring all of this out for myself, but nonetheless there are several competing JS frameworks including Backbone, Ember, and Angular that attempt to reconcile the conflicts between Rails and the browser and follow the principles of conventions over configuration and RESTful paths.  When consideing which framework to choose, this comes to mind...

<iframe src="//giphy.com/embed/3GPbOod9GkC5i?html5=true" width="480" height="270" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

...unfortunately there is no clear choice, only corgis...or cats...

<iframe src="//giphy.com/embed/40Fpxgn6Yq640?html5=true" width="480" height="270" frameBorder="0" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>
...and all these frameworks ultimately do the same thing, hence the confusion.

Initially, I thought I’d stumbled onto the holy grail when I went back and reviewed my Backbone labs, but then I went back to my chart and realized there was a problem.  There is  only one view shared by both Rails and the browser!  There is no way to create separate views that detach the Ruby from the Javascript.  To say it succinctly, there is only one browser window and it is written in Javascript.  After doing further research on the internet about these frameworks, the whole situation becomes a lot more complicated.  There is no magical “what if I told you” moment for reconciling the conflicts between Rails and Javascript in the views, only lines on lines on lines of code...or racks...

<iframe width="560" height="315" src="https://www.youtube.com/embed/IcXxXz0XPt8" frameborder="0" allowfullscreen></iframe>

RACK UP!!

There is only a range of options with various strengths and weaknesses based on need and personal preference.   I am beginning to see why at Flatiron we have not received a clear answer to our questions about which JS front end framework to use with Rails or if we even should use a JS framework with Rails.  In addition, I am also beginning to see why some developers just turn to Node and create an entire full stack JS web app.  Finally, I think I understand why Steven is so excited about Volt as it appears to abstract away JS entirely, letting Ruby covert to JS, a layer below the coding, while maintaining the consistency and elegance of Ruby on Rails.

Till next time when I break down the choices on the front end, in honor of the end of labs and green lights, and it being Friday, I leave you with…

<iframe width="560" height="315" src="https://www.youtube.com/embed/o-AbEO6J8s0" frameborder="0" allowfullscreen></iframe>

Peace out we in project mode!

Octocats Rule!









