# Documentation for the OBIS Species Distribution Models (part of the MPA Europe project)

Documentation for the OBIS contribution to [MPA Europe](https://mpa-europe.eu) (WP3): species distribution models (SDMs), diversity metrics and habitat maps for European marine species.

The rendered documentation is available at <https://iobis.github.io/mpaeu_docs>.

## Contents

The documentation is a [Quarto](https://quarto.org) book (see `_quarto.yml`). Chapters, in order:

| File | Content |
|---|---|
| `index.qmd` | Introduction |
| `studyarea.qmd` | Definition of the study area |
| `sdms.qmd` | The SDM framework and the modelling workflow |
| `datadownload.qmd` | Species list, occurrence data and quality control |
| `datamining.qmd` | Additional biodiversity data (literature, repositories, GBIF) |
| `datause.qmd` | How to access and use the models (map platform, AWS, STAC) |
| `understanding.qmd` | How to interpret SDM outputs |
| `citations.qmd` | Datasets used (loaded from `datasets_citation.json` in `mpaeu_sdm`) |

`methods-testing.qmd` and `results.qmd` are kept in the repository but currently not included in the book (they are commented out in `_quarto.yml`).

## Related repositories

- [iobis/mpaeu_sdm](https://github.com/iobis/mpaeu_sdm): code to run the modelling pipeline
- [iobis/mpaeu_msdm](https://github.com/iobis/mpaeu_msdm): the `obissdm` R package
- [iobis/mpaeu_maps](https://github.com/iobis/mpaeu_maps): data access and how to cite the product
- [iobis/mpaeu_studyarea](https://github.com/iobis/mpaeu_studyarea): study area shapefiles

## Building the docs

```bash
quarto render
```

Output goes to `docs/` (used by GitHub Pages). Computation results are cached in `_freeze/`. Some chapters read example model outputs from `files/results`, which are not fetched by the render.

## Project status

The MPA Europe project concluded in 2025. The documentation describes the modelling as done in version 2 of the SDMs (concluded in August 2025). See the [`mpaeu_sdm` NEWS](https://github.com/iobis/mpaeu_sdm/blob/main/NEWS.md) for later code changes.
