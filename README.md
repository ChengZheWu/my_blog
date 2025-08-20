# Create a Blog with Tailwind Next.js Starter Blog

This guide explains how to set up a blog website using the [Tailwind Next.js Starter Blog](https://github.com/timlrx/tailwind-nextjs-starter-blog). It provides a robust starting point for creating a content-focused blog using modern tools like Next.js, Tailwind CSS, and MDX.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/timlrx/tailwind-nextjs-starter-blog.git my-blog
cd my-blog
```

### 2. Install Dependencies

Make sure you have Node.js and npm installed, then run:
Office Website: https://nodejs.org/zh-tw

```bash
npm install
```

### 3. Run the Development Server

```bash
npm run dev
```

Visit `http://localhost:3000` in your browser to view the blog locally.

## Customize Your Blog

You can personalize your blog in the following ways:

### Edit Site Metadata

Update the file:

```
data/siteMetadata.js
```

Change the blog title, description, author, language, and more.

### Write Blog Posts

Create blog posts in:

```
data/blog/*.mdx
```

Each `.mdx` file is a blog post. You can use front matter for metadata and Markdown + JSX for content.

### Styling

- Tailwind CSS is already configured.
- You can override styles in `styles/globals.css` or customize the Tailwind config in `tailwind.config.js`.

### Dark Mode

Built-in dark mode toggle using `next-themes`. It works out-of-the-box.

### Search (Optional)

Local search is enabled by default using `Fuse.js` or `FlexSearch` (depending on config).

## Deployment

Deploy to Vercel

### 1. Push Your Project to GitHub

Make sure your project is version-controlled and pushed to GitHub:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/your-username/my-blog.git
git push -u origin main
```

Replace `your-username` with your GitHub account name.

---

### 2. Log in to Vercel

1. Visit [https://vercel.com](https://vercel.com)
2. Sign up or log in using your **GitHub** account
3. Authorize Vercel to access your GitHub repositories

---

### 3. Import Project to Vercel

1. Click **"Add New → Project"**
2. Find and select your `my-blog` repo
3. Click **Import**

---

### 4. Configure Build Settings

Usually Vercel auto-detects settings, but confirm:

| Option           | Value                 |
| ---------------- | --------------------- |
| Framework        | Next.js               |
| Build Command    | `npm run build`       |
| Output Directory | `.next` (default)     |
| Root Directory   | `/` if app is in root |

Click **Deploy**.

---

### 5. Deployment Complete

- Vercel will build and deploy the site
- A public URL will be created like: https://myblog-alpha-umber.vercel.app/ (This is my blog)
- Future commits to GitHub will **auto-redeploy**

## Advanced Features

Blog

- Tag support and tag pages
- Pagination for long post lists
- Custom 404 page (`pages/404.js`)
- RSS feed, sitemap, and SEO config in `next-seo.config.js`
- Author pages (`data/authors/`)

Vercel

- Add Environment Variables
- Add Custom Domain

## Optional Integrations

- Google Analytics (via environment variable `NEXT_PUBLIC_GOOGLE_ANALYTICS`)
- Plausible, Umami, or other providers
- Comment systems like Giscus or Disqus

## Notes

This project was built as a side project to practice software development and document my learning journey.  
Some parts of the code were assisted by AI tools (e.g., ChatGPT) to help with coding, debugging, and optimization.  
All code has been reviewed and adapted to fit the goals of this project.

## 📄 License

[MIT](https://github.com/timlrx/tailwind-nextjs-starter-blog/blob/main/LICENSE) © [Andy Wu](https://myblog-alpha-umber.vercel.app/)
