# Salus

Deploy your static HTML site by uploading a `.zip` archive as a GitHub Release asset.

## Upload archive flow

1. Create a release in this repository.
2. Attach a `.zip` file that contains your site files (`index.html`, assets, etc.).
3. Publish the release.

The workflow at `/home/runner/work/Salus/Salus/.github/workflows/deploy-release-archive.yml` will:
- download the first `.zip` asset from that release,
- extract it,
- deploy it to GitHub Pages.