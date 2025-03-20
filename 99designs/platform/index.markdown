---
layout: default
title: 99 Designs Competition - Superexpert.AI Platform
---


# 99Designs Competition - Superexpert.AI Platform


## Background Context

Superexpert.AI is an open source platform for building AI agents. Developers can download the app from [GitHub](https://github.com/Superexpert/superexpert-ai){:target="_blank"} and run it locally. Alternatively, developers can try out the app using the live demo at [demo.superexpert.ai](https://demo.superexpert.com){:target="_blank"}

## Technology

I use Tailwind for all styling for the Superexpert.AI platform. 

## Color Palette

My preference is to stick with an orange color palette for the Superexpert.AI platform  See [https://superexpert.com/](https://superexpert.com/).


## Responsiveness

The Superexpert.AI platform needs to work on both desktop and mobile.

## Terminology

* "Superexpert.AI" - The name of the platform should be a single word including ".AI".
* "Open Source" -- Not "Open-Source".
* "Platform" -- Superexpert.AI is a "platform" and not a "framework."

## Inspiration

* [GitHub Settings Page](github.pdf) - Organizes complex set of user settings in a clean way.

## Pages

I need designs for the following 4 pages:

### 1. Agent List

* goal: This is the first page that a new user of the platform sees after registering. The developer can
create a new agent, edit existing agents, edit the tasks associated with an agent, or chat with an agent.

* location: you can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by registering. Alternatively, here is a [PDF file](agents.pdf){:target="_blank"}

* Notes:
    * Keep it simple. The goal is to make the platform as usable as possible for third-party developers.
    * Notice the yellow "Demo Mode" warnings. The warning shows up on the demo site to warn developers that
    not all functionality is enabled in the demo version.

### 2.Task Definition Form

* goal: This is the form that users complete to define an agent task (the heart of the application). The goal is to prevent the user from being overwhelmed with the number of configuration options. For example, the user can configure the LLM model, server tools, attachments, RAG, etc.  
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Tasks" and then clicking "Edit" next to the "home" or "global" task. I've also grabbed the page in a [PDF file](home-task.pdf){:target="_blank"}. 
* audience: The audience is software engineers who might not understand many of the options. For example, they might not know when to pick a different temperature setting or add an attachment.
* Notes: 
    * The design should be minimalistic and not get in the way of the functionality of the form. The goal should be to keep the form as friendly and simple to use as possible.
    * Notice that some form fields are disabled (the fields have a gray background). You cannot change the Name or Description for the "home" and "global" task. However, you can change the Name and Description for any new tasks that you create.
    * Notice the yellow "Demo Mode" warnings. The demo version of the Superexpert.AI platform has some functionality disabled at https://demo.superexpert.ai (otherwise, people would be uploading massive amounts of database data).

### 3.Chat Form 1
* goal: Simple but distinctive. This is the AI chat interface that you build with the Superexpert.AI platform. 
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Chat." I've also grabbed the page in a [PDF file](chat.pdf){:target="_blank"}. 
* audience: The audience is the end users of the Superexpert AI platform -- not the software engineers but their customers.
* Notes: 
    * Notice that there is a busy-wait indicator when the AI Agent is thinking.
    * Using the Task Definition Form, the developer can choose a particular theme to use with each task. In other words, the Chat appearance can be modified by the developer by using a theme picker.


### 4.Chat Form 2
* goal: Simple but distinctive. A second version of the chat interface that is dramatically different than Chat Form 1. 
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Chat." I've also grabbed the page in a [PDF file](chat.pdf){:target="_blank"}. 
* audience: The audience is the end users of the Superexpert AI platform -- not the software engineers but their customers.



