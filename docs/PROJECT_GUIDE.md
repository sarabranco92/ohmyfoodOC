# ohmyfoodOC — project guide

Static restaurant directory with four restaurant menu pages, Sass styles and CSS interactions.

## Scope and source

This guide describes the default branch `master` reviewed on 3 October 2026. Commands were checked against committed manifests and configuration; applications and external integrations were not executed as part of this documentation update.

## Repository map

- `index.html`
- `SASS/main.scss`
- `SASS/main.css`
- `SASS/layouts`
- `SASS/utlis`

## Prerequisites and local use

Clone the repository and enter its root directory:

```sh
git clone https://github.com/sarabranco92/ohmyfoodOC.git
cd ohmyfoodOC
```

Use a modern browser. No npm install is required for the static frontend. With Python installed, serve the site locally:

```sh
python -m http.server 8000
```

On Windows, use `py -m http.server 8000` if `python` is unavailable. Open http://localhost:8000/. This is a local preview server, not production hosting.

### Recompile styles

With a Sass CLI installed, run from the repository root:

```sh
sass SASS/main.scss SASS/main.css
```

This is a suggested maintenance command, not a repository npm script.

## Configuration and implementation notes

Reservation and ordering language describes the design brief. No checkout, order-processing or reservation backend is present. Edit Sass sources rather than only the compiled CSS. The directory is named `utlis`, exactly as committed.

## Verification checklist

Open all four restaurant links, return to the home page, and inspect dish selection, heart animations and the loading animation at different screen widths.

No dedicated automated test/spec files were found in the reviewed application tree. Where a test script exists, its presence alone does not establish test coverage.

## Maintenance

Keep this guide in sync when routes, commands, environment variables or hosting paths change. Use development databases/accounts for integration checks. Keep private credentials in server-side environment configuration and out of documentation. No new license or ownership terms are introduced by this guide; retain existing repository notices.
