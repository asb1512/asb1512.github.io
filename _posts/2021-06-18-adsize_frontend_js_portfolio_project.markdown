---
layout: post
title:      "AdSize: Frontend JS Portfolio Project"
date:       2021-06-18 21:03:04 +0000
permalink:  adsize_frontend_js_portfolio_project
---


For my Frontend JS Project, I chose to make a platform called **AdSize**, where designers and advertising professionals can access ad-dimensions for popular ad platforms in one, consolidated platform.

Part of the inspiration came from my own experiences in graphic design. You are often asked to make an ad set for a specific client on a specific platform (i.e. Facebook, Google, Yahoo, etc.) and if you don't know them all by-heart, then you'll have to do some searching on Google to find the official sizes and options.

When using AdSize, a user visits the site and is prompted to 'select a platform'. Using AJAX, the Rails 6 backend is sent a GET request for all the of the ad platforms available. Once the user has picked a platform, all of its possible ad dimensions appear on screen; rendered true to their size (a 1200x628 FB banner ad is rendered with a width of 1200 pixels and a height of 628 pixels). When viewing on mobile or tablet, the sizing will need to be altered and scaled to keep dimensions from distorting.

The user can use their email to login and have access to a to-do list for whatever they wish. Items can be created and deleted at will. The list can be hidden for easier viewing.

While working on this project, I have become much more comfortable with JS and its syntax, but when completing tasks specifically related to DOM manipulation, vanilla JS quickly shows some its weaknesses. This is where frameworks come in, encapsulating some of the repetition into reusable blocks of code.

For the creative process, I decided to go with the recommendation from Flatiron curriculum. This is the idea of taking one piece of the application and setting up all the relevant parts needed to get it working, instead of attempting to set up the entire pieces at once (i.e. setting up only the backend). For example, I chose to start with the Platform model.

After creating the Rails app and file structure, I started by making the model and its migration. Once that was working, I created a serializer class with the help of a great gem called 'Active Model Serializers' and made the JSON response was formatted correctly. I then went into the frontend and made sure I could call the endpoint and receive the data I was looking for. The received data is collected and used to create new instances of the Platform class for the DOM. I repeated this process for all parts of the project.

By the end of this project, I am more excited than ever to learn more of what JavaScript and its frameworks have to offer to create beautiful and interactive web applications.


