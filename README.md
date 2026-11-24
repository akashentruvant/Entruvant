# Entruvant website

Static site. No build step. Everything needed is in this folder.

## Files
| File | Purpose |
|---|---|
| index.html | The whole site (Home, The journey, About, Partners, Questions, Book) |
| img/ | Photos and logos (WebP) plus the sharing image og.jpg |
| CNAME | Tells GitHub Pages to serve the site at www.entruvant.com |
| .nojekyll | Stops GitHub processing the files |
| 404.html | Sends any wrong address back to the home page |
| robots.txt, sitemap.xml | For search engines |
| favicon.ico, favicon-32.png, apple-touch-icon.png | Browser tab and phone home screen icons |

## Put it online with GitHub Pages
1. On github.com, create a new repository called `entruvant-website` (Public, or Private on a paid plan).
2. Click **Add file > Upload files**, drag in everything inside this folder (including the hidden `.nojekyll` file), and click **Commit changes**.
3. Go to **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, and click **Save**.
4. In the same page, under **Custom domain**, enter `www.entruvant.com` and click **Save**.
5. At the domain registrar for entruvant.com, add these DNS records:
   - `CNAME` record: host `www`, value `YOUR-GITHUB-USERNAME.github.io`
   - `A` records: host `@`, values `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
6. Wait for DNS to update (minutes to a few hours), then tick **Enforce HTTPS** in Settings > Pages.

## Updating the site later
Upload the changed files over the old ones and commit. The site updates within a minute or two.

## Checks after going live
- Click **Begin your Legacy Snapshot** and confirm Heath's Google calendar loads inside the panel.
- Try the language switcher (the globe in the header).
- Share the link in a message to confirm the preview image shows.

Contact: Heath Stone, heath@entruvant.com, +1 (604) 340-7188
