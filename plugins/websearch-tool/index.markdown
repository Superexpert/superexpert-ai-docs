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
<p class="py-4">
Execute the following command from the root of your superexpert-ai project folder:
</p>
{% highlight bash %}
npm install @superexpert-ai/websearch-tool
{% endhighlight %}

<p class="py-4">
    Add the plugin to your superexpert-ai/superexpert-ai.plugins.server.ts file:
</p>
{% highlight js %}
// other plugins...
import '@superexpert-ai/websearch-tool';
{% endhighlight %}
<h2 class="font-bold text-2xl pt-4">Usage</h2>
<p class="py-4">
After installion, you can pick the <code>Web Search Tool</code> plugin as a server tool or as a context data tool.
</p>
    </div>
</section>

