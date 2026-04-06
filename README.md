# Jacques M. Jean — Professional Portfolio

A clean, professional portfolio website for Jacques M. Jean, featuring insights on AI governance, systems thinking, and organizational advisory work.

## About This Site

This is a custom-built portfolio showcasing professional expertise in AI governance, public policy, advisory services, and strategic engagement. The site is designed to present research, publications, and thought leadership with a focus on clarity and professionalism.

## Tech Stack

- **HTML5** - Semantic markup for accessibility and SEO
- **CSS3** - Custom styling with mobile-responsive design
- **Vanilla JavaScript** - Lightweight interactions, no frameworks
- **Google Fonts** - Playfair Display (headings) and Inter (body)
- **Formspree** - Contact form handling without backend infrastructure

## Deployment on GitHub Pages

This site is designed to be deployed on GitHub Pages with a custom domain.

### Steps to Deploy

1. **Create a GitHub repository** named `Jacquesmjean.com` (or your GitHub username)
2. **Enable GitHub Pages** in the repository settings:
   - Go to Settings > Pages
   - Select `main` branch as the source
   - Save
3. **Push your code** to the repository:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
4. **Verify deployment**: Your site will be available at `https://github.com-username.github.io/Jacquesmjean.com` (or just the username if it's your primary site)

## Custom Domain Setup

To use `jacquesmjean.com` as your custom domain:

### On GitHub

1. In your repository settings (Settings > Pages)
2. Under "Custom domain", enter `jacquesmjean.com`
3. GitHub will automatically create a `CNAME` file (already included in this repo)

### With Your Domain Registrar

1. Update your domain's DNS settings to point to GitHub Pages:
   - **For apex domain** (jacquesmjean.com): Create an A record pointing to GitHub's IP addresses:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **For www subdomain**: Create a CNAME record pointing to `<username>.github.io`

2. Wait for DNS propagation (typically 24 hours)

3. Return to GitHub repository settings and verify the custom domain

### HTTPS/SSL

GitHub Pages automatically provides an HTTPS certificate for your custom domain. After setting the custom domain, GitHub handles the SSL certificate provisioning (may take up to 24 hours).

## Updating Content

### Home Page
Edit `index.html` directly. Update hero section, featured content, and call-to-action elements.

### Pages
Each main page is in `/pages/`:
- `about.html` - Bio and background
- `advisory.html` - Advisory services and expertise
- `governance.html` - AI governance focus
- `insights.html` - Blog and thought leadership
- `flagship-paper.html` - Key publication
- `engagement.html` - Speaking and engagement
- `contact.html` - Contact form

### Blog Posts
Add new posts to `/blog/` directory. Use `sample-post.html` as a template. Create a new file like `my-article.html` and update the insights page to link to it.

### Navigation & Footer
Navigation and footer are present on every page. To update them globally:
1. Edit the nav section in `index.html`
2. Copy the same nav HTML to each page in `/pages/` and `/blog/`
3. Update footer sections consistently

### Contact Form
The contact form on `pages/contact.html` uses Formspree. Update the form's `action` attribute with your Formspree endpoint:
1. Go to [formspree.io](https://formspree.io)
2. Create a new form for your email
3. Copy the form action URL
4. Replace the `action` attribute in the contact form

## Site Structure

```
Jacquesmjean.com/
├── index.html                 # Home page
├── CNAME                      # Custom domain file
├── README.md                  # This file
├── robots.txt                 # SEO: crawler instructions
├── sitemap.xml               # SEO: site map
├── .gitignore                # Git ignore rules
├── css/
│   └── (styles are inline in each HTML file)
├── pages/
│   ├── about.html
│   ├── advisory.html
│   ├── governance.html
│   ├── insights.html
│   ├── flagship-paper.html
│   ├── engagement.html
│   └── contact.html
└── blog/
    └── sample-post.html
```

## Design System

### Colors
- **Navy (Primary)**: `#0F1B4C`
- **White (Background)**: `#FFFFFF`
- **Gold (Accent)**: `#C9A84C`
- **Light Gray (Secondary)**: `#F8F9FA`

### Typography
- **Headings**: Playfair Display (serif)
- **Body**: Inter (sans-serif)

### Responsive Design
All pages use CSS media queries for mobile, tablet, and desktop layouts. The sticky navigation, featured images, and content blocks adapt to smaller screens.

## SEO Configuration

### robots.txt
Allows all crawlers and points to the sitemap.

### sitemap.xml
Auto-generated XML sitemap for search engine indexing. Update with any new pages.

### Meta Tags
Each page includes:
- Title tag (page-specific)
- Description meta tag
- Viewport meta tag for mobile
- Open Graph tags for social sharing (optional)

## Performance Tips

1. **Optimize images**: Use compressed formats (WebP where supported)
2. **Lazy loading**: For blog images, add `loading="lazy"` attribute
3. **Minify CSS/JS**: For production, consider minifying inline styles
4. **Caching headers**: GitHub Pages automatically sets appropriate caching

## Maintenance

- Update navigation links across all pages when adding new sections
- Keep the `sitemap.xml` in sync with new pages
- Test responsive design on mobile before deploying
- Verify all internal links work after restructuring

## License

This portfolio is personal and proprietary. All content, design, and materials are copyright Jacques M. Jean.

## Support

For issues or questions about deployment, refer to [GitHub Pages Documentation](https://docs.github.com/en/pages).
