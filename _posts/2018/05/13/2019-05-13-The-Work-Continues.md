---
layout: post
title: The Work Continues
subtitle: As it should
author: Jamie Higgins
date: 2018-05-13
categories: Personal
image: /img/post/2018/05/13/banner.jpg
---

> Since Monday is a Bank Holiday in Ireland, we didn’t have work, so this week starts from Tuesday instead.

### Tuesday

It was really a slow start to the day, I was just following up on tickets from last week that the customer still hasn’t responded to yet. Other than that, I started using the Dynamics Learning Portal (DLP) to research what goes into making sure that an instance of Dynamics is fully compatible with mobile, such as offline records and customising views to make sure that they also look good on mobile. We got our headshots that we took last Thursday today, so I went and updated my company email and LinkedIn with it. Only problem is that I don’t have glasses on in it, only because of the glare, but it’ll do.

Going back to that ticket last week with the JavaScript file that needed updating, I was too focused on updating the JavaScript that I forgot to also update the view on the live instance, oops. One quick update later and the ticket is complete, nice.

There was also a ticket I got where both the live and the dev portals for a customer would throw a Null Object Reference exception on login. I went into the PC that hosts the websites and ran `iisreset` and that seemed to do it? I honestly don’t know if that was the fix, but it is working now, so that’s good enough for me.

### Wednesday

Gotta love it when errors come back in full force and they're worse than before.

The portal from the last ticket went down again, and this time running `iisrest` didn't fix it as I couldn't even log into the CRM to test out some settings. What it came down to was that the main account that is used to connect the CRM to the machine hosting the portals' password was changed and the error was occurring because it couldn't make a connection. So we had to get the new password from the customers and input it into the Application Settings of the IIS Settings. Problem solved.

The same customer then told me that I could close 2 of the tickets that were left open as I was waiting for him to test somethings out. Not my problem now I guess ¯\\\_(ツ)_/¯.

Then the real fun began. Another customer syncs their data between Dynamics CRM and Dynamics GP using Scribe, and this can cause some problems sometimes when data just refuses to sync properly. Today was one of those days. And since this is my first time having a ticket like this, of course I have no idea how to properly fix it. So it was a lot of going back and forth with one of my colleagues since he has a better understanding of the whole process of resolving the issue. I ended up having to log a case with Scribe and I did get a response, but I was too busy to get back to it. Tomorrow it is!

I was busy working on a ticket that was actually the first one that I received, where there were a bunch of small changes that needed to be made to make the CRM better on the Windows 10 app. Still going... but which way...

### Thursday

Alright, today wasn't all that interesting, only because I was working on 2 tickets for most of the day. Going back to the ticket involving syncing to GP being broken, it still is. I now have my manager and the customer asking me why it isn't fixed yet, and it's because I'm waiting for Scribe Support to get back to me. I reviewed what's there currently with a colleague who is more familiar with the system to see if there is anything we can do for the time being, but even he's stumped as it's a weird variation on an error that is somewhat common with this system. Not a lot I can do with this now, even though it's Priority 1 :/.

The other ticket I was working on was one where there is a problem with the system where when an email comes into a mailbox, it gets assigned to the wrong people. I spent a decent amount of time trying to see if there is anything that could help; the auto case creation, workflows, plugins, various other processes, nothing. It was only right at the end of the day that Joe decided to have a look at the roles of the users who are supposed to get the cases and the person who is currently getting them and there is a role that looks like it is the culprit. Why it's synced up on user role, who knows. I've emailed the customer about it so now we'll wait and see what happens.

Other than that, I got another ticket about the storage limit of one system, but since Joe has a ticket dealing with mass deletion, and that this is now the second ticket I've gotten relating to this issue, I'm just going to ignore it. My manager will be back tomorrow, so she'll sort it out then.

Told you it wasn't that long of a day.

### Friday

Today's post could just be that the data is now syncing between Dynamics and GP again and I'd be happy with just that.

Ok, I should explain. I didn't do a huge amount to resolve the issue, but I had a guess that we could reset the password for the account and change the settings for Scribe to reflect this, and that seemed to do it. However, I didn't change the password or the connection to Scribe since I didn't have all the privilages to do so, but we got someone else who did to do it and everything is good now, happy Christmas to me!

Only other thing that happened was that we did some work on the plugin where some records were updating at the wrong stages of the system. There's still a bit of work that needs to be done with it though as it throws an error for the time being.

Until next time,

--Jamie