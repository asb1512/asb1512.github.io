---
layout: post
title:      "Lingua Franca: A Rails Porfolio Project"
date:       2021-04-12 20:37:39 +0000
permalink:  lingua_franca_a_rails_porfolio_project
---


After completing my Sinatra project and moving on to Rails, I began to see why people fall in love with it. 'Convention over configuration', an adage often repeated in the Rails ecosystem, began to become more clear as I have learned more and more about the framework and its benefits.

For my project, I chose to try and replicate a website that is near and dear to my heart. As an avid language learner, I realized quickly that the biggest missing piece to mastery is often the lack of speaking and time spent practicing the language in a natural, conversational way. Luckily, I stumbled upon a site, https://www.language-exchanges.org/, that allowed me to pair up with native speakers and practice; all for free!

I have titled my Rails App as Lingua Franca, after the common language that is used when two parties do not share a language. In my app, a user visits the site and can choose to register through the site or through an already existing GitHub account. Once users have input some pertinent information about themselves, including their native languages, languages being learned, and a profile picture, they can begin to find users to speak and improve with. The user is able to send friend requests to other users, who can in turn view their profiles and skype usernames. This site is meant to serve as a middleman or matchmaker. There are already plenty of competent platforms for video/audio calls, such as Skype, Zoom, Google meetings, and so on.

While the app idea in concept sounds fairly simple, I quickly realized in the planning phase that sending friend requests and displaying relevant users (in regards to one user's native language and their foreign languages, and vice versa) was no easy task for someone new to Rails.

Mapping out the database and model relationships proved to be quite complicated and I ended up with nine total tables in the database, three of which are related to Active Storage, allowing for the storage of images. There is a User model which has many invitations, and has many languages through language users. Languages have and belong to many Flags through a `flags_languages` join table. I felt the need to distinguish flags (countries) from languages due to the fact that a language is often spoken in more than one country and can vary widely based on the culture of said country (i.e. English in the US, the UK, Australia, Ireland, etc.) and this allows a user to visit a flag show page and see all the countries in which the language is spoken, or vice versa to see a country and the languages that are spoken there, which can also vary quite a bit.

Connecting users to the languages they speak is a languages_users table with a boolean `:foreign_language` that is set upon account creation and can be changed later on, if desired. This is important because I did not want each user to have their own array of languages that they speak and are learning, which would lead to needless repetition in the database. Instead, the user and languages are related without changing the user or language records themselves.

Once this was all settled, I finally set out setting up and creating a bare Rails 6 application. I then set up migrations and models, working from the backend frontward with routes, then controllers, and finally views.

For the frontend, I went with Bootstrap 4 after having diffuculties getting Bulma to function properly with Rails 6, which turned out to be a great choice! The wealth of documentation and online support have proven invaluable in getting the app up and running.

I always appreciate and enjoy the portfolio projects, not only for the sake of applying what you have learned, but because you end up learning so much more in the process. Whether it be Stack Overflow, the Rails documentation, YouTube, Medium, etc., you begin to have a much more thorough understanding of Rails and how it relates to the Internet as a whole, all while hearing this from actual developers who are in the industry.

I look forward to the next project and the next big step in my journey to become a full-stack web developer!
