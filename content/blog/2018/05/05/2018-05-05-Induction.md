---
title: Induction 
subtitle: I choose you!
author: Jamie Higgins
date: 2018-05-05
---

### Monday

Started off the week with a ticket from last week whereby a person wasn't able to finish a business process flow and it came down to them not having the System Administrator that they had in the development instance, so not hard to fix.

At this stage, we had a meeting with one other developer in Dublin and the main customer where there was a problem with the logic of one of the processes that needed to be fixed, so we needed to have this meeting to sort out what the logic is supposed to do. I wasn't sure what work the developer had done so far with the dev instance, so I emailed him to see what he had worked on, so I wasn't treading over ground that was already done.

Most of the rest of the day wasn't full of anything important; I started looking into Resco Inspections for a project that I'll be working on at some stage with Joe during this work placement. But other than that, yeah, quiet day

### Tuesday

I knew I had a ticket that was due today that was in relation to unblocking IP addresses, the one where I kept getting locked out because I kept messing up the password? Yeah, that one. Turns out, after talking to the other people around me, it looks like it's not really an issue that we're supposed to be working on and it's more so for their internal IT team. So that ended that one, I just marked it as "Waiting Customer" just in case the person sends another email.

There's also been this ticket that's been kicking around the office since the start of last month where one user (Who has the full System Administrator role) is not able to see parts of the system, specifically, the notes that they must make when they are out on a call. I'll be honest, I really don't know what is causing the issue, but my best guess is it's their machine or internet connection, since I can't seem to recreate the issue on my end, with a user with the same roles as them.

We were introduced to a new user at this stage, though we don't have any ticket for them yet. Their system is a little funky to edit, since you first have to open TeamViewer and then use RDP on that machine. I mean, sure. The actual system itself is only for logging customer cases and for mailboxes, so there's not a huge amount within it.

And then, the last 20 minutes hit. Oh my, the last 20 minutes hit.

I got about 3 replies to tickets that I've had sitting there since Friday all at once, as I'm preparing to leave. I've had a pretty quiet day again, with about 4 hours or so of not a lot going on and then this happens. I had 2 replies from one customer in which we responded to the wrong tickets, so I had to get him to clarify and another where a person got back with some more changes that they need done to the system. I more or less just responded to them and just left it at that. Look at this way, I now have something to do tomorrow.

### Wednesday

Whoa, what a day.

First ticket of the day, I had to figure out why some records weren’t being synced with Dynamics NAV. They were manually forced into NAV, but why weren’t they there by default. Until I realised that the records in question were forced into a stage that they weren’t supposed to be in yet, meaning that the system couldn’t validate the data properly. Ok, that’s fine, but how did the user get past the validation that is there to prevent any of this happening? These are the questions of a generation.

We also had a call with one of the customers in relation to the slow performance of Dynamics on their devices. He was trying to show us that it would take upwards of 6 minutes to sync any records, but as he did, it loaded about as fast as it does on our machines. It just looks like the issue is connectivity and considering that most of the people who work with this company are farmers with little to no internet most of the time, this would make sense. Only thing we could offer is a change request where we’ll try and implement better support for offline content on their devices, but we’ll discuss that on Wednesday with him over another call.

Considering tomorrow is the induction with the company, we travelled up to Dublin by train and stayed in Liam and Ciara’s house, which is the same place we’ll be staying in when we’re up in Dublin in 2 months’ time. It’s small, but more than enough when we’re there.

### Thursday

Fun day was had by all. The day started off with trying to sort out breakfast for myself and Joe. Went walking around of a while and found one place on Google Maps, but upon realising it was on the 5th floor of a building, I thought it would probably be too expensive, so back down the stairs I marched, but not before snapping a picture of this poster

![Poster of bugs with profanities below each insect](/assets/img/post/2018/05/05/Image_1.jpg)

So I got lost on the way to the next place, but ended up in a breakfast bar anyway and got a breakfast sandwich, so that worked out well.

At which point, the real meat of the day begins… talks delivered from the higher-ups in the company, though they were actually interesting, going over the history of the company, what types of customers they tend to deal with, etc.. After all of that, we went to lunch with the rest of the new employees (There was about 21 of us in total) that was payed for by the company, which was pretty tasty (both the lunch and the fact that it was payed for). We didn’t really get to go around Dublin past that, since our train was so close at this stage, so back to Galway we went. And crash on the day I did.

### Friday

Most of today was spent working on one ticket, but there were some weird bugs with it that made it go on longer than I anticipated it would.

Update a chart to display more info; easy enough.

Update a form to add more fields to a lookup fields; Hmm…

Ok, I can explain though, there’s a JavaScript file that goes with the form that makes certain fields available based on the selection made in a lookup field. All I had to do was add 2 more options to this list and add them to this file, expect that the file validates based off value, instead of ID.

So here’s me, looking at this file seeing if I can get it working with the field value, just to be consistent with what was already there, and then just giving up and using ID instead since I knew that would work 100% of the time. At this point, the customer is satisfied with the work, but they can’t test it until Tuesday. Great, guess we’ll wait until then to see if I did it right.

All in all, fun if busy week with lots to do and going to Dublin was a nice little mid-week break, somewhat, it’s still work related.

Until next week,

--Jamie