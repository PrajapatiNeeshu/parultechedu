# UP TGT PGT Study Portal

A content-first study portal for UP TGT and UP PGT exam preparation, built with MkDocs Material and ready for GitHub Pages.

## What is included

- Exam guides for UP TGT and UP PGT
- Syllabus checklists and subject maps
- Chapter note templates
- Subject-wise MCQ templates
- Job update tables for vacancies, admit cards, answer keys, and results
- Online test and mock-test trackers
- Resource lists for books, channels, websites, and previous papers
- GitHub Actions deployment to GitHub Pages

## Run locally

Make sure Python 3.9 or newer is installed, then run these commands from this folder:

```powershell
python -m venv venv
venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m mkdocs serve
```

Open <http://127.0.0.1:8000> in your browser. Stop the server with `Ctrl+C`.

## Create content

1. Add a Markdown file under `docs/`.
2. Follow the nearest existing template.
3. Add the page to `nav` in `mkdocs.yml` when it should appear in the menu.
4. Run `python -m mkdocs build --strict` before publishing.

For notes, keep one chapter or concept per page. For current updates, always include an official source URL and the date last verified.

## Publish with GitHub Pages

1. Create a GitHub repository and push this project to its `main` branch.
2. Replace `YOUR_USERNAME` in `mkdocs.yml` with your GitHub username.
3. In the repository settings, set Pages to use the GitHub Actions source if required by your organization.
4. Push changes to `main`. `.github/workflows/deploy.yml` publishes the site automatically.

You can also publish manually with:

```powershell
python -m mkdocs gh-deploy --force
```

## Project layout

```text
docs/                 Markdown content
mkdocs.yml            Site configuration and navigation
requirements.txt      Python dependencies
.github/workflows/    GitHub Pages deployment
```

Always verify recruitment information against the official authority website before sharing it with learners.
