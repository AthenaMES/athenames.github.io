# Writing articles and case studies

Everyone can **read** the blog, which is what you want for Google. Only people with access to this GitHub repository can **publish**. Today that is only you.

## Option A: the private editor (easiest)

Pages CMS gives you a simple editor in the browser, with a text editor, image upload and a Publish button.

1. Open **app.pagescms.org** and click **Sign in with GitHub**.
2. Install the Pages CMS GitHub App when asked, and allow it to use **only** the `athena-website` repository.
3. Open the repository. You will see **Blog articles** and **Case studies** in the left menu (they come from `.pages.yml`).
4. Click **Add an entry**, fill in the title, the summary for Google, the date and the cover image, write the article, then click **Save**.
5. The site rebuilds by itself. The article is live at `/blog/your-title/` in 1 to 3 minutes.

**Case studies** start hidden (**Show on the website** is off). Switch it on only when the facts are final and the customer has agreed in writing.

## Option B: straight in GitHub

1. Open the `_posts` folder in the repository and click **Add file → Create new file**.
2. Name it `YYYY-MM-DD-short-title.md`, for example `2026-11-20-how-to-plan-vendor-stages.md`.
3. Copy the top block (between the `---` lines) from the sample article, change it, and write the article below in Markdown.
4. Click **Commit changes**.

Images: open `assets/images/posts`, click **Add file → Upload files**, then use `/assets/images/posts/your-image.jpg` in the article.

For a case study, copy `_case_studies/2026-11-07-case-study-template.md`, give it a new name, fill it in and set `published: true`.

## Keep it to you only

- Do not add collaborators under **Settings → Collaborators** unless you want them to publish.
- Pages CMS can also invite editors by email. Only do this for people who should publish.
- Turn on two-factor sign-in for your GitHub account (**Settings → Password and authentication**).

## Writing for Google, in short

- One topic per article. Put the main phrase in the title, for example "stage-wise planning for machine shops".
- Write the summary (about 150 characters) as if it were the line under the title on Google.
- Use headings (H2) for each part, and link to the home page sections (`/#modules`, `/#demo`).
- Cover image 1200 x 630 pixels, with a short description.
- Publish regularly, for example two articles a month, and one case study each quarter.
