# Week 1 — Website Development

**Goal:** Create a documentation website using GitHub Pages, Markdown, and MkDocs.

!!! warning "Evidence pending"
    The procedure below describes the website setup. Screenshots and observations should be added after the steps have been performed; they have not been invented.

## 1. Understanding the tools

| Tool | Function |
| --- | --- |
| Git | Records file changes and versions |
| GitHub | Hosts the project repository |
| GitHub Pages | Serves a public website |
| Obsidian | Edits Markdown documentation |
| MkDocs | Converts Markdown into static HTML |
| Material for MkDocs | Provides navigation, search and styling |

## 2. Choosing MkDocs

MkDocs suits documentation websites because it uses readable Markdown files. The Material theme supplies responsive navigation, search, and light/dark modes. The source is separate from the published HTML, which is generated automatically.

## 3. Repository structure

```text
digital-fabrication/
├── .github/workflows/deploy.yml
├── docs/
│   ├── index.md
│   ├── about.md
│   ├── week-1.md
│   ├── projects.md
│   └── resources.md
├── mkdocs.yml
└── requirements.txt
```

The `docs` folder contains Markdown documents. `mkdocs.yml` defines the website theme and navigation. The GitHub Actions workflow builds the site.

## 4. Publication procedure

1. Create a public GitHub repository named `digital-fabrication`.
2. Add the MkDocs configuration, Markdown pages, and GitHub Actions workflow.
3. Open **Actions** and check whether **Deploy MkDocs to GitHub Pages** completes successfully.
4. In **Settings → Pages**, select **Deploy from a branch**, `gh-pages`, and `/ (root)`.
5. Visit [the final website](https://gaminghub492.github.io/digital-fabrication/).

```text
Markdown → GitHub commit → GitHub Actions → MkDocs build
→ gh-pages branch → published website
```

## 5. Using Obsidian

Install [Obsidian](https://obsidian.md/), download the repository, and open the `docs` directory as a vault. Edit a Markdown document and save it. Commit and push the changes to update the site.

## 6. Optional local preview

With Python installed, run from the repository directory:

```powershell
python -m pip install -r requirements.txt
python -m mkdocs serve
```

Open `http://127.0.0.1:8000/`.

Other useful Git commands:

```powershell
git status
git add .
git commit -m "Update documentation"
git push
```

## 7. Evidence and reflection

- [ ] Create the GitHub repository and capture a screenshot.
- [ ] Upload the source and show the repository structure.
- [ ] Confirm successful deployment and capture a screenshot.
- [ ] Visit and screenshot the live website.
- [ ] Install Obsidian and open the Markdown documents.
- [ ] Edit a document, save it, and record the result.
- [ ] Explain any errors and how they were solved.

### Reflection prompts

**What worked?** Explain the steps you completed and how you verified them.

**What problems occurred?** Record errors, their causes, and the fixes you used.

**What did I learn?** Describe how version control, Markdown, static-site generation, and hosting work together.

See [Resources](resources.md) for the course materials.
