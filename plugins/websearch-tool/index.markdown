---
layout: default
title: Superexpert.AI Plugins - Websearch Tool
---


<section class="py-12 md:py-20 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto text-center">
        <!-- Section Header -->
        <div class="mb-12">
            <div class="my-8 h-8 px-6 py-4 bg-white rounded-3xl shadow-[0px_3px_15px_0px_rgba(0,0,0,0.10)] outline outline-1 outline-offset-[-1px] outline-slate-50 inline-flex justify-start items-start gap-1.5">
                <div class="self-stretch flex justify-start items-center gap-1">
                    <div class="justify-start text-zinc-800 text-base font-normal leading-normal">
                        Plugins
                    </div>
                </div>
            </div>
            <h2 class="text-3xl sm:text-4xl md:text-5xl font-normal text-gray-900 mb-4">
                Web Search Tool
            </h2>
        </div>
    </div>
    <div class="max-w-4xl mx-auto">
        <h2 class="font-bold text-2xl">Installation</h2>
        Execute the following command from the root of your superexpert-ai project folder:
<div markdown="1">
```bash
npm install @superexpert-ai/websearch-tool
```
<p class="py-2">
    Add the plugin to your superexpert-ai/superexpert-ai.plugins.server.ts file:
</p>
{% highlight ruby linenos hl_lines="2,4-6" %}
import '@/lib/adapters/llm-adapters/system-adapters'; 
import './lib/system-tools/system-server-data';
import './tools/server-data';
import './lib/system-tools/system-server-tools';
import './tools/server-tools';
import './lib/system-tools/system-client-tools';
import './tools/client-tools';
import '@superexpert-ai/websearch-tool';
{% endhighlight %}

</div>
    </div>
</section>

