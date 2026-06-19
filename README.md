# My Jekyll Site

A simple, clean Jekyll website hosted on GitHub Pages.

## Quick Start

### Local Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/pythonisaur/myjekyll.git
   cd myjekyll
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   ```

3. **Run the local server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **View your site:**
   Open `http://localhost:4000` in your browser

## Project Structure

```
.
├── _config.yml              # Site configuration
├── _layouts/
│   ├── default.html         # Main layout (header, footer, nav)
│   └── post.html            # Blog post layout
├── _posts/                  # Blog posts (Markdown files)
│   └── 2026-06-19-hello-jekyll.md
├── assets/css/
│   └── main.css             # Stylesheet
├── about.md                 # About page
├── index.html               # Homepage
├── Gemfile                  # Ruby dependencies
└── Gemfile.lock             # Locked dependency versions
```

## How to Update Content

### Update Site Configuration

Edit `_config.yml` to customize your site:

```yaml
title: My Jekyll Site
description: A simple Jekyll website deployed on GitHub Pages
url: "https://yourusername.github.io"
github_username: yourusername
```

### Create a New Blog Post

1. Create a new file in the `_posts/` directory with the naming format: `YYYY-MM-DD-title.md`

   Example: `2026-06-20-my-first-post.md`

2. Add Front Matter (metadata) at the top:

   ```markdown
   ---
   layout: post
   title: "My First Post"
   date: 2026-06-20
   categories: [jekyll, blog]
   author: Your Name
   ---
   
   Your post content in Markdown...
   ```

3. Write your content in Markdown format.

### Update the About Page

Edit `about.md` to customize the About section.

### Customize the Homepage

Edit `index.html` to modify the homepage layout and content.

## How to Deploy

### Step 1: Enable GitHub Pages

1. Go to your repository settings: https://github.com/pythonisaur/myjekyll/settings/pages
2. Under **Source**, select **Deploy from a branch**
3. Choose **main** branch and **/ (root)** folder
4. Click **Save**

GitHub will automatically build and deploy your Jekyll site.

### Step 2: Make Changes and Push

1. **Make your changes locally** (edit posts, update config, etc.)

2. **Test locally:**
   ```bash
   bundle exec jekyll serve
   ```

3. **Stage your changes:**
   ```bash
   git add .
   ```

4. **Commit with a message:**
   ```bash
   git commit -m "Update: Add new blog post"
   ```

5. **Push to GitHub:**
   ```bash
   git push origin main
   ```

6. **Wait for deployment:**
   - GitHub automatically builds and deploys on every push
   - Check the **Actions** tab to see the deployment status
   - Your site updates at: `https://pythonisaur.github.io/myjekyll/`

### Step 3: View Your Live Site

Once deployed, your site is available at:
```
https://pythonisaur.github.io/myjekyll/
```

## Common Tasks

### Add a New Category/Tag

Update your post's Front Matter:
```markdown
---
layout: post
title: "Post Title"
date: 2026-06-20
categories: [category1, category2]
tags: [tag1, tag2]
---
```

### Add an Author

Include in post Front Matter:
```markdown
---
layout: post
title: "Post Title"
author: Author Name
---
```

### Customize Styling

Edit `assets/css/main.css` to change colors, fonts, and layout. The CSS is organized by sections:
- **Reset & Base** - Global styles
- **Header** - Navigation and site title
- **Main Content** - Content area
- **Posts** - Blog post styling
- **Footer** - Footer styling
- **Responsive** - Mobile design

## Troubleshooting

### Site not updating after push?
- Check the **Actions** tab in GitHub for build errors
- Ensure `_config.yml` has the correct `url` and `baseurl`
- Try a hard refresh (Ctrl+Shift+R or Cmd+Shift+R)

### Posts not appearing?
- Verify the filename format: `YYYY-MM-DD-title.md`
- Check that the date in Front Matter is not in the future
- Ensure the file has `layout: post` in Front Matter

### Bundle install fails?
```bash
bundle update
bundle install
```

## Technologies Used

- **Jekyll** - Static site generator
- **Markdown** - Content format
- **Liquid** - Template language
- **GitHub Pages** - Hosting & deployment
- **CSS3** - Styling

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [Liquid Template Language](https://shopify.github.io/liquid/)

## License

This project is open source and available under the MIT License.

---

**Happy blogging!** 🚀
