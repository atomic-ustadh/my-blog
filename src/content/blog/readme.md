---
title: 'Just Read It'
description: 'Lorem ipsum dolor sit amet'
pubDate: 'Jul 08 2022'
heroImage: '../../assets/blog-placeholder-3.jpg'
---
#  Tech Tuts
> Welcome to Tech Tuts, your go-to blog for all things tech! Dive into tutorials, tips, and insights.

## 📚 Features:
- ✅ Minimal styling (make it your own!)
- ✅ 100/100 Lighthouse performance
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support

## Project Structure

``` text
├───.gitignore
├───astro.config.mjs
├───package-lock.json
├───package.json
├───README.md
├───tsconfig.json
├───dist\
│   ├───index.html
├───public\
│   ├───favicon.svg
│   └───fonts\
└───src\
    ├───consts.ts
    ├───content.config.ts
    ├───content.config.ts
    ├───content.config.ts
    ├───content.config.ts
    ├───assets\   ---> Static assets like images
    │   ├───blog-placeholder-about.jpg
    │   └───earth.png
    ├───components\ ---> Astro/React/Vue/Svelte/Preact components.
    │   ├───BaseHead.astro
    │   ├───Footer.astro
    │   ├───FormattedDate.astro
    │   ├───Header.astro
    │   └───HeaderLink.astro
    ├───content\ ---> Markdown and MDX files for blog posts.
    │   └───blog\
    │       ├───markdown-style-guide.md
    │       ├───second-post.md
    │       ├───third-post copy.md
    │       ├───using-mdx.mdx
    │       └───wordpress-installation.md
    ├───layouts\ ---> Layout components to wrap pages.
    │   └───BlogPost.astro
    ├───pages\
    │   ├───about.astro
    │   ├───index.astro
    │   ├───others.astro
    │   ├───rss.xml.js
    │   └───blog\
    │       ├───[...slug].astro
    │       └───index.astro
    └───styles\
        └───global.css
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

The `src/components/` directory is where the Astro/React/Vue/Svelte/Preact components live.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema.


## Getting Started

1. **Create a new Astro Project**

   ```bash
   npm create astro@latest -- --template blog
   ```

2. **Install dependencies:** If you skip this step when creating the Project.

   ```bash
   npm install
    ```

3. **Start the development server**

   ```bash
   npm run dev
   ```

4. **Build for production**

   ```bash
   npm run build
   ```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
| `npm run format`          | Format all `.ts`, `.tsx`, `.astro` and `.md` files |
| `npm run lint`            | Lint all `.ts`, `.tsx`, `.astro` and `.md` files |

## Tech Stack
- [Astro](https://astro.build/)
- [MDX](https://mdxjs.com/)
- [Netlify](https://www.netlify.com/)

## Deployment

This site is configured to deploy to [Netlify](https://www.netlify.com/).
- To deploy a static version of this site:
Netlify is already configured to host static sites. So no configuration needed.

- To deploy a dynamic version of this site:
1. Install the `@astro/Netlify` Adapter
With the `astro add` command. This will install `@astrojs/netlify` and make the appropriate changes to your `astro.config.mjs` file in one step.
    ```bash
    npx astro add netlify
    ```
2. Push your code to a Git repository (GitHub, GitLab, Bitbucket).
3. Create a new site on Netlify and link it to your repository.
4. Set the build command to `npm run build` and the publish directory to `dist/`.
Alternatively, you can create a `netlify.toml` file in the root of your project with the following content:
    ```toml
    [build]
      command = "npm run build"
      publish = "dist"
    ```
5. Click "Deploy Site".

Tech Tuts Deployment? [![Netlify Status](https://api.netlify.com/api/v1/badges/0e980602-116a-41de-b88c-3037ef140f3d/deploy-status)](https://app.netlify.com/projects/techtuts/deploys)

## 👀 Want to learn more?
Check out the official [Astro documentation](https://docs.astro.build)

## 👀 About the Author 

Visit my Portfolio on:

[![My Website](../../assets/globe.svg)](https://atomicustadh.pages.dev/)
[![GitHub](../../assets/github.svg)](https://github.com/atomic-ustadh)
[![LinkedIn](../../assets/linkedin.svg)](https://linkedin.com/in/atomic-ustadh)
[![Twitter(formerly x.com)](../../assets/twitter-x.svg)](https://x.com/atomicustadh)
