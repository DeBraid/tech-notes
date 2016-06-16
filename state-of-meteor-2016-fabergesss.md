# Fabergésss 

Fabergésss (FAB-ROH-JAY-ES) is a funky way to describe the javascript ecosystem.  Lots of new tools, rapid pace of change, fragmentation of leadership and mass developer exhaustion.  

![](http://i.giphy.com/8TNHNwBEhhc4g.gif)

Google search 'javascript fatigue'.  There is a clear frustration on part of developers getting slammed by the paradox of choice.

## Meteor 

Love Meteor, torn by their choices for v1.3+...

Meteor <1.0 created a wonderful developer experience, its was one of their core values.  The `meteor` CLI was simple and effective, the Atmosphere package ecosystem made package management, building and deploying easy.

Books were written, like Discover Meteor.  Atmosphere packaged were developed.  Deploys were easy and free. Then the biz dev people took over and the changes that ensued following Meteor 1.0 launch were dramatic.  

Frustration abounds. Author [Sacha Grief](https://www.discovermeteor.com/blog/the-state-of-meteor-part-1-what-went-wrong/) wrote a popular post on the State of Meteor: 

> Many [Meteor] community members [want] a real framework. One that would make choices for you, and give you easy blueprints to quickly build apps. In other words, not just a few two-by-fours, but an actual IKEA kit.

Humans crave structure and discipline.  We're all just big kids.  Meteor 1.0 provided that. And then 1.3 happened, with such massive shifts that it should be 2.0... 

## The New Meteor

With a move towards the way 'most people in the JS ecosystem are building apps' (slamming their faces against the wall with shitty undocumented tools). We love ES6, but the `import`/`export` pattern (from a new, dedicated `imports` folder) is un-Meteor, a Meteor Dark Pattern.

A Meteor Dark Pattern (MDP) is something that favors scale over simplicity. MDG has sided with MDPs, destroying their main selling point: **positive developer experience**. 

### MDG

They are VERY smart people at MDG and did a wonderful job in bringing the best JS framework to market over the past 3-4 years.  

They have numerous valid reasons for choosing Fabergésss over Meteor 1.0.  My learned assumption is that Meteor 1.0 as it was engineering did not work at scale -- something their largest customers emphasized loudly -- therefore monetization would be difficult.  

In order to provide RoI, MDG is offering hosting services.  A great many small websites is less economical for them than dozens of very large apps. Hell AWS is an amazing business, I'd like to get a piece of that action too!

I do not begrudge MDG for taking this path, but I'm sad that their goals shifted from developer experience for all to developer services for few!  

### What If's?

Open source is HARD, and Meteor was/is providing value to developers.  They should get paid for their contribution to app development ecosystem. 

What if instead they offered a non-mongodb backend sooner?  This seemed to the primary critique pre-1.0.  What if Angular-Meteor never happened (a strategic error IMO given angular 1.0 is being set to pasture by Google).

## Community Feedback 

Many agree the old Meteor was magic and want it back. A comment from [Meteor forum](https://www.discovermeteor.com/blog/the-state-of-meteor-part-1-what-went-wrong/#comment-2470340694): 

> Lego brick development is the holy grail of programming and Meteor has that in smart packages. Getting sidetracked by the latest JS flavor of the month (Angular, React, etc) at the expense of the smart package scheme will be the death of the framework. 

Another [comment](https://www.discovermeteor.com/blog/the-state-of-meteor-part-2-what-happens-next/) from state of meteor thread: 

> As a seasoned developer (15 years building web apps) I liked Meteor (and Blaze really) because it made all those decisions for me, and then got out of the way. I could cobble together my own stack, and I've done that, but what happens is I end up spending too much of my mental energy on that problem, and less on the business needs of whatever I'm building. What I love about Meteor is that even if I don't need real time data access (DDP), or even if MongoDB doesn't scale well, I spend more of my time thinking about how to solve business problems. 

## Conclusions 

Javascript fatigue continues.  Developers will get crushed by the complexity of day-to-day app building in the for the modern web.  Maybe some will just start developing explicitly for native, other look to react-webpack, feathers, npm-as-build-tool solutions.  Angular2.0-Firebase anyone? Who knows... 

We'll all look back fondly at the Meteor 1.0 days and yearn for a platform that makes developing web applications such a joy again. 

