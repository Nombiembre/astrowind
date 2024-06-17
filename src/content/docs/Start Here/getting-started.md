---
title: Getting started
description: Get started with Astro.
sidebar:
  order: 1
---

Starlight is a full-featured documentation theme built on top of the Astro framework. This guide will help you get started with a new project. See the manual setup instructions to add Starlight to an existing Astro project.

## Quick Start

### Create a new project

Create a new Astro + Starlight project by running the following command in your terminal:

```bash
astro create --template starlight my-project
```

This will create a new project in the `my-project` directory with the necessary files and folders to get started.

### Install dependencies

Install the necessary dependencies by running the following command in your project directory:

```bash
npm install
```

### Start the development server

Start the development server by running the following command:

```bash
npm run dev
```

This will start the development server and open your project in your default browser.

### Build the project

To build the project for production, run the following command:

```bash
npm run build
```

This will create a production-ready build of your project in the `dist` directory.

### Deploy the project

To deploy your project to a hosting provider, such as Netlify or Vercel, you can use the following command:

```bash
npm run deploy
```

This will build your project and deploy it to the hosting provider.

# Manual Setup

If you want to add Starlight to an existing Astro project, follow these steps:

1. Install the necessary dependencies:

```bash
npm install @astrojs/starlight
```

2. Import the Starlight component in your `src/pages/index.astro` file:

```astro
---
import StarlightPage from "@astrojs/starlight/components/StarlightPage.astro";
---

<StarlightPage frontmatter={{ title: "My Project" }}>
  <h1>Welcome to my project!</h1>
</StarlightPage>
```

3. Create a `src/content/docs/index.md` file with the following content:

```md
---
title: My Project
description: A short description of my project.
---

# Introduction

Welcome to my project!
```

4. Run the development server:

```bash
npm run dev
```

This will start the development server and open your project in your default browser.

5. Build the project:

```bash
npm run build
```

This will create a production-ready build of your project in the `dist` directory.

6. Deploy the project:

```bash
npm run deploy
```

This will build your project and deploy it to the hosting provider.

# Customization

Starlight provides a number of customization options to help you tailor the theme to your needs.
