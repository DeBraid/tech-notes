# Fabergésss 

Fabergésss (FAB-ROH-JAY-ES) is a funky way to describe the javascript ecosystem.  Lots of new tools, rapid pace of change, fragmentation of leadership and mass developer exhaustion.  

Google search 'javascript fatigue'.  There is a clear frustration on part of developers getting slammed by the paradox of choice.

Love Meteor, torn by their choices for v1.3+...

Meteor <1.0 created a wonderful developer experience.  The `meteor` CLI was simple and effective, the Atmosphere package ecosystem made package management, building and deploying easy.

From Discover Meteor author [Sacha Grief](https://www.discovermeteor.com/blog/the-state-of-meteor-part-1-what-went-wrong/): 

> Many [Meteor] community members [want] a real framework. One that would make choices for you, and give you easy blueprints to quickly build apps. In other words, not just a few two-by-fours, but an actual IKEA kit.

Humans crave structure and discipline.  We're all just big kids. 

And then 1.3 happened, with such massive shifts that it should be 2.0... 

With a move towards the way 'most people in the JS ecosystem are building apps' (slamming their faces against the wall with shitty undocumented tools). We love ES6, but the `import`/`export` pattern (from a new, dedicated `imports` folder) is un-Meteor, a Meteor Dark Pattern.

A Meteor Dark Pattern (MDP) is something that favors scale over simplicity. MDG has sided with MDPs, destroying their main selling point: positive developer experience. 

They are VERY smart people at MDG.  They have numerous valid reasons for choosing Fabergésss over Meteor 1.0.  My assumption is that Meteor 1.0 as it was engineering did not work at scale, therefore monetization would be difficult.  

In order to provide RoI, MDG is offering hosting services.  A great many small websites is less economical for them than dozens of very large apps. Hell AWS is an amazing business, I'd like to get a piece of that action too!

I do not begrudge MDG for taking this path, but I'm sad that their Motivation was money, which I wholly support and endorse!  

Open source is HARD, and Meteor was/is providing value to developers.  They should get paid for their contribution to app development ecosystem. 

      ie.  Atmosphere packages were magic, they just worked.


  It was perfect for starting out and smaller apps, so why exactly adopt the 'best practices' from broader JS ecosystem? 


  Best the attractiveness was ease of use.  When ease of use is a founding principle, 1.3 is a dark pattern. So anything 

What if?

What if instead they offered a non-mongodb backend sooner? If 1.0 launched with mongo and Postgres how would things be different? 

Comment from [Meteor thread](https://www.discovermeteor.com/blog/the-state-of-meteor-part-1-what-went-wrong/#comment-2470340694): 

> Lego brick development is the holy grail of programming and Meteor has that in smart packages. Getting sidetracked by the latest JS flavor of the month (Angular, React, etc) at the expense of the smart package scheme will be the death of the framework. 

Another [comment](https://www.discovermeteor.com/blog/the-state-of-meteor-part-2-what-happens-next/) from state of meteor thread: 

> As a seasoned developer (15 years building web apps) I liked Meteor (and Blaze really) because it made all those decisions for me, and then got out of the way. I could cobble together my own stack, and I've done that, but what happens is I end up spending too much of my mental energy on that problem, and less on the business needs of whatever I'm building. What I love about Meteor is that even if I don't need real time data access (DDP), or even if MongoDB doesn't scale well, I spend more of my time thinking about how to solve business problems. 