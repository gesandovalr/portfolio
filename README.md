# German Sandoval — Infrastructure, Cloud & Automation Portfolio

Bilingual English/Spanish static portfolio website prepared for GitHub Pages.

## Files

- `index.html` — main website
- `styles.css` — responsive styling
- `script.js` — mobile navigation and dynamic year
- `.nojekyll` — prevents GitHub Pages/Jekyll from altering the static site

## Before publishing

Edit `index.html` and replace:

- `your-email@example.com`
- `https://www.linkedin.com/`
- `https://github.com/`

with your real contact and profile URLs.

## Publish with GitHub Pages

1. Create a new repository, for example `portfolio`.
2. Upload all files from this folder to the repository root.
3. Commit and push.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select:
   - Branch: `main`
   - Folder: `/ (root)`
7. Save.

GitHub will provide a URL similar to:

`https://YOUR-USERNAME.github.io/portfolio/`

## Use a custom domain

Create a file called `CNAME` in the repository root containing only your domain, for example:

`germansandoval.com`

Then configure the DNS records with your domain provider according to GitHub Pages documentation.

## Suggested positioning

**Infrastructure, Cloud & Automation Consultant**

> Helping companies automate, modernize and secure infrastructure across on-premises and cloud environments.

## Notes

The site deliberately positions services around business outcomes such as reliability, repeatability, recovery and reduced operational risk instead of presenting a simple list of tools.


## Bilingual language switcher

The site includes an **EN / ES** language selector in the navigation.

- The page changes language instantly without reloading.
- The selected language is stored in `localStorage`.
- On the first visit, Spanish is selected automatically when the browser language starts with `es`; otherwise English is used.
- The HTML `<html lang="">`, page title and meta description are updated dynamically.
- No external translation API is required.


## Back-to-top fix

The footer control is now a real button instead of an anchor link.

It uses JavaScript to scroll to the absolute top of the page and does not add `#top` to the URL.


## Back-to-top link

The footer uses the original link-style **Back to top / Volver arriba** control.

- It points to `#top`.
- The header is explicitly marked with `id="top"`.
- JavaScript adds smooth scrolling while keeping the URL clean.
- If JavaScript is unavailable, the native `href="#top"` fallback still works.
