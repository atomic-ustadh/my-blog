#  Tech Tuts
>### Welcome to Tech Tuts, your go-to blog for all things tech! Dive into tutorials, tips, and insights.

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
│   ├───consts.ts
│   ├───content.config.ts
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
    ├───assets\   --- Static assets like images
    │   ├───blog-placeholder-about.jpg
    │   └───earth.png
    ├───components\ --- Astro/React/Vue/Svelte/Preact components.
    │   ├───BaseHead.astro
    │   ├───Footer.astro
    │   ├───FormattedDate.astro
    │   ├───Header.astro
    │   └───HeaderLink.astro
    ├───content\ --- Markdown and MDX files for blog posts.
    │   └───blog\
    │       ├───markdown-style-guide.md
    │       ├───second-post.md
    │       ├───third-post copy.md
    │       ├───using-mdx.mdx
    │       └───wordpress-installation.md
    ├───layouts\ --- Layout components to wrap pages.
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

1. **Clone the repository**

   ```bash
   npm create astro@latest -- --template blog
   ```

2. **Install dependencies**

   ```bash
   npm install
    ```

3. **Start the development server**

   ```bash
   npm run dev
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

## 👀 Want to learn more?
Check out the official [Astro documentation](https://docs.astro.build)

## Tech Stack
- [Astro](https://astro.build/)
- [MDX](https://mdxjs.com/)
- [Netlify](https://www.netlify.com/)

## Deployment

This site is configured to deploy to [Netlify](https://www.netlify.com/).
