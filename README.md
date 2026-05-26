# Salus

Deploy your static HTML site by uploading a `.zip` archive as a GitHub Release asset.

## Upload archive flow

1. Create a release in this repository.
2. Attach a `.zip` file named `site.zip` that contains your site files (`index.html`, assets, etc.).
3. Publish the release.

The workflow at `.github/workflows/deploy-release-archive.yml` will:
- download `site.zip` from that release,
- extract it,
- deploy it to GitHub Pages.