# Shivam Kapoor — portfolio site

Static site, no build step. Files:

| File | What it is |
|---|---|
| `index.html` | The whole portfolio (styles, scripts, 3D model and screenshots are inside) |
| `og.jpg` | Link-preview image for LinkedIn, WhatsApp, X |
| `favicon.svg` | Browser tab icon |
| `robots.txt`, `sitemap.xml` | Help Google find and index the site |
| `vercel.json` | Security and caching headers for Vercel |

## Deploy (GitHub + Vercel, recommended)

1. On github.com, create a new **public** repository named `portfolio`.
2. Click **Add file → Upload files**, drag in every file from this folder, and commit.
3. Go to vercel.com, **sign up with GitHub**, then **Add New → Project** and **Import** the `portfolio` repo.
4. Set **Project Name** to `shivam-kapoor`, **Framework Preset** to `Other`, leave the build command empty, and click **Deploy**.
5. Your site is live at `https://shivam-kapoor.vercel.app`.

If Vercel gives you a different address, find-and-replace `shivam-kapoor.vercel.app`
with your real address in `index.html`, `robots.txt` and `sitemap.xml`, then commit again.

Every later commit to GitHub redeploys the site automatically.

## Deploy (command line, alternative)

```bash
# install the Vercel command-line tool
npm i -g vercel
# move into this folder
cd shivam-portfolio-site
# log in to Vercel (opens your browser)
vercel login
# publish the production site
vercel --prod
```

## After it's live

- **Activate the contact form:** send yourself one message from the site, then click the
  activation link FormSubmit emails to 15shivamkapoor@gmail.com. Messages arrive after that.
- **Check the link preview:** paste your URL into LinkedIn's Post Inspector
  (linkedin.com/post-inspector) to refresh and preview the card.
- **Get found on Google (optional):** add the site in Google Search Console and submit
  `https://shivam-kapoor.vercel.app/sitemap.xml`.
- **Custom domain (optional):** Vercel → your project → Settings → Domains.

Inside claude.ai the AI twin answers with Claude and shows the shared leaderboard and live
visitors. On your own domain these switch automatically to the built-in answer engine and
on-device scores; everything else works the same.
