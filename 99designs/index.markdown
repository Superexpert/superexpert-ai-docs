---
layout: default
title: 99 Designs Competition
---


# 99Designs Competition


## Background Context

Superexpert.AI is an open source platform for building AI agents. I need to design two things:


1. The Superexpert.AI platform itself -- users can download the app from [GitHub](https://github.com/Superexpert/superexpert-ai){:target="_blank"} and run it locally. Alternatively, users can try out the app using the live demo at [demo.superexpert.ai](https://demo.superexpert.com){:target="_blank"}
2. The Superexpert.AI website -- Users can navigate to superexpert.ai (this website) to view the landing page and product documentation. This website should be friendly and professional.

## Technology

I use Tailwind for all styling for both the Superexpert.AI platform and the superexpert.ai website. 

## Color Palette

My preference is to stick with an orange color palette for both the Superexpert.AI platform and the Superexpert.AI website. See [https://superexpert.com/](https://superexpert.com/).

For syntax highighting, I can use any of these themes: https://jwarby.github.io/jekyll-pygments-themes/languages/ruby.html

## Responsiveness

Both the Superexpert.AI platform and the Superexpert website need to work on both desktop and mobile.

## Terminology

* "Superexpert.AI" - The name of the platform should be a single word including ".AI".
* "Open Source" -- Not "Open-Source".
* "Platform" -- Superexpert.AI is a "platform" and not a "framework."

## Pages

I need designs for the following 5 pages:

### 1.Landing Page

* goal: This is the main landing page. I will be promoting this page everywhere. The goal is to drive downloads of the Superexpert.AI framework.
* location: [https://superexpert.ai](https://superexpert.ai)
* audience: The primary audience is software engineers with a secondary audience of business decision makers (Product Managers, VPs).
* inspiration: https://www.langchain.com/langgraph,  https://anythingllm.com/, https://www.restack.io/

### 2.Install In Minutes

* goal: This is a step-by-step walkthrough of how users can install the platform. I will use the design for this page as the template for all of the other walkthroughs (for example, Quick Start, Create Attachments, Deploy to Production, etc.) The experience should be friendly.
* location: [https://superexpert.ai/docs/install-in-minutes/](https://superexpert.ai/docs/install-in-minutes/)
* audience: The audience is software engineers.

### 3.Task Definition Form

* goal: This is the form that users complete to define an agent task (the heart of the application). The goal is to prevent the user from being overwhelmed with the number of configuration options. For example, the user can configure the LLM model, server tools, attachments, RAG, etc.  
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Tasks" and then clicking "Edit" next to the "home" or "global" task. I've also grabbed the page in a [PDF file](home-task.pdf){:target="_blank"}. 
* audience: The audience is software engineers who might not understand many of the options. For example, they might not know when to pick a different temperature setting or add an attachment.
* Notes: 
    * The design should be minimalistic and not get in the way of the functionality of the form. The goal should be to keep the form as friendly and simple to use as possible.
    * Notice that some form fields are disabled (the fields have a gray background). You cannot change the Name or Description for the "home" and "global" task. However, you can change the Name and Description for any new tasks that you create.
    * Notice the yellow "Demo Mode" warnings. The demo version of the Superexpert.AI platform has some functionality disabled at https://demo.superexpert.ai (otherwise, people would be uploading massive amounts of database data).

### 4.Chat Form 1
* goal: Simple but distinctive. This is the AI chat interface that you build with the Superexpert.AI platform. 
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Chat." I've also grabbed the page in a [PDF file](chat.pdf){:target="_blank"}. 
* audience: The audience is the end users of the Superexpert AI platform -- not the software engineers but their customers.
* Notes: 
    * Notice that there is a busy-wait indicator when the AI Agent is thinking.
    * Using the Task Definition Form, the developer can choose a particular theme to use with each task. In other words, the Chat appearance can be modified by the developer by using a theme picker.


### 5.Chat Form 2
* goal: Simple but distinctive. A second version of the chat interface that is dramatically different than Chat Form 1. 
* location: You can view this page at [https://demo.superexpert.ai](https://demo.superexpert.ai) by creating a new agent and clicking "Chat." I've also grabbed the page in a [PDF file](chat.pdf){:target="_blank"}. 
* audience: The audience is the end users of the Superexpert AI platform -- not the software engineers but their customers.

