# Claude Code Project Guide — Orchid Pest Risk Analysis

## Project Purpose

Spatial analysis of how proximity to urban areas and plant import centers
affects the risk of a grower encountering an invasive insect pest that
affects multiple cultivated crops, including orchids.

## Authors

- **Laura Carotti** — lead author
- **Francesca Salinari** — collaborator
- **[Collaborator, Netherlands]** — collaborator (name to be confirmed)
- **Mathis Erler** — collaborator

## Repository Layout

```
data/
  raw/          # unmodified source data — never overwrite by script
  processed/    # cleaned and analysis-ready datasets produced by scripts
scripts/        # R scripts (.R) and Quarto documents (.qmd)
docs/           # rendered HTML output, served via GitHub Pages
index.qmd       # site landing page
_quarto.yml     # Quarto project configuration
```

## Code Guidelines

1. **Language**: All analytical code must be written in R.
2. **Readability over performance**: code clarity takes priority; avoid
   premature optimisation.
3. **Comprehensible names**: variable and function names should be
   self-explanatory without reading surrounding context.
   Names up to 40 characters are acceptable.
4. **Standard functions**: prefer base-R and tidyverse idioms over custom
   helpers when a standard function exists.
5. **No unnecessary abstraction**: do not create helper functions for
   one-off operations; three clear lines beat a premature wrapper.
6. **Comments only where logic is non-obvious**: do not comment what
   the code obviously does.

## Publishing

The analysis is published to GitHub Pages from the `docs/` folder on the
`main` branch. Render with:

```bash
quarto render
```

Then commit and push `docs/` along with source changes.

## Agent Files

The `.claude/` directory and any other Claude Code session files are
gitignored and must not be committed.
