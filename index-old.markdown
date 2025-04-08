---
layout: default
title: home
---


# Headline: "Open Source AI Made Simple"

## Sub-headline: "Build advanced, multi-task AI Agents—no coding required"

## Call-to-Action (CTA): "Download for Free on GitHub" (link to https://github.com/Superexpert/superexpert-ai)
## Secondary Call-to-Action (CTA): "Try the Live Demo - Build a Custom Agent in Under 60 Seconds" (link to https://demo.superexpert.ai/)

# Should emphasize open source

Include "open source (MIT License)” front and center—include a GitHub link icon. (see https://github.com/logos)

# Overview of Features

* ⚡ Build Fast: Deploy sophisticated agents without code.


<img src="/assets/home/agent-instructions.jpg" width="400" />


* 🌐 Fully Customizable: Declarative APIs to integrate your own tools seamlessly.

```typescript
@Tool({
      name:'updateProfile', 
      description: `Update the user's profile`
})
public async updateProfile(
   @ToolParameter({
      name: 'name',
      description: 'The name of the profile property to update',
   })
   name: string,
   @ToolParameter({
      name: 'value',
      description: 'The new value for the profile property',
   })
   value: string
) {
   // Update the user's profile in the database
```

* 📚 Powerful Data Handling: Easily manage document retrieval (RAG) at scale.

<img src="/assets/home/rag.jpg" width="400" />


* 🤖 Multi-Model Compatible: Choose the perfect AI model (OpenAI, Anthropic, Gemini) based on performance and cost.

<img src="/assets/home/ai-models.jpg" width="400" />


* 🏗️ Modern Web Application Architecture: Next.js + TypeScript + PostgreSQL for maximum scalability and performance.

# FAQ


### 1. How much does Superexpert.AI cost?

The platform is open source (MIT license). You can download from [https://github.com/superexpert/superexpert-ai](https://github.com/superexpert/superexpert-ai) for free. 

### 2. Why should a developer choose Superexpert AI over the multitude of other AI platforms available?

Superexpert AI is an open-source platform empowering developers with the flexibility, transparency, and community support to build and deploy cutting-edge AI applications

### 3. What types of applications can I build with Superexpert.AI?

You can build anything from a simple chatbot to a sophisticated AI Agent that can perform hundreds of distinct tasks. For example, you can use Superexpert.AI to build Customer Service Agents, Knowledge Discovery Tools, Employee Onboarding Systems, and Process Automation Solutions. 


For example, a startup can use Superexpert.AI to create a customer support agent that answers product inquiries, checks order status, and processes refunds—without writing a single line of code.

### 4. Can I create custom agents without writing code?

Yes. The Superexpert.AI platform uses a friendly form interface to enable you to configure agents and tasks. You
can build sophisticated AI solutions without writing a single line of code.

### 5. I have complex needs. How easy is to extend the platform?

The Superexpert.AI platform was designed to be extensible. You can easily add custom tools that load custom data for each task (for example, customer profiles) or execute custom functions (display a modal popup asking a customer to complete a form). Superexpert.AI supports a simple declarative method of making tools available to AI Agents that works across different AI providers.

### 6. I need to build an AI Agent that can answer questions concerning information that is stored in hundreds of documents. Does Superexpert.AI support RAG (Retrieval Augmented Generation)?

Yes. You can upload documents and Superexpert.AI will chunk the documents and generate embeddings for you automatically.

### 7. Where can I deploy my application built with Superexpert.AI?

The Superexpert.AI platform is compatible with Vercel, AWS, GCP, and Azure. You can use any hosting provider that supports Node.js and PostgreSQL.


### 8. Can I contribute to the project? What's the process?

Yes. The platform is being actively developed. We happily accept Pull Requests.



