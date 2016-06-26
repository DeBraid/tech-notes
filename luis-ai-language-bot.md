# LUIS: a bot for natural language 

> Microsofts Language Understanding Intelligent Service (LUIS) offers a fast and effective way of adding language understanding to applications.

from [Docs](http://docs.botframework.com/builder/node/guides/understanding-natural-language/).  Also see 10min LUIS [tutorial](https://vimeo.com/145499419).

## What is LUIS 

LUIS uses pre-built models from `Bing` and `Cortana` to understand language and AI. 

It has a `bot builder` which uses the `LuisDialog` class to reference a custom language model (your training data).  Adding `intents` handlers to take **actions** in response to user `utterances`.

LUIS lets you build language models specific to your domain. 

Intents are actions (start, stop), entities are types (run / walk).

Utterances are parsed, and the model is trained by specifying the intent and selecting the entity within a given utterance. 

> IE: starting my jog now

Your intent is to start an activity, the entity (or activity) is a jog.

### Model features can act as a class.  

For example, [run, jog, walk, sprint, bike ride, swim, etc] could all be grouped as a class.  LUIS will accept this as a `Model Feature`.

### Pre-built entities 

From Bing, and elsewhere, you can choose list of pre-built entities like: 

* numbers 
* temp 
* money 
* encyclopedia

## Intents, Entities, and Model Training

LUIS allows developers to quickly deploy an `http` endpoint that will take the `sentences` (utterances) you send it, and interpret them as `intents` and key `entities`.

Once your application is deployed and traffic starts (querys are being sent / questions are being asked) LUIS uses active learning to improve itself.

Hierarchical Entities: 
> The generic entity acts as the parent and the children are the specific types, or sub-groups, under the parent, yet both share the same characteristics. 

For example, a generic entity may be called “Date” and the specific children of this parent may be called “StartDate” and “EndDate”. 

## Create Your Model

















