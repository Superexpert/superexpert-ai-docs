---
layout: default
title: Superexpert.AI Plugins
plugins:
  - name: "Web Search Tool"
    description: "This plugin enables Superexpert.AI to perform web searches using Tavily."
    url: "/plugins/websearch-tool"
  - name: "Orange Theme"
    description: "This plugin adds a new orange chat theme."
    url: "/plugins/orange-theme"
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
                Extend Superexpert.AI with Plugins
            </h2>
            <p class="text-base sm:text-lg md:text-xl text-gray-700 max-w-3xl mx-auto">
                Add new AI models, tools, and themes.
            </p>
        </div>
    </div>
    <div class="max-w-4xl mx-auto">
      <div class="grid grid-cols-1 gap-4">
        {% for plugin in page.plugins %}
        <a href="{{ plugin.url }}">
          <div class="p-6 bg-white rounded-xl shadow hover:shadow-lg transition-shadow duration-300 border border-gray-200">
            <h3 class="text-xl font-semibold text-gray-900">{{ plugin.name }}</h3>
            <p class="mt-2 text-gray-600">{{ plugin.description }}</p>
          </div>
        </a>
        {% endfor %}
      </div>
    </div>
</section>
