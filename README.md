# Glow-With-Lily
Realistic fitness, sustainable weight loss, and lifestyle coaching for busy moms and everyday people no extreme diets, no burnout.
Official GitHub Actions badge (recommended)
- Put this in your README where you want the badge to appear.

Markdown:
```markdown
[![Export assets](https://github.com/OWNER/REPO_NAME/actions/workflows/export-svgs-pr.yml/badge.svg)](https://github.com/OWNER/REPO_NAME/actions/workflows/export-svgs-pr.yml)
```

Example (replace OWNER/REPO_NAME):
```markdown
[![Export assets](https://github.com/LillaqwayHudspeth/REPO_NAME/actions/workflows/export-svgs-pr.yml/badge.svg)](https://github.com/LillaqwayHudspeth/REPO_NAME/actions/workflows/export-svgs-pr.yml)
```

2) Shields.io badge (customizable, same purpose)
- Use this if you want a different style or additional query params.

Markdown:
```markdown
![Export assets](https://img.shields.io/github/actions/workflow/status/OWNER/REPO_NAME/export-svgs-pr.yml?label=export%20assets&logo=github&style=for-the-badge)
```

Example:
```markdown
![Export assets](https://img.shields.io/github/actions/workflow/status/LillaqwayHudspeth/REPO_NAME/export-svgs-pr.yml?label=export%20assets&logo=github&style=for-the-badge)
```

3) Add a short status line and link (nice under the badge)
```markdown
**Automated image export:** [Export SVGs → PNG & WebP workflow](https://github.com/OWNER/REPO_NAME/actions/workflows/export-svgs-pr.yml) — runs on SVG changes and creates a PR with optimized assets.
```

4) Quick instructions for reviewers (optional small block)
```markdown
> The workflow rasterizes and optimizes SVGs into `dist/images/`, uploads artifacts to the workflow run, and opens a PR with previews. Use the workflow Dispatch inputs to enable/disable lossy PNG quantization (`lossypng`) or change thumbnail width (`thumb_width`).
```

Notes & tips
- Make sure the workflow file path in the badge URL matches exactly the file name in .github/workflows (we created `export-svgs-pr.yml`).
- The badge link points to the workflow page where you can see run history and artifacts. Artifact downloads are available from the Actions run page and also included as links in the PR description created by the workflow.
- If you want the README to show the *latest generated assets PR* automatically, we can:
  - Add a small GitHub Actions step that updates a static JSON or markdown file with the last PR URL and include that file via include in README; or
  - Leave the workflow PR description and artifact previews as-is (the workflow already puts previews in the PR).

Would you like me to:
- Commit the badge directly into your README.md (I can open a PR that adds the badge to your README in the repo you specify), or
- Produce a short README snippet that includes both the badge and a one-line explanation tailored to your repo name (tell me the repo name and I’ll create the exact markdown and optionally open a PR)?
