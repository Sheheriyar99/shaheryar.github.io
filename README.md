# 🚀 Shaheryar's Cloud & AWS Blog

A modern, clean, and professional blog for sharing cloud architecture, DevOps, and AWS expertise. Built with Jekyll and hosted on GitHub Pages.

## ✨ Features

- **Modern Design**: Clean, minimalist interface with AWS orange accent colors
- **Responsive**: Fully responsive on mobile, tablet, and desktop
- **Blog Platform**: Easy to write and publish blog posts
- **AWS Community Builder Integration**: Prominent call-to-action to apply for AWS Community Builder program
- **Fast**: Static site generation with Jekyll
- **SEO Optimized**: Built-in SEO support with jekyll-seo-tag

## 📁 Project Structure

```
├── index.md                 # Home page
├── blog.md                  # Blog listing page
├── _posts/                  # Blog posts (Markdown)
│   ├── 2026-01-08-aws-cdk-infra.md
│   └── 2026-01-07-lambda-best-practices.md
├── _layouts/                # Jekyll templates
│   ├── default.html        # Main layout
│   └── post.html           # Blog post layout
├── _includes/               # Reusable components
│   ├── header.html         # Navigation
│   └── footer.html         # Footer
├── assets/
│   └── css/
│       └── main.css        # All styling
├── _config.yml             # Jekyll configuration
└── README.md               # This file
```

## 🎯 Quick Start

### Writing a Blog Post

Create a new file in `_posts/` with the naming convention: `YYYY-MM-DD-title.md`

```markdown
---
layout: post
title: Your Post Title
date: 2026-01-09
categories: [AWS, DevOps, Cloud]
tags: [lambda, s3, kubernetes]
excerpt: Brief summary of your post
---

Your content here...

<!--more-->

More content after the break...
```

### Building Locally (Optional)

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`

## 🌐 Live Site

Your blog is automatically published at: **https://sheheriyar99.github.io**

Changes are deployed automatically when you push to the `main` branch.

## 🎨 Customization

### Colors
Edit CSS variables in `assets/css/main.css`:
```css
:root {
  --primary: #FF9900;        /* AWS Orange */
  --dark: #232F3E;           /* AWS Dark */
  --light: #F5F5F5;          /* Light Gray */
}
```

### Site Metadata
Update `_config.yml`:
```yaml
title: Your Site Title
description: Your site description
author: Your Name
```

### Navigation
Edit `_includes/header.html` to add/modify navigation links

## 📝 Content Tips

### Blog Post Front Matter
```yaml
---
layout: post
title: Post Title
date: YYYY-MM-DD
categories: [Category1, Category2]
tags: [tag1, tag2, tag3]
excerpt: Short summary (shows in listings)
---
```

### Markdown Features

**Code blocks with syntax highlighting:**
```python
def hello():
    print("Hello, World!")
```

**Lists:**
- Item 1
- Item 2
  - Nested item

**Blockquotes:**
> "A great quote"

## 🔗 Key Sections

- **Home**: Hero section with CTA to apply for AWS Community Builder
- **Blog**: Latest 6 posts with "View All" link
- **All Posts**: Complete blog archive with filtering
- **Individual Posts**: Full post layout with related posts

## 🚀 AWS Community Builder Integration

The site prominently features the AWS Community Builder program:
- Hero section CTA button
- Footer call-to-action section
- Navbar quick link

Users can apply directly via AWS's official page:
https://aws.amazon.com/developer/community/builders/

## 📊 Site Analytics

To add Google Analytics:
1. Add to `_config.yml`:
```yaml
google_analytics: YOUR_TRACKING_ID
```

2. Jekyll will automatically include the tracking code.

## 🛠️ Technical Stack

- **Static Site Generator**: Jekyll
- **Hosting**: GitHub Pages
- **Styling**: Pure CSS (no frameworks)
- **SEO**: jekyll-seo-tag plugin
- **Feeds**: jekyll-feed plugin

## 📝 Writing Tips

1. **Use excerpt_separator**: Add `<!--more-->` to break content
2. **Categories & Tags**: Helps organize and discover posts
3. **Front Matter**: Always include required fields
4. **Markdown**: Keep formatting simple and clean
5. **Code Blocks**: Always specify language for syntax highlighting

## 🎯 Next Steps

1. **Write your first post**: Create a new file in `_posts/`
2. **Customize**: Update colors, fonts, and layout to match your brand
3. **Add social links**: Update footer with your profiles
4. **Share**: Post your blog on social media and communities

## 📞 Support

For Jekyll help: https://jekyllrb.com/
For GitHub Pages: https://pages.github.com/
For AWS Community: https://aws.amazon.com/developer/community/

---

**Happy blogging!** 🎉

