---
title: "Getting Started with Hugo"
date: 2023-08-15
draft: false
tags: ["hugo", "static site", "web development"]
---

# Getting Started with Hugo

Hugo is a fast and modern static site generator written in Go. It makes website creation fun again.

## Why I Chose Hugo for My Blog

When I was looking for a platform to host my blog, I had several requirements:

1. **Speed**: Both in development and for the end user
2. **Simplicity**: Easy to maintain and update
3. **Flexibility**: Ability to customize as needed
4. **Markdown Support**: For easy content writing

Hugo checked all these boxes. It's incredibly fast, with build times measured in milliseconds for most sites. The development server has live reload built-in, which makes the writing and editing process smooth and enjoyable.

## Basic Hugo Structure

A typical Hugo site has the following structure:

```
my-hugo-site/
│
├── archetypes/
├── assets/
├── content/
├── data/
├── layouts/
├── static/
├── themes/
└── config.toml
```

The `content` directory is where all your content lives. For a blog, you'd typically have a structure like:

```
content/
├── blog/
│   ├── post-1.md
│   └── post-2.md
└── about/
    └── index.md
```

## Getting Started

If you're interested in trying Hugo for your own site, installation is simple:

```bash
# Install Hugo on macOS
brew install hugo

# Create a new site
hugo new site my-awesome-site

# Add a theme
cd my-awesome-site
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo theme = \"ananke\" >> config.toml

# Create your first post
hugo new posts/my-first-post.md

# Start the development server
hugo server -D
```

And that's it! Your site should be running at http://localhost:1313/.

## Conclusion

Hugo has been a fantastic choice for my blogging needs. It's fast, flexible, and has a great community behind it. If you're looking for a static site generator, I highly recommend giving Hugo a try!

In future posts, I'll dive deeper into customizing Hugo themes and creating more complex layouts. Stay tuned! 