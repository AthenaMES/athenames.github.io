# Athena Manufacturing Intelligence website

The marketing website for Athena, with a blog and case studies.

| What | Where |
| --- | --- |
| Home page | `index.html` |
| Blog list | `blog/index.html` |
| Articles | `_posts/` |
| Case studies | `_case_studies/` (the template is hidden until `published: true`) |
| Blog look and layout | `_layouts/`, `_includes/`, `assets/css/blog.css` |
| Logo, icons, share image | `assets/img/` |
| Images for articles | `assets/images/posts/` |
| Site settings (web address) | `_config.yml` |
| Private blog editor settings | `.pages.yml` |

- **Go live:** see `HOSTING.md`.
- **Write an article or case study:** see `BLOGGING.md`.

Contact details shown on the site (name, phone, email, hours) are set at the top of the script in `index.html`, in the `CONTACT` block.

Built on Jekyll, which GitHub Pages runs for you. Plugins used: jekyll-seo-tag, jekyll-sitemap, jekyll-feed (all supported by GitHub Pages).
