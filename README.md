# Pest Risk and Proximity to Urban Areas and Import Centers

A spatial analysis of how proximity to urban areas and plant import centers
influences the probability that a grower will encounter an invasive insect
pest affecting multiple cultivated crops, including orchids.

**Author**: Mathis Erler

## Published analysis

The rendered analysis is available at:  
`https://mdmdma.github.io/orcid-pest/`

## Repository structure

| Path | Contents |
|------|----------|
| `data/raw/` | Unmodified source data |
| `data/processed/` | Cleaned, analysis-ready datasets |
| `scripts/` | R scripts and Quarto analysis documents |
| `docs/` | Rendered HTML site (served via GitHub Pages) |

## Reproduce the analysis

Requirements: R ≥ 4.3, [Quarto](https://quarto.org/) ≥ 1.4.

```r
# Install required packages (first run only)
install.packages(c("tidyverse", "sf", "terra", "tmap"))
```

Render the site:

```bash
quarto render
```

The output is written to `docs/` and can be previewed locally with
`quarto preview`.
