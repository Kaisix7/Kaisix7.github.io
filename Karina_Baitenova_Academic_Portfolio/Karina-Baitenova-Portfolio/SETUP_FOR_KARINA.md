# Put this site on your own GitHub Pages account

This is your starter site. You do not need to copy anyone else's bio, projects, photograph, or publication list. The pages have already been rewritten around your own plan. Read them once and change anything that does not sound like you.

## 1. Replace your portrait

Use a square or portrait-oriented JPG photograph. Rename it **exactly** to `prof_pic.jpg` and copy it to:

`assets/img/prof_pic.jpg`

The ZIP includes a generic placeholder image so the site can render without showing another person's face. Replace it before publishing. Keep the same filename and lower-case extension.

## 2. Create a repository

Sign in to [your GitHub account](https://github.com/Kaisix7). Click **+** > **New repository**.

Repository name: `Kaisix7.github.io` (GitHub matching is case-insensitive; the address will be `https://kaisix7.github.io/`). Set visibility to **Public**. Do not create an initial README because this ZIP already contains one.

## 3. Upload these files

**Extract the ZIP on your computer first.** Do not upload the ZIP file itself to GitHub and expect Pages to unpack it. Open the extracted `Karina-Baitenova-Portfolio` folder, then copy all the files and subfolders, including `.github` and `.gitignore`.

In the new repository click **uploading an existing file** or **Add file > Upload files**. Drag the *contents* of the extracted folder into the upload area, not the enclosing folder. Confirm `_config.yml` and `about.md` appear at the repository root. Commit to `main`.

For easier uploading, open a GitHub Codespace for the empty repository, unzip the package using the terminal, and copy hidden directories as well:

```bash
unzip Karina-Baitenova-Portfolio.zip -d /tmp/karina-site
cp -a /tmp/karina-site/Karina-Baitenova-Portfolio/. .
git add .
git commit -m "Set up personal portfolio"
git push origin main
```

If a ZIP is uploaded to Codespaces, you can use the VS Code Explorer to move it into the repository before running those commands. **The ZIP is not itself the website.**

## 4. Configure GitHub Pages

Open **Settings > Pages** in your repository. Under **Build and deployment**, choose **GitHub Actions**.

The included `.github/workflows/jekyll.yml` will install Ruby dependencies, build Jekyll, and deploy `_site`. Check the **Actions** tab. When the workflow succeeds, visit `https://kaisix7.github.io/`.

## 5. Local preview

Use GitHub Codespaces or a computer with Ruby and Bundler:

```bash
bundle install
bundle exec jekyll doctor
bundle exec jekyll build --trace
bundle exec jekyll serve --host 0.0.0.0 --port 4000 --force_polling --watch
```

Open port 4000 in Codespaces. Do not open source `.md` files directly in the browser.

## 6. Things to check

- About appears only once in the navigation.
- Blog, Projects, Research, Publications, Code, and CV open correctly.
- Dark mode works and the layout responds to mobile screen widths.
- Your photo and the KB favicon appear.
- The copyright line appears once.
- Your GitHub, ResearchGate, and ORCID links are correct.
- No other person's biography, email, or academic achievements appear.
- Projects marked *in development* are still actually in development.

## 7. Before applying to graduate school

The `GRADUATE_ROADMAP.md` and `RESEARCH_PLAN.md` files are planning documents. They are not proof of offers, current faculty openings, publications, or funding. Verify programs and potential supervisors on official university websites before contacting them.

## 8. One technical warning

The original site had a Jekyll Sass compilation error caused by `@import "main";` inside its own `main.scss`. Do not add that self-import. This package uses the original theme Sass module layout and retains a targeted navigation fix. The theme dependencies are pinned to avoid unexpected upgrades.

The package was checked for YAML/front-matter formatting and structure, but Ruby gems cannot be installed in this offline packaging environment. The GitHub Actions build is the final compatibility check. If any dependency breaks, keep the theme and ask for a minimal fix rather than replacing it.
