# Sondgeroth Fit Website

Static site for [sondgerothfit.com](https://sondgerothfit.com), hosted on GitHub Pages.

## Structure

```
index.html                  Home page (hero, about, testimonials, programs, contact)
services/index.html         Services page (all coaching options)
privacy-policy/index.html   Privacy policy
CNAME                       Custom domain configuration
ruck.jpg                    Hero background image
ben-profile.jpg             Profile photo
training-bw.jpg             Training image
```

## Pages

| URL | File | Description |
|-----|------|-------------|
| `/` | `index.html` | Home — hero, about Ben, testimonials, programs overview, contact |
| `/services` | `services/index.html` | Full services list with descriptions |
| `/privacy-policy` | `privacy-policy/index.html` | App privacy policy |

External links (not hosted here):
- **Get Started** -> Typeform onboarding form
- **App** -> Apple App Store

## Deployment

Hosted via **GitHub Pages** from the `main` branch (root).

- **Custom domain:** sondgerothfit.com
- **DNS:** Configure A records or CNAME per [GitHub Pages docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)
- **No build step** — pure static HTML/CSS, no JavaScript

### Push via HTTPS

```bash
gh auth login
git push -u origin main
```

## Local Preview

Open `index.html` directly in a browser — no server required. For sub-pages, use a local server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
