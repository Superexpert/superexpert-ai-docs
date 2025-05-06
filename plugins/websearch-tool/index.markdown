---
layout: content
title: Superexpert.AI Plugins - Websearch Tool
tag: Plugins
heading: Web Search Tool
---

<h2 class="font-bold text-2xl">Installation</h2>
<p class="py-4">
Execute the following command from the root of your superexpert-ai project folder:
</p>
{% highlight bash %}
npm install @superexpert-ai/websearch-tool
{% endhighlight %}

<p class="py-4">
    Add the plugin to your superexpert-ai.plugins.server.ts file:
</p>
{% highlight js %}
// other plugins... 
import '@superexpert-ai/websearch-tool';
{% endhighlight %}

<p class="py-4">
    Add your Tavily API key to your .env file (Get a key for free from <a href="https://tavily.com/" target="_blank">Tavily</a>):
</p>
{% highlight js %}
TAVILY_API_KEY=<You API Key>
{% endhighlight %}

<h2 class="font-bold text-2xl pt-4">Usage</h2>
<p class="py-4">
After installion, you can pick the <code>Web Search Tool</code> plugin as a server tool or as a context data tool.
</p>
