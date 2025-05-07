---

layout: content
title: Superexpert.AI - Choose a Theme
description: Learn how to select, modify, and create custom themes for your Superexpert.AI chat interface.
tag: Docs
heading: Choose a Theme
subheading: Customize the Appearance of Your Chat Interface
---

<article>
{% capture markdown_content %}

# Customizing Themes in Superexpert.AI

Superexpert.AI allows you to fully customize the look of your chat interfaces by selecting, modifying, or creating themes.

## Selecting a Theme

To select a theme for your chat interface:

1. Click the **Agents** menu from the main navigation.
2. Click on the **Tasks** button next to the agent you wish to customize.
3. Expand the **Theme** section and select your desired theme.

![Choosing a Theme](choose-theme.png)

*Figure 1: Selecting a theme from the dropdown.*

By default, tasks inherit the theme set in the `global` task. You can override this setting individually for each task.

## Modifying an Existing Theme

Superexpert.AI themes are managed via CSS modules located in the `themes/chat-bot` folder. To modify an existing theme, follow these steps:

1. Open the relevant CSS module file (e.g., `default.module.css`).
2. Update the CSS rules as desired. For example, changing the background color of the Default theme:

```css
.chatPage {
    @apply flex flex-col min-h-screen bg-pink-50 text-lg;
    font-family: 'Inter', sans-serif;
}
```

The above example sets the page background to pink using Tailwind classes.

![Modified Theme Example](pink-theme.png)

*Figure 2: Theme modified to have a pink background.*

Superexpert.AI uses Tailwind CSS, but you can use standard CSS if preferred.

To modify the HTML structure (such as the logo or adding new elements), edit the `app/(chat)/ui/chat-bot.tsx` ReactJS file.

## Creating a New Custom Theme

To create a new theme from scratch:

### Step 1: Create a New CSS Module

Create a new CSS file in the `themes/chat-bot` directory, for example `super.module.css`, and define your styles:

```css
.chatPage {
    @apply flex flex-col min-h-screen bg-indigo-50 text-gray-900;
    font-family: 'Roboto', sans-serif;
}
```

### Step 2: Register Your Theme

Add your new theme to `themes/chat-bot/themes.ts`:

```js
import stylesSuper from '@/themes/chat-bot/super.module.css';

registerTheme({
    id: 'super',
    description: 'A professional, clean Superexpert.AI theme.',
    name: 'Super Theme',
    imagePreview: '/themes/super/super-preview.png',
    theme: stylesSuper,
});
```

Make sure you place a preview image in `public/themes/super/` to visually represent your theme in the interface.

After completing these steps, your custom theme becomes available for selection:

![Custom Theme Applied](custom-theme.png)

*Figure 3: Applying your custom theme.*

## Sharing Themes via NPM

You can package and share your Superexpert.AI themes as NPM modules. For detailed instructions, refer to the [Create Custom Plugins](/docs/create-custom-plugins) documentation.

{% endcapture %}
{{ markdown_content | markdownify }}

</article>