# Jason (Feng) Guo — Academic Homepage

A simple, fast, GitHub-Pages-hosted academic site styled after
[Hanzhe Zhang's homepage](https://hanzhezhang.github.io/).
Pure HTML + one CSS file. No build step. No frameworks.

## File Structure

```
jason-site/
├── index.html              # Home page (bio, photo, news)
├── style.css               # Shared stylesheet
├── research/
│   └── index.html          # Publications + working papers
├── teaching/
│   └── index.html          # Course history
└── files/
    ├── profile.jpg         # YOUR PHOTO — REPLACE THIS
    └── CV_JasonGuo.pdf     # YOUR CV — ADD THIS
```

## Before You Deploy: Things to Customize

These are placeholders in the HTML files — find and replace before pushing.

1. **Profile photo** — Save your headshot as `files/profile.jpg`
   (or update the `<img src=...>` path in `index.html`).
2. **CV** — Save your CV as `files/CV_JasonGuo.pdf`.
3. **Google Scholar link** — In `index.html` and `research/index.html`,
   replace `YOUR_ID` in
   `https://scholar.google.com/citations?user=YOUR_ID` with your actual ID.
4. **SSRN link** — Same idea, replace `YOUR_ID` in the SSRN URLs.
5. **GitHub username** — In the footer of `index.html`, replace `YOUR_USERNAME`.
6. **News section** — On `index.html`, the News list has placeholders.
   Hanzhe's site uses these conventions:
   - 📖 publication / paper update
   - 🔈 talk, announcement, visit
   - 🏆 award or honor
   - 💰 grant or funding

## How to Deploy on GitHub Pages (Windows)

### Step 1 — Create a GitHub repo

GitHub Pages will serve a personal site for free if your repository is named
exactly `<username>.github.io`. For example, if your GitHub username is
`jasonfengguo`, name the repo `jasonfengguo.github.io`.

1. Go to <https://github.com/new>.
2. **Repository name:** `<your-username>.github.io` (lowercase, exact).
3. **Visibility:** Public.
4. Don't add a README, .gitignore, or license (you'll push files in the next step).
5. Click **Create repository**.

### Step 2 — Push the files (using GitHub Desktop, easiest on Windows)

1. Install [GitHub Desktop](https://desktop.github.com/) and sign in.
2. **File → Clone repository →** pick the repo you just created.
   Choose a local folder (e.g., `C:\Users\Jason\Documents\GitHub\`).
3. Open that folder in File Explorer. Copy all the files from this `jason-site/`
   folder INTO it (so `index.html` is at the top level of the repo).
4. Add `profile.jpg` and `CV_JasonGuo.pdf` to the `files/` subfolder.
5. Back in GitHub Desktop, you'll see all the changes. Type a commit message
   like "Initial site" and click **Commit to main**, then **Push origin**.

### Step 3 — (Usually automatic) Turn on Pages

For a `<username>.github.io` repo, GitHub Pages turns on automatically.
To verify:

1. On GitHub.com, go to your repo → **Settings** → **Pages**.
2. **Source** should be `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Wait 1–2 minutes, then visit `https://<your-username>.github.io`.

### Step 4 — Update later

Edit the `.html` files locally. In GitHub Desktop, commit the changes and push.
Your site refreshes within a minute or two.

## Optional: Custom Domain

If you own a domain (e.g., `jasonguo.com`):

1. In your repo, create a file named `CNAME` (no extension) with one line:
   `jasonguo.com`.
2. At your domain registrar, add a CNAME DNS record pointing to
   `<username>.github.io`.
3. In **Settings → Pages**, enter the custom domain and tick **Enforce HTTPS**.

## Notes on the Design

- Single CSS file, ~100 lines. Edit `style.css` to change colors, fonts, widths.
- Default link color is classic academic blue. Change it in `style.css` if you
  prefer black or another color.
- The home page uses a flex layout: bio on the left, photo on the right.
  On mobile (≤700px), the photo moves above the text.
- All content was migrated from your existing Google Site
  (<https://sites.google.com/view/jason-feng-guo/>) — proofread before
  going live in case anything has changed.
