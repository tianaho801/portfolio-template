# Portfolio Template (Quarto + GitHub Pages)

## Setup

1. Click **Use this template** -> **Create a new repository**.
   Name it `yourusername.github.io` (exactly your GitHub username) and set it to **Public**.
2. Open [Posit Cloud](https://posit.cloud) -> **New Project** -> **New Project from Git Repository** -> paste your new repo's HTTPS URL.
3. In the **Terminal** tab, run once:
   ```
   git config --global user.name "Your Name"
   git config --global user.email "you@email.com"
   ```
4. Edit `_quarto.yml`, `index.qmd`, `about.qmd`, `project1.qmd`, `project2.qmd`.
   Replace `images/profile.jpg` with your own photo (same name, or update the path).
5. Click **Render**.
6. Git panel: check all files -> **Commit** -> **Push**.
   When asked for a password, paste your GitHub **personal access token**.
7. On GitHub: **Settings -> Pages -> Deploy from a branch -> `main` -> `/docs` -> Save**.
8. Wait 2-5 minutes. Your site is live at `https://yourusername.github.io`.

## Making a token

GitHub -> Settings -> Developer settings -> Personal access tokens -> Tokens (classic) -> Generate new token. Tick the `repo` scope. Copy it right away; GitHub shows it once.

## Common errors

- YAML uses **spaces, never tabs**. Indentation matters.
- Keep `.qmd` files in the **root folder**, not subfolders.
- Image filenames are **case-sensitive** (`IMG_1.JPG` is not `img_1.jpg`).
- If R code fails: `install.packages(c("knitr", "rmarkdown"))`.
- **Render before you push**, or the live site will not update.
- Do not delete the `docs/` folder or `docs/.nojekyll`.
