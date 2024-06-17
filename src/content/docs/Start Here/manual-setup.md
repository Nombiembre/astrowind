---
title: Manual Setup
description: Manual setup instructions to add Starlight to an existing Astro project.
slug: start-here/manual-setup
sidebar:
  order: 2
---

The quickest way to create a new Starlight site is using create astro as shown in the Getting Started guide. If you want to add Starlight to an existing Astro project, this guide will explain how.

## Set up Starlight

To follow this guide, you’ll need an existing Astro project.

### Add the Starlight integration

Starlight is an Astro integration. Add it to your site by running the astro add command in your project’s root directory:

```bash
npx astro add starlight
```

This will install the required dependencies and add Starlight to the integrations array in your Astro config file.

### Configure the integration

The Starlight integration is configured in your astro.config.mjs file.

Add a title to get started:

```js
import { defineConfig } from "astro/config";
import starlight from "@astrojs/starlight";

export default defineConfig({
  integrations: [
    starlight({
      title: "My delightful docs site",
    }),
  ],
});
```

Find all available options in the Starlight configuration reference.

### Configure content collections

Starlight is built on top of Astro’s content collections, which are configured in the src/content/config.ts file.

Create or update the content config file, adding a docs collection that uses Starlight’s docsSchema:

```js
import { defineCollection } from "astro:content";
import { docsSchema } from "@astrojs/starlight/schema";

export const collections = {
  docs: defineCollection({ schema: docsSchema() }),
};
```

### Create a docs index page

Create a docs index page in the src/content/docs/index.md file with the following content:

```md
---
title: My Project
description: A short description of my project.
---

# Introduction

Welcome to my project!
```

## Start the development server

Start the development server by running the following command:

```bash
npm run dev
```

This will start the development server and open your project in your default browser.

## Build the project

To build the project for production, run the following command:

```bash
npm run build
```

This will create a production-ready build of your project in the `dist` directory.

## Deploy the project

To deploy your project to a hosting provider, such as Netlify or Vercel, you can use the following command:

```bash
npm run deploy
```

This will build your project and deploy it to the hosting provider.

# Customization

Starlight provides a number of customization options to help you tailor the theme to your needs.
