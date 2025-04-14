# AI Tools Directory Website 🤖

A comprehensive directory of AI tools and resources presented in a clean, responsive 3-column grid layout.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/ai-tools)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization](#customization)
  - [Adding Directory Items](#adding-directory-items)
  - [Modifying Categories](#modifying-categories)
  - [Updating Hero Section](#updating-hero-section)
  - [Styling Changes](#styling-changes)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support](#support)

## Overview

AI Tools is a curated directory website showcasing the latest artificial intelligence tools and resources. The website features a responsive grid layout, filtering capabilities, and an easy-to-navigate interface.

## Features

- 🎯 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category-based filtering
- 💨 Fast loading performance
- 📱 Mobile-friendly design
- 🎨 Customizable styling
- 🔄 Easy content updates

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-tools.git
cd ai-tools
```

2. Install dependencies:
```bash
npm install
```

3. Run development server:
```bash
npm run dev
```

## Directory Structure

```
ai-tools/
├── src/
│   ├── components/
│   │   ├── Card.js
│   │   ├── Grid.js
│   │   └── Hero.js
│   ├── data/
│   │   └── tools.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
│       └── index.js
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization

### Adding Directory Items

Add new tools by editing `src/data/tools.json`:

```json
{
  "tools": [
    {
      "id": "tool-name",
      "title": "Tool Name",
      "description": "Tool description goes here",
      "category": "category-name",
      "url": "https://toolurl.com",
      "image": "/images/tool-image.png"
    }
  ]
}
```

### Modifying Categories

Update categories in `src/data/categories.js`:

```javascript
export const categories = [
  {
    id: "category-1",
    name: "Category Name",
    description: "Category description"
  }
];
```

### Updating Hero Section

Modify the hero section in `src/components/Hero.js`:

```javascript
const Hero = () => {
  return (
    <div className="hero">
      <h1>Your Custom Title</h1>
      <p>Your custom description</p>
    </div>
  );
};
```

### Styling Changes

Customize styles in `src/styles/main.css`:

```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --background-color: #ffffff;
}
```

## Deployment

1. Create a Vercel account at [vercel.com](https://vercel.com)
2. Install Vercel CLI:
```bash
npm i -g vercel
```

3. Deploy:
```bash
vercel
```

## Custom Domain Setup

1. Go to Vercel dashboard
2. Select your project
3. Click "Settings" → "Domains"
4. Add your domain
5. Follow DNS configuration instructions

## Troubleshooting

Common issues and solutions:

- **Build Errors**: Run `npm clean-install` and try rebuilding
- **Image Loading Issues**: Ensure images are in the correct format (PNG/JPG) and properly referenced
- **Styling Problems**: Clear browser cache and reload
- **Category Filters Not Working**: Check category IDs match between tools and categories

## Support

- 📚 [Documentation](https://docs.yoursite.com)
- 💬 [Discord Community](https://discord.gg/yourserver)
- 🐛 [Issue Tracker](https://github.com/yourusername/ai-tools/issues)
- 📧 [Email Support](mailto:support@yoursite.com)

---

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

Made with ❤️ by [Your Name]