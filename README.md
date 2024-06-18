## How to change site url

- Edit `src/config.yaml` and change `site.site` to your new url
- Edit `astro.config.mjs` and change `site` to your new url

## How to change site title

- Edit `src/config.yaml` and change `site.name` to your new title
- Edit `src/config.yaml` and change `metadata.title.default` to your new title
- Edit `src/config.yaml` and change `openGraph.site_name` to your new title

For Docs site, you can change the title in `astro.config.mjs`:

```js "title"
  starlight({
      title: "AstroWind",
    }),
```

## How to change favicons

Favicons for astrowind are located in `src/assets/favicons` and are used in `src/components/Favicons.astro`
Favicon for docs is located in `public/`

## Dependencies from `dependencies`

### Removed

- `@astrojs/rss`

### Keeped

- `@astrojs/sitemap` Sitemap generation is better for google to understand the site structure
- `@astrolib/analytics`: Google Analytics
- `@astrolib/seo` SEO
- `@astrojs/starlight`: Starlight Documentation Integration
- `@fontsource-variable/inter`: for Inter font
- `astro`: ...
- `astro-embed`: Optimized embeds, used in page "/homes/start-ups/"
- `astro-icon`: Optimized icons
- `limax`: Slugify, used in permalinks.ts
- `lodash.merge`: merge, used in configBuilder.ts
- `unpic`: Optimized images, used in Image.astro and images-optimization.ts

## Dependencies from `devDependencies`

### removed

- `@astrojs/mdx` Mainly used for blog posts
- `globals` JSON file accesible globally, but not being used in onwidget/astrowind
- `reading-time` Dependency for blog posts
- `rehype-plugin-image-native-lazy-loading` Dependency for blog posts
- `sharp` Image processing, but not being used in onwidget/astrowind
- `@eslint/js`
- `@types/eslint__js`
- `@typescript-eslint/eslint-plugin`
- `@typescript-eslint/parser`
- `astro-eslint-parser`
- `eslint`
- `eslint-plugin-astro`
- `typescript-eslint`
- `eslint-plugin-jsx-a11y`

  Add eslint dependencies based on your preferences

### Keeped

- `@astrojs/partytown` Increases web performance
- `@astrojs/tailwind`
- `@iconify-json/flat-color-icons` Critical for the site, used for all the icons
- `@iconify-json/tabler` Critical for the site, used for all the icons
- `@tailwindcss/typography` Better styling for markdown
- `@types/js-yaml` TypeScript support for YAML, used for "/src/config.yaml"
- `@types/lodash.merge` TypeScript support for lodash.merge, used for "/src/utils/configBuilder.ts"
- `js-yaml` for "/src/config.yaml"
- `prettier` Format code with `npm run format`
- `prettier-plugin-astro`
- `tailwind-merge`
- `tailwindcss`
- `typescript`
- `astro-compress`

## Files

### Deleted

- .editorconfig
- .npmrc
- .prettierignore
- .prettierrc.cjs
- .stackblitzrc
- LICENSE.md
- eslint.config.js
- netlify.toml
- package-lock.json
- public/decapcms/config.yml
- public/decapcms/index.html
- sandbox.config.json
- src/components/blog/Grid.astro
- src/components/blog/GridItem.astro
- src/components/blog/Headline.astro
- src/components/blog/List.astro
- src/components/blog/ListItem.astro
- src/components/blog/Pagination.astro
- src/components/blog/RelatedPosts.astro
- src/components/blog/SinglePost.astro
- src/components/blog/Tags.astro
- src/components/blog/ToBlogLink.astro
- src/components/widgets/Announcement.astro
- src/components/widgets/BlogHighlightedPosts.astro
- src/components/widgets/BlogLatestPosts.astro
- src/content/post/astrowind-template-in-depth.mdx
- src/content/post/get-started-website-with-astro-tailwind-css.md
- src/content/post/how-to-customize-astrowind-to-your-brand.md
- src/content/post/landing.md
- src/content/post/markdown-elements-demo-post.mdx
- src/content/post/useful-resources-to-create-websites.md
- src/pages/[...blog]/[...page].astro
- src/pages/[...blog]/[category]/[...page].astro
- src/pages/[...blog]/[tag]/[...page].astro
- src/pages/[...blog]/index.astro
- src/pages/rss.xml.ts
- src/utils/blog.ts
- src/utils/frontmatter.mjs
- vercel.json

### Modified

- .vscode/astrowind/config-schema.json
- .vscode/extensions.json
- .vscode/settings.json
- README.md
- astro.config.mjs
- package.json
- src/components/widgets/Footer.astro
- src/components/widgets/Header.astro
- src/config.yaml
- src/content/config.ts
- src/layouts/LandingLayout.astro
- src/layouts/PageLayout.astro
- src/navigation.js
- src/pages/homes/mobile-app.astro
- src/pages/homes/personal.astro
- src/pages/homes/saas.astro
- src/pages/index.astro
- src/pages/privacy.md
- src/pages/terms.md
- src/types.d.ts
- src/utils/directories.ts
- src/utils/images-optimization.ts
- src/utils/images.ts
- src/utils/permalinks.ts
- src/utils/utils.ts
- tailwind.config.cjs

### New

- src/content/docs/Guides/example.md
- src/content/docs/Reference/example.md
- src/content/docs/Start Here/astro.md
- src/content/docs/Start Here/getting-started.md
- src/content/docs/Start Here/manual-setup.md
- src/content/docs/Start Here/zeus.md
