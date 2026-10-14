
# Vishal Chaudhary | Technical GRC & Security Architecture Portfolio

This repository contains the source for Vishal Chaudhary's personal portfolio and article site, published via GitHub Pages. It combines a static portfolio homepage, a blog archive, and a Markdown-based publishing workflow for security, governance, compliance, and architecture content.

## Live site

- Website: https://vishsecurity.github.io/
- Blog archive: https://vishsecurity.github.io/blog.html

## What this project includes

- Responsive portfolio landing page with a polished Apple-inspired aesthetic
- Light and dark theme toggle
- Dynamic blog archive with search and filtering
- Markdown-based article content loaded through the static site
- GitHub Pages friendly setup with no build step required

## Project structure

```text
.
├── index.html
├── blog.html
├── post.html
├── assets/
├── Post/
│   ├── posts.json
│   ├── building-governance.md
│   └── pci-dss-scope-reduction.md
├── README.md
└── .gitignore
```

## Tech stack

- HTML5
- CSS3
- Vanilla JavaScript
- GitHub Pages hosting
- Markdown article content

## Local development

1. Clone the repository:

```bash
git clone https://github.com/vishsecurity/vishsecurity.github.io.git
cd vishsecurity.github.io
```

2. Start a local web server:

```bash
python -m http.server 8000
```

3. Open the site in a browser:

```text
http://localhost:8000
```

> The article loader uses fetch requests, so the site should be served via a local web server rather than opened directly as a file.

## Publishing a new article

The site uses a JSON catalog and Markdown files to render posts.

1. Create a new Markdown file in the `Post/` directory.
2. Add a matching entry to `Post/posts.json`.
3. Use a unique `slug` and set the correct `file` name.
4. Keep the newest items at the top of the array so they appear first on the homepage.

Example entry:

```json
{
  "slug": "cloud-security-baseline",
  "file": "cloud-security-baseline.md",
  "title": "Cloud Security Baseline",
  "tag": "Cloud Security",
  "date": "Oct 2026",
  "summary": "A short description shown on the portfolio."
}
```

The archive page searches by title, tag, and summary, and the homepage can display the newest three articles automatically.

## Customization

- Update the theme colors in the `:root` and `[data-theme="light"]` selectors in the HTML styles.
- Adjust page copy and section content directly in the HTML files.
- Update article metadata in `Post/posts.json` when adding or reordering posts.

## Contact

- Email: vishchaudhary20021994@gmail.com
- LinkedIn: https://www.linkedin.com/in/vishal-chaudhary-224701116/
- YouTube: https://www.youtube.com/@GovernanceGuard
- GitHub: https://github.com/vishsecurity

## License

This project is distributed under the MIT License.
