---
layout: post
title:      "The WRONG Way to Store Passwords"
date:       2020-06-04 00:48:30 +0000
permalink:  the_wrong_way_to_store_passwords
---


As budding web developers, just getting to the point where you can code even the most modest of websites can often seem like an insurmountable task. But as we grow and learn, and real, operational websites begin to seem more and more possible, I've found myself asking: what about user authentication? How does it work? Where are usernames and passwords stored? How could I keep them safe?

The world we live in is a world of security breaches, leaks, whistleblowers, and the rest, and the security of your users' information is more important now than ever before.

You might be shocked to know that many of your favorite websites store user information in plain text. This means that your email `johndoe@gmail.com` and your password `P@ssw0rd123` are sitting in the database just the way you typed them. If there is ever a security breach and someone finds a 'backdoor' into your database, then no further work is required to steal hundreds, thousands, or even millions of users' sensitive information.

**How can you as the developer protect against this?**
One of the first options you have is encryption. A basic form of encryption takes the user's password and uses a key, then encrypts it. This means that if someone did have access to the data, at the very least, user information couldn't be read right away. However, any compotent hacker would know this, and in turn, take both the user info, as well as the key. In addition, if your site is big enough, you're bound to have users that have the same passwords, and despite the encryption, someone could discern passwords through their frequency.

A unfortunate example of this occurred with Adobe. An industry leader with millions of users fell victim to a database breach and millions of user passwords were leaked onto the web (including mine! If you want to see if your info has been breached, visit this very handy site https://haveibeenpwned.com/). If it could happen to a giant like Adobe, it could happen to you.

One of your next options is *hashing*. Hashing uses an algorithm that alters the password into something unrecognizable. Unfornately, hashing suffers from many of the same pitfalls as encryption. In addition to this lack of uniqueness for users who share the same password, if you were to use one of the most common hashing algorithms, such as MD5 or SHA1, many of these can be cracked by simply typing them into Google! To get around this, a proceduring know as '*salting*' has been created. Salt is a random string of characters that is different for each user that is added into the hashing algorithm. This allows two users with the same password to still have different data that is stored; and due to their length, many common attacks, including brute force are no longer feasible.


And finally, the best and possibly the easiest way is to use things like 'Sign In with Google, Facebook, etc. This allows you to leverage the security solutions that they've already implemented and perfected over the years, not to mention the vast amounts of capital available to them.

The moral of the story here is **security matters**. In our increasingly tech-based society, your users will appreciate that you went the extra mile in protecting their personal information.




Source
https://www.youtube.com/watch?v=8ZtInClXe1Q


