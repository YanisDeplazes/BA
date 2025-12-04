# Project Name

This is a github template for school projects.

## Installation

Create and activate a virtual environment (recommended), then install all dependencies:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Project Structure

All project documentation lives in the `docs/` directory:

```
├── docs/
```

## Documentation Development

To preview the documentation locally with MkDocs, run:

```bash
mkdocs serve
```

The documentation site will be available at [http://127.0.0.1:8000](http://127.0.0.1:8000).

### MkDocs Configuration Notes

Update mkdocs.yml with your project details;

```yaml
site_name: Project Name # Change to your project title
site_description: Project Description # Change to your project description
site_author: Yanis Deplazes
```

## Deployment Notes

This template uses GitHub Actions to deploy MkDocs to GitHub Pages. Before deploying, make sure to:

1. **Add your GitHub token** as a secret named `TOKEN` in your repository settings.
2. **Update the custom domain** in `deployment.yml` by replacing `<NAME>` with your chosen subdomain, e.g.:

```yaml
echo "projectname.yanis.io" > public/CNAME
```
