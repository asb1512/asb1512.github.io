---
layout: post
title:      "Market Watch CLI"
date:       2020-07-02 15:02:29 +0000
permalink:  market_watch_cli
---


For the CLI Data Gem Project, I have chosen to go with the API route over scraping.

I was able to find a public API called [Alpha Vantage](https://www.alphavantage.co/) that delivers up-to-date* market data through different API endpoints.

I felt that learning the basics of interacting with APIs is an essential skill in my line of work, since I'll be dealing with a lot of databases, as well as web-related functions.

This project has been one of my most difficult undertakings since starting at the Flatiron School. Throughout all the labs up to this point, we've been able to lean on the 'Ask a Question' feature that can give you the hint you need when you've exhausted all your options. But this time, it's more real. You're on your own and you're forced to use the same resources as any other developer. Google. It's really powerful and can answer your questions faster than most people could.

This process has also shown me the importance of test-driven-development; and that however laborious it may feel to plan, even when you just want to get started, it's extrememly important in making a clean, functioning program.

I divided my program into four main classes: the CLI class, a Display class, an AlphaVantage class, and a Date class.
- The bin file instantiates a new instance of the CLI class which prompts the user for input, deals with the general framework of the application, and general user input.
- In an effort to keep the application DRY, the Display class deals with the aspects of the program that change based on which data the user desires to see.
- The AlphaVantage class is what actually sends a get request to the API and formats the slug to the appropriate endpoint.
- The Date class, which is an internal class of Ruby, was needed to allow this CLI the ability to check not only the date, but the current and yesterday's day-of-the-week.

After watching the 'Daily Deal CLI' walkthrough example, I tried to emulate the instructor's idea of programming the CLI first, hard-coding what you want the program to do without getting tied up with the specifics of how that would actually happen. After the basic set up, I began to deal with the API itself and how the URL and its slug change the data that is returned. Once this was figured out, I began work on the Display class. This class takes a JSON hash that is returned and parses it into something digestable by the user. This section was probably the most difficult, as the data returned very long and included many levels of nesting.

Overall, the CLI is still rough around the edges, but I feel much more confident in my abilities after having creating a real program that actually works!

This project hasn't dulled my interest in programming whatsoever; in fact, it has done the exact opposite and makes my very eager to dig in deeper and tackle the next challenge that lies ahead.

Happy coding!






















*Unfortunately, you cannot request data from the current day until the market has closed at 4:00pm EST.
