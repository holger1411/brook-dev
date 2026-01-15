# Brook - A Free Bootstrap 5 Blog Template

**Live Demo**: [brooks-html-template.netlify.app](https://brooks-html-template.netlify.app/)

## What is Brook?

Brook is a free, open-source blog template built with [Bootstrap 5](https://getbootstrap.com/) and [Eleventy 3](https://www.11ty.dev/). A clean, focused design for writers and content creators.

## Features

- Clean blog layout
- Post grid
- Category pages
- Author section
- Newsletter signup
- Responsive design
- Dark mode support

## For Beginners

If you're familiar with basic HTML but not advanced web development, you can still use Brook. Simply use the `/public` folder from this repository. Edit the content, add your images, and upload it to your web server. Done!

## For Developers

Brook is built on:

- **Bootstrap 5** - CSS framework
- **Eleventy 3** - Static site generator
- **Nunjucks** - Template language (Eleventy also supports Liquid, Handlebars, Pug, and more)
- **Gulp** - Task runner for SCSS compilation and optimization

Eleventy allows you to use various data sources: static content, computed data, APIs, frontmatter, markdown files, and more.

## Requirements

- **Node.js 18+** (required for Eleventy 3)

Check your Node version:

```bash
node --version
```

## Installation

1. Clone or download this repository
2. Open your terminal and navigate to the project folder
3. Run:

```bash
npm install
```

## Development

### Development Build

Build without minification (faster, readable output):

```bash
npm run build-dev
```

Output is stored in the `/dev` folder.

### Watch Mode

For development with auto-rebuild on file changes:

```bash
npm run watch
```

This will:
- Build the site to `/dev`
- Compile SCSS to CSS
- Start BrowserSync
- Auto-rebuild on file changes

## Production Build

Build optimized site for deployment:

```bash
npm run build
```

This will:
- Compile and minify CSS
- Purge unused CSS
- Minify HTML

Output is stored in the `/public` folder - deploy this to your web server.

## License

MIT
