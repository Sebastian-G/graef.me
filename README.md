# graef.me

Static source for the `graef.me` landing page.

## Repository Layout

- `static-content/` contains the published site.
- `.github/workflows/deploy-pages.yml` deploys the site to GitHub Pages.

## Local Preview

Because the site is fully static, any simple file server works:

```sh
python3 -m http.server --directory static-content 8000
```

Then open `http://localhost:8000`.

## GitHub Pages Setup

1. Push the repository to GitHub.
2. Open `Settings -> Pages`.
3. Set `Source` to `GitHub Actions`.
4. Set the custom domain to `graef.me`.
5. Ensure DNS is pointed at GitHub Pages.

## Notes

This repository intentionally publishes only the contents of `static-content/`.
