---
layout: post
title: "Software Development"
date: 2014-06-16 08:32:45 +0530
comments: true
categories: Development Process
---

In my new organization, I'm actually beginning to understand the various flavours of developing software and have learnt one thing - It isn't as easy as it looks to the outside world. There are tons of procedures, processes and responsibilities to look after before the stable product code lies in the hands of the end user. Let me begin to see what goes where.

Say you have a product. Assume you also have a customer in hand. The customer wants a basic flavour of your product to work accroding to it's expectations. That's when you decide to roll out software to him/her. You now tend to phase out various levels of that product so that it doesn't break in the event of the customr's daily interactions with the product - on any level of intensity, load or any other factor.

You first begin to work on the core features of the product on your own system and build up your own **local** environment. If the product involves a client-server architecture, you ensure all of the components works in your local system first with 127.0.0.1 as your server IP. You write code, attach testcase to them, check if every process of the product works intact with the testcases.  You also load the database locally, test the product with the database and document the procedure. All of this involves just you, nobody else, at the moment. Then, the components begin to split away from themselves, leading to a distributed architecture. More and more people now begin to do the thing that you're doing but all need to be synchronized with data. The database is usually the first part to be installed as a core, distributed entity. All local instances begin to access data corresponding to their won databases from a single point of contact. The load reduces on your local system and thus, you thus have now set up the first local instance of the process.

After the local instance works, you then freeze your code to a version control system - you tend to submit your code for your peers to test them with their own testcases to delve with. We need an independently running setup of your product somewhere to test this within the organization for all testers to act upon the single system. Thus, enters the build stage of the process, a crucial component which integrates your code with the product and compiles all of the components on a timely basis for synchronization. Testers act on this setup for the reported features/bugs. Thus, the second stage of the process - **local site** setup is crucial for local changes. Build is run separately for this.

Now that all your code is been tested and is agreed upon, this will be now moved to the third stage - the developmental stage. The customer sees that the features are now being tested as part of the developmental process. I'm a bit hazy on this topic as this is where developers are detached from the system and it is only development team's QA on the customer side take up further testing and keep on releasing bugs/patches to be fixed. They can either be residing in your organization or in the customer's place. Build is run separately.

The fourth stage is where the actual users come into play - the user acceptance testing phase. A certain belt of your product's users are picked who test it thoroughly as per the customer's requests and keep reporting for any issues. The customer is convinced only in this stage where he gets a real snapshot of the ongoing process of delivery of the requirements. UAT build is again, separate.

Lastly, once everybody agrees that the code works successfully, the final build is run which thus, releases the product into the production stage - the real field area of usage. All users of the product use it, benefit from it and in turn, help the customer make money.

Certain things get redundant as the code stage begins to rise stagewise. Developers lose role after dev stage, software delivering agent loses role after UAT and customer after production stage. So, if you see that you report a bug/issue in the software and it gets recorded, be patient to see it get fixed according to a timeline. The way the problem is tracked and fixed takes longer so as to not impact the stability, reliaability and value. 