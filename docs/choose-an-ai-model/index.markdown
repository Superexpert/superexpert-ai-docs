---
layout: content
title: Superexpert.AI - Choose an AI Model
description: Superexpert.AI enables you to use LLM models from OpenAI, Anthropic, and Google.
tag: Docs
heading: Choose an AI Model
subheading: Select the Best Model for the Task

---
<article>
{% capture markdown_content %}

# Choosing an AI Model

Optimize your Superexpert.AI agents by selecting the right AI models for your tasks, balancing performance, cost, and complexity.

## Selecting an AI Model for a Task

Superexpert.AI lets you easily specify which AI model your agent should use. You can set a default model for all tasks or select specific models tailored to individual tasks.

### Setting a Global AI Model

To define a default AI model for all tasks:

1. Click **Agents** in the main navigation menu.
2. Select the agent you want to modify by clicking the **Tasks** button next to it.
3. You'll see a list of all tasks associated with the agent. Every agent includes a **Global Task** and a **Home Task**.
4. Click the **Global Task** to edit it.
5. Under the **AI Model** section, select the desired model (e.g., GPT-4.1, Claude 3 Opus, Gemini 2.0 Pro).
6. Save your changes. Changes made to the global task become the default for all other tasks.

![Choose Model](choose-model.png)
*Figure 1: Choosing the default AI model.*

### Specifying a Model for Individual Tasks

For specific tasks, you might not always need the most powerful model. Choose a more cost-effective model to optimize your expenses.

1. Go to the specific task you want to edit.
2. In the **AI Model** section, select a suitable model based on task complexity (e.g., use GPT-4o mini for faster responses or GPT-4.5 Preview for creative tasks).
3. Save your changes.

This flexibility helps you control costs without sacrificing performance—only pay for the Einstein-level models when needed!

## Registering a New AI Model

You can easily integrate new AI models from providers like OpenAI, Anthropic, or Google by updating the Superexpert.AI configuration.

### Step-by-Step Guide

1. Open the file located at `/lib/adapters/system-adapters.ts`.
2. Use the existing adapters to register a new model. For instance, here's how GPT-4.1 is registered:

```typescript
// Register OpenAI: GPT-4.1 
registerLLM({
    definition: {
        id: 'gpt-4.1',
        name: 'OpenAI: GPT-4.1',
        provider: 'openai',
        description:
            'Flagship GPT model for complex tasks',
        maximumOutputTokens: 32_768,
        maximumTemperature: 2,
    },
    adapter: OpenAILLMAdapter,
});
```

### Adding Future Models

Integrating future models, like a hypothetical GPT-6, is simple:

1. Copy and modify an existing registration block.
2. Update the model `id`, `name`, and `description`.
3. Save the file and redeploy Superexpert.AI to start using the new model immediately.

By simplifying model integration, Superexpert.AI ensures your agents are always leveraging cutting-edge AI advancements.



{% endcapture %}
{{ markdown_content | markdownify }}

</article>