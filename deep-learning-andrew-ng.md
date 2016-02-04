# Deep Learning, Self-Taught Learning and Unsupervised Feature Learning

From Andrew Ng [via YouTube](https://www.youtube.com/watch?v=n1ViNeWhC24&ab_channel=黄鑫), published on 13 May 2013 at Graduate Summer School: Deep Learning, Feature Learning. 

## What do we want computers to do for us? 


We want computers to take our data (images, audio, text) and do things like: 

* images/video
	* label
	* suggest tags
	* image search

* audio 
	* speech recognition
	* music classification 
	* speaker ID

* text 
	* web search
	* anti-spam
	* machine translation 


> Machine Learning is the best shot at the above tasks, but its a long hard road ahead.

### Why is machine learning so hard?

Computer vision problem: look at pixel intensity values and determine what object you're looking at. 

This is not easy!  It involves comparing diagnosing `feature representation`, like "does a bike have handlebars? wheels?" and then passing this feature info to the learning algo.

> Lots of time is being spent in Silicon Valley developing feature representations.

### Where do we get the features from? 

Teams of 10s-100s of researchers spent decades hand-engineering features.  For example, one common technique, SIFT, took David Lo (s) 10 years to develop SIFT, and it works pretty well, but still needs improvement.  

> Even elite researchers in the field of machine learning often have difficulty comprehending the code! 



## One-learning algorithm hypothesis 

Most of human learning can be explained with a single algorithm.  This is a good thing, since most of learning can explained in half a page of pseudocode. 

A learning algorithm once trained is complex, but the complexity of the things we're training usually comes from the DATA, not the algorithm itself. 

Quote from [Wired]. “People understand the linear algebra behind deep learning. But the models it produces are less human-readable. They’re machine-readable,” Nicholson says. “They can retrieve very accurate results, but we can’t always explain, on an individual basis, what led them to those accurate results.” [Wired]: www.wired.com/2016/02/ai-is-changing-the-technology-behind-google-searches/

## Can we learn better feature representation?

