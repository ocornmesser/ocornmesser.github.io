# Owen Cornmesser Personal Website

Static personal academic website designed for GitHub Pages. It follows the same general pattern as the reference sites:

- A clear academic homepage with a navigation bar
- About, research areas, news, selected publications, projects, teaching, and contact sections
- No local build step
- Plain HTML, CSS, and JavaScript

## GitHub Setup Steps

Use a user site if this will be your main personal website.

1. Sign in to GitHub.
2. Click the `+` button in the top-right corner.
3. Click `New repository`.
4. Set `Owner` to your personal GitHub account.
5. Name the repository exactly `USERNAME.github.io`, replacing `USERNAME` with your GitHub username in lowercase.
6. Set visibility to `Public`.
7. Leave `Add a README file` unchecked if you are pushing this local folder.
8. Click `Create repository`.
9. In a terminal opened in this folder, run:

   ```bash
   git init
   git branch -M main
   git add .
   git commit -m "Initial personal website"
   git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
   git push -u origin main
   ```

10. In the GitHub repository, open `Settings`.
11. In the left sidebar, click `Pages`.
12. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
13. Set `Branch` to `main` and folder to `/root`.
14. Click `Save`.
15. Wait a few minutes, then open `https://USERNAME.github.io/`.

GitHub may automatically configure Pages for a repository named `USERNAME.github.io`, but checking `Settings > Pages` is still worth doing.

## Local Note

This folder appears to live inside a larger existing Git working tree. If you want this website to be its own clean repository, run the commands above from this exact folder. A nested `.git` directory will make this folder independent from the parent repository.

## Updating the Live Site

After editing files locally, publish the changes to GitHub Pages with:

```bash
git add .
git commit -m "Update website content"
git push
```

GitHub Pages usually republishes within a few minutes.

## What To Customize Next

Edit `index.html` and replace:

- News items as your work changes
- Publication statuses as papers move from under review to accepted or published
- Research and project summaries as repositories or papers become public
- The profile image once you have a photo you want to use

Replace `assets/img/profile-placeholder.svg` with a real profile photo when ready. Keep the filename the same or update the `src` in `index.html`.

## Files

- `index.html`: main website
- `cv.html`: editable web CV
- `software/index.html`: software projects page available at `/software/`
- `files/CurriculumVitae.pdf`: PDF CV linked from the site
- `assets/css/styles.css`: layout and visual styling
- `assets/js/site.js`: mobile navigation, icons, active section state, and footer year
- `assets/img/research-grid-banner.png`: generated visual banner
- `assets/img/profile-placeholder.svg`: temporary profile image
- `.nojekyll`: tells GitHub Pages to publish the static files directly
- `404.html`: simple not-found page

## References

- PIC Lab: https://pic-lab.github.io/
- Luke Lowery: https://lukelowry.github.io/
- GitHub Pages docs: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
