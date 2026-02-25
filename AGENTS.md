# AGENTS.md

## Cursor Cloud specific instructions

This is a GitHub profile README repository containing a single `README.md` file. There is no application code, build system, or runtime dependencies.

### Development tools

- **Lint**: `markdownlint README.md` — checks markdown style/formatting (installed globally via npm).
- **Preview**: `grip README.md 0.0.0.0:6419` — renders the README with GitHub styling at `http://localhost:6419` (installed via pip).

### Notes

- The "application" is the rendered Markdown on GitHub. There is no build step, no test suite, and no backend service.
- Grip may hit GitHub API rate limits for unauthenticated requests. Set `GITHUB_USERNAME` and `GITHUB_TOKEN` env vars if you encounter 403 errors during preview.
