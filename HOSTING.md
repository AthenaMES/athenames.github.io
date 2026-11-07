# Put the Athena website live with GitHub Pages

GitHub Pages hosts the site for free and builds the blog for you. You do not need to install anything on your computer.

## 1. Create the repository

1. Sign in at github.com (or create a free account).
2. Click **+** at the top right, then **New repository**.
3. Name it, for example `athena-website`.
4. Choose **Public**. GitHub Pages is free for public repositories; a private repository needs a paid GitHub plan (Pro, Team or Enterprise).
5. Click **Create repository**.

## 2. Upload the files

1. Unzip `athena-website.zip` on your computer.
2. In the new repository, click **uploading an existing file** (or **Add file → Upload files**).
3. Open the unzipped folder, select **everything inside it** (not the folder itself) and drag it into the browser.
4. Hidden files: make sure `.pages.yml` is included. On a Mac press `Cmd + Shift + .` in Finder to show hidden files; on Windows turn on **View → Show → Hidden items**.
5. Click **Commit changes**.

## 3. Turn on GitHub Pages

1. In the repository, open **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose branch **main** and folder **/ (root)**, then click **Save**.
4. Wait 1 to 3 minutes. Open the **Actions** tab to watch the build; a green tick means it is live.
5. Your site is at `https://YOUR-USERNAME.github.io/athena-website/`.

## 4. Use your own domain (recommended)

With your own domain, every link and image works as it is. Example: `www.athena-mes.com` or `athena.nmtgindia.com`.

1. **Settings → Pages → Custom domain**: type the domain and click **Save**. GitHub adds a `CNAME` file to the repository.
2. At your domain provider (GoDaddy, Hostinger, Cloudflare and so on), add DNS records:
   - For a subdomain such as `www` or `athena`: a **CNAME** record pointing to `YOUR-USERNAME.github.io`
   - For the bare domain (`athena-mes.com`): four **A** records:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. When the check passes, tick **Enforce HTTPS** (it can take up to 24 hours to appear).
4. Open `_config.yml` in the repository (click it, then the pencil icon) and set:
   - `url: "https://your-domain"` (no slash at the end)
   - `baseurl: ""`
   Click **Commit changes**.

**No custom domain yet?** Set `url: "https://YOUR-USERNAME.github.io"` and `baseurl: "/athena-website"` in `_config.yml`. The home page and blog work, but images you add inside the text of an article may not show until you move to your own domain.

## 5. Tell Google about the site

1. Open search.google.com/search-console and add your domain.
2. Verify it (the DNS method works with GitHub Pages).
3. Under **Sitemaps**, submit `sitemap.xml`. The site creates it automatically and updates it with every new article.

## What builds automatically

- `sitemap.xml`: every page, article and published case study, for Google
- `blog/feed.xml`: a feed of articles
- Page titles, descriptions, share images and structured data on every page
- `robots.txt` pointing search engines to the sitemap

## Changing the website later

Edit `index.html` in GitHub (pencil icon) and commit. The live site updates in about a minute.
