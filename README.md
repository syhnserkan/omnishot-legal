# Omnishot Legal Pages

Static legal pages for [Omnishot](https://apps.apple.com/app/omnishot) — hosted on GitHub Pages.

## Pages

| File | URL | Description |
|------|-----|-------------|
| `index.html` | `/` | Landing page linking to both documents |
| `privacy.html` | `/privacy.html` | Privacy Policy |
| `terms.html` | `/terms.html` | Terms of Service |

## Languages

All pages support **English** (default) and **Turkish**.

- Language is auto-detected from the browser (`navigator.language`)
- Users can switch manually via the EN / TR toggle on every page
- Language selection carries over between pages via the `?lang=` query parameter

## Deployment (GitHub Pages)

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Save — your site will be live at:

```
https://<username>.github.io/<repo>/
https://<username>.github.io/<repo>/privacy.html
https://<username>.github.io/<repo>/terms.html
```

## Updating Content

- **Email / contact**: search and replace `support@omnishot.app` across all `.html` files
- **Last updated date**: update the `updated` string in both the HTML default text and the `content` JS object inside each file (both `en` and `tr` keys)
- **New section**: add the HTML element with an `id`, then add matching keys to both language objects in the `<script>` block

## Contact

support@omnishot.app
