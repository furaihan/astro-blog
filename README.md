# Astro Blog

A modern, fast, and beautiful blog built with **Astro.js** and **Tailwind CSS**. This blog features a green color palette theme, Markdown support for blog posts, and is optimized for performance and developer experience.

## ✨ Features

- **🚀 Lightning Fast**: Built with Astro.js for optimal performance
- **📝 Markdown Support**: Write blog posts in Markdown with frontmatter
- **🎨 Beautiful Design**: Clean, green-themed design with Tailwind CSS
- **📱 Responsive**: Looks great on all devices and screen sizes
- **🏷️ Tagging System**: Organize posts with a flexible tagging system
- **📅 Date Organization**: Posts are automatically sorted by publication date
- **⚡ Deno Ready**: Configured to run with Deno runtime

## 🚀 Quick Start

### Prerequisites

Make sure you have [Deno](https://deno.land/) installed on your system:

```bash
# Install Deno (if not already installed)
curl -fsSL https://deno.land/install.sh | sh
```

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd astro-blog
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   deno task dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:4321` to see your blog in action!

## 📝 Creating Blog Posts

To create a new blog post:

1. Create a new `.md` file in the `src/content/blog/` directory
2. Add frontmatter with the required fields:

```markdown
---
title: "Your Post Title"
description: "A brief description of your post"
date: 2024-01-15
tags: ["tag1", "tag2", "tag3"]
draft: false  # Set to true to hide the post
---

# Your content here

Write your blog post content using Markdown syntax.
```

### Frontmatter Fields

- `title` (required): The title of your blog post
- `description` (required): A brief description used in post previews
- `date` (required): Publication date in YYYY-MM-DD format
- `tags` (optional): Array of tags to categorize your post
- `draft` (optional): Set to `true` to hide the post from the blog

## 🎨 Color Palette

The blog uses a green color palette with these primary colors:

- **Primary Green**: Various shades from `primary-50` to `primary-950`
- **Accent Green**: Lime green variants from `accent-50` to `accent-950`
- **Neutral Colors**: Gray shades for text and backgrounds

You can customize these colors in the `tailwind.config.js` file.

## 📁 Project Structure

```
├── public/                 # Static assets
├── src/
│   ├── content/
│   │   ├── blog/          # Blog post markdown files
│   │   └── config.ts      # Content collection configuration
│   ├── layouts/
│   │   ├── Layout.astro   # Base layout component
│   │   └── BlogPost.astro # Blog post layout
│   ├── pages/
│   │   ├── blog/
│   │   │   ├── index.astro      # Blog listing page
│   │   │   └── [...slug].astro  # Individual blog posts
│   │   └── index.astro    # Homepage
│   └── styles/
│       └── global.css     # Global styles and Tailwind imports
├── astro.config.mjs       # Astro configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── deno.json             # Deno tasks and configuration
└── package.json          # Project dependencies
```

## 🛠️ Available Commands

| Command              | Action                                      |
| :---                | :---                                        |
| `deno task dev`     | Starts local development server             |
| `deno task build`   | Build your production site to `./dist/`    |
| `deno task preview` | Preview your build locally                  |
| `deno task astro`   | Run Astro CLI commands                      |

## 📚 Learn More

- [Astro.js Documentation](https://docs.astro.build)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Deno Documentation](https://deno.land/manual)

## 🤝 Contributing

Feel free to contribute to this project by submitting issues or pull requests.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).