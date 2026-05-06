# Portfolio

**Live site: <https://rubenayla.xyz/>**

Personal portfolio site built with MkDocs Material showcasing my projects and work.

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/rubenayla/portfolio.git
cd portfolio
```

2. Install dependencies (uv will automatically create a virtual environment):
```bash
uv sync
```

3. Run local server:
```bash
uv run mkdocs serve
```

Visit `http://127.0.0.1:8000` to view the site.

## Deployment

The site is automatically deployed to GitHub Pages via GitHub Actions on every push to `main`.

### Setup GitHub Pages

1. Go to your repository Settings > Pages
2. Under "Build and deployment", select "GitHub Actions" as the source
3. Push to main branch to trigger deployment

## Structure

```
portfolio/
├─ docs/
│  ├─ index.md               # Homepage
│  ├─ projects/              # Project pages
│  │  ├─ kart.md
│  │  ├─ cyberwheel.md
│  │  └─ satellites.md
│  └─ about.md               # About page
├─ mkdocs.yml                # MkDocs configuration
├─ pyproject.toml            # Project dependencies
└─ .github/workflows/        # GitHub Actions
```

## Adding Content

### Images

Place images in `docs/images/` and reference them in markdown:
```markdown
![Alt text](../images/your-image.jpg)
```

### New Projects

1. Create a new markdown file in `docs/projects/`
2. Add it to the `nav` section in `mkdocs.yml`

## License

This project is open source and available under the MIT License.
