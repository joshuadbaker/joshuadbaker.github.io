---
layout: post
title: "AJAX Forms"
date: 2015-06-04 08:43:13 -0400
comments: true
categories: 
---

AJAX.  I’ve been thinking a lot about AJAX recently, trying to relate new discoveries in Rails back to my introduction to Backbone.js and more recently, the excellent tech talk about Ember.  

The whole idea of calling a server and loading webpages repeatedly, feels so…2005.  It seems so much cleaner and more professional to make one request to a server to load the entire page and be done.  Pages have become incredibly complex and so much can happen on just one section of a page let alone the entire page.  Not to mention, mobile use is revolutionizing the entire concept of what our web experience is and the last thing we want as web developers is to limit our mobile users’ experiences.  In addition,  with what is already being done with WebGL and the canvas element in HTML5, I simply can’t imagine how much our web experience will change in the next 5 years.  Given this paradigm, it is absolutely imperative I embrace AJAX and all the possibilities it can provide for a more efficient and joyful web experience.  I have to face the facts, the web is getting more sophisticated, elegant, and abstracted.

First, too quickly review, AJAX provides a channel for passing back and forth data from a web server without having to make additional calls to the server to reload the entire page.  Below is the chart I presented from my last post that provides a visual explanation of AJAX.  

<img src="/images/web_front_back.png">

Rails of course already integrates the use of AJAX into its framework and it is quite effective, especially in how it handles forms.  Without AJAX, if a form is filled out and the submit button is pressed, and event is fired off and a Post call is made to server which refreshes the entire page.  AJAX sends the information without refreshing the page.  In my case, for practice, I created a simple, very simple Rails app to try and get a form working in this new format.  Here is my controller:

<img src="/images/controller.png">

In this form I tried a variation on the responds_to method placing it at the top of the controller so it affects each action. 

Next, I created an html.erb file that holds the mark up language for the page.  This page is pretty straight forward and holds the references for the JQuery. 

<img src="/images/htmlerb.png">

Next I created the js.erb files that integrate ruby/rails into js files to manipulate the forms on the page with toggle methods.  

<img src="/images/newjserb.png">

<img src="/images/createjserb.png">

These files are where the action takes place.  I feel like the js.erb file is where I need to spend more time learning how ruby integrates into javascript.

Though I’ve tried to change and move different elements around I’m still not able to get the form to appear.  I’m really excited to figure this out though because integrating a Rails backend into an AJAX controlled front end will make for a dynamic and more sophisticated web site. 
   
One of my goals for my group’s project is to integrate some AJAX functionality into our web app to make it more efficient and user friendly.  I decided to experiment with some hidden forms after reading about them online.  The hidden forms are AJAX forms that display on a toggle
