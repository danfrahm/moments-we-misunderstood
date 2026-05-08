# Moments We Misunderstood — GitHub Pages Site

This folder contains a static landing page designed for GitHub Pages.

## Files

- `index.html` — main landing page text, links, and layout structure
- `styles.css` — visual styling and mobile responsiveness
- `images/` — hero image, moment card images, note image, generated memory-box image, favicon

The call-to-action buttons currently point to this Kit landing page:

https://feathered-hair-and-folded-notes.kit.com/99a3992d9c

## How to publish on GitHub Pages

1. Go to GitHub and create a new repository.
   - Suggested repository name: `moments-we-misunderstood`
   - Make it public unless you have a paid GitHub plan that supports private Pages publishing.

2. Upload the files in this folder.
   - Upload `index.html`, `styles.css`, and the full `images` folder.
   - Do not upload the ZIP file itself as the site contents.

3. Enable GitHub Pages.
   - Open the repository.
   - Go to **Settings** → **Pages**.
   - Under **Build and deployment**, choose **Deploy from a branch**.
   - Branch: `main`
   - Folder: `/root`
   - Click **Save**.

4. Wait a minute or two.
   - GitHub will publish the site at a URL like:
     `https://YOUR-USERNAME.github.io/moments-we-misunderstood/`

5. Test the funnel.
   - Open the GitHub Pages URL on your phone.
   - Click `Explore the Moments`.
   - Click `Follow the Story`.
   - Confirm it opens the Kit page.
   - Submit a test email through Kit.

## How to edit the site

### Change text
Open `index.html` and edit the visible text between the tags.

Examples:

- Hero headline:
  `We didn’t understand these moments while they were happening.`

- Card headline:
  `Some girls already knew how it worked.`

- CTA text:
  `Follow the Story`

### Change images
Replace files inside the `images` folder while keeping the same file names.

For example, to change the hero image, replace:

`images/hero-sleepover.jpg`

with a new image using the same file name.

### Change the Kit link
In `index.html`, search for:

`https://feathered-hair-and-folded-notes.kit.com/99a3992d9c`

Replace it with the new Kit URL.

## GoDaddy custom domain setup

After the GitHub Pages site works, you can point your GoDaddy domain to it.

Typical DNS records:

| Type | Host | Points to |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR-USERNAME.github.io |

Then, in GitHub:

1. Repository → **Settings** → **Pages**
2. Under **Custom domain**, enter your GoDaddy domain.
3. Save.
4. Wait for GitHub to verify the domain and issue HTTPS.

Do not change your GoDaddy `NS` records unless you intentionally move DNS hosting away from GoDaddy.
