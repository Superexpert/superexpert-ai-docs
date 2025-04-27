---
layout: content
title: Superexpert.AI Plugins - RAG Tool
tag: Plugins
heading: RAG Tool
---

<article>
<h2 class="font-bold text-2xl">Overview</h2>
<p>
The Superexpert.AI RAG tool enables you to reliably upload multiple large files to Superexpert.AI. You can upload  
both text files (including JSON and CSV) and PDF files.
</p>
<p>
If there is a network error or any other type of error then you can resume your upload from the last chunk. That
way, you can handle chunking and uploading hundreds of large files.
</p>

<img src="./rag.png" />

<h2 class="font-bold text-2xl">Usage</h2>
<p class="py-4">
Execute the following command to create the configuration file (rag.config.js):
</p>
{% highlight bash %}
npx @superexpert-ai/rag init
{% endhighlight %}

<p class="py-4">
Execute the following command to chunk and upload the files:
</p>
{% highlight bash %}
npx @superexpert-ai/rag run
{% endhighlight %}



<p>
For details, see <a href="https://www.npmjs.com/package/@superexpert-ai/rag">@superexpert-ai/rag</a>
</p>
</article>
