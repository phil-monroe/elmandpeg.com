# Elm and Peg Consulting — Website

Static site for [elmandpeg.com](https://elmandpeg.com), hosted via GitHub Pages.

## Structure

```
.
├── index.html          # Main landing page
├── assets/
│   └── logo.png        # Brand logo
├── CNAME               # Custom domain for GitHub Pages
└── .nojekyll           # Disables Jekyll processing
```

## Hosting on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages** in the repository.
3. Under **Branch**, select `main` and `/ (root)`, then click **Save**.
4. In your domain registrar's DNS settings, add the following records pointing to GitHub Pages:

   | Type  | Name | Value                   |
   |-------|------|-------------------------|
   | A     | @    | 185.199.108.153         |
   | A     | @    | 185.199.109.153         |
   | A     | @    | 185.199.110.153         |
   | A     | @    | 185.199.111.153         |
   | CNAME | www  | `<your-github-username>.github.io` |

5. GitHub Pages will automatically provision an SSL certificate once DNS propagates (may take up to 48 hours).

## Local Preview

Open `index.html` directly in a browser, or run a simple local server:

```bash
npx serve .
# or
python3 -m http.server
```
