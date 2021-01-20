---
layout: post
title:      "Autolog – Sinatra Web App"
date:       2021-01-20 05:23:56 +0000
permalink:  autolog_sinatra_web_app
---


In the Flatiron curriculum, I view this project as a major milestone in my journey to becoming a full-stack web developer. This is the first time I have had the pleasure of see a functioning website that I built! Not to say that all the lessons and the CLI project leading up to this were not fun and challenging; they were the building blocks that I most certainly need, but it can be difficult to see the 'big picture' when starting out. I'm proud to say that I'm finally catching my first glimpses of that 'big picture'.

Since a very young age, I have always been fond of cars, motorcycles, and anything else that moves under its own power and that is why I chose to create a Sinatra CRUD application that would allow the user to keep track of their vehicles and their associated repairs. Sometimes, keeping track of service records and other pertinent information can be cumbersome and often requires filing away documents and receipts. Autolog puts all of that data in one place that is accessible from virtually any device with an internet connection.

Obviously there is quite a bit more additional functionality that would greatly improve the user experience; and in the future I hope to do just that, but at the moment, my skill level does not match that of my aspirations. Features such as push notifications for repair reminders, uploading images, etc. are things that come to mind.

Regarding the process of developing this project, I started with the help of a really cool gem, Corneal. This provides the scaffolding for a Sinatra application and makes getting started much more seamless. I cross-referenced quite a few labs from the Sinatra unit to help things like the `config/environment.rb` and `config.ru` files get up and running.

After this, I pushed my local repository up to GitHub and created a secondary branch for development. In the future, it would be cool to do a refactor, clean up the code, and add helpful comments on a master branch.

At the beginning of my Flatiron journey, the importance of version control and Git was completely lost on me, and I just accepted it as something important to be understood at a later date and moved on. Even for my CLI project, I found myself staging changes, making commits, and pushing them without really understanding their use or purpose. However, this project has truly opened my eyes to the awesome potential and power of Git. That is something I never thought I would be able to say.

I decided to develop Autolog by starting with the backend and then moving frontward. I sketched out my model relationships on a notepad first to help visualize how I would set up my database. Once that was settled, I began to created the models: `User`, `Vehicle`, and `Entry`. Luckily, the table relationships were not too difficult and ended up as follows: A `User` has many `Vehicles` and a `Vehicle` has many `Entries`.

Once that was worked out, I began creating my `UsersController` and all the necessary routes in order for a user to sign up and login/logout.

After authentication was solved, I began to work on building out all the necessary CRUD routes and views for the three models. This was by far the most lengthy and time-consuming part of this project.

Finally, came the frontend aspect where I styled my site using CSS. This project has shown me that CSS is not a 'wannabe' programming language by any means, but instead has all the intricacies found in any other respected programming language and requires dedication for mastery. The possiblities are endless and I love that.

Overall, I have found this project to be very rewarding and has given me a taste of what web development is truly like. It makes me look forward to Rails and its potential even more and has solidified my resolve to become a full-stack web developer.

