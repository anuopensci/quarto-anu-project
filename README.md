

<!-- README.md is generated from README.qmd. Please edit that file -->

# A starter for Quarto project

This is a template for a project that involves data.

There are varying suggestions for the folder structure (see Related).
This particular project has the following structure.

    project/                          # Root of the project folder (rename this)
    │
    ├── project.Rproj                 # RStudio project (rename this to the root folder name)
    │
    ├── .git/                         # Git tracking folder
    ├── .gitignore                    # List of files/folders to be ignored by GIT
    │
    ├── .Rprofile                     # project R profile
    ├── .Renviron                     # project R environment
    ├── renv/                         # renv package management folder
    │
    ├── _targets/                     # targets outputs storage folder
    ├── _targets.R                    # targets pipeline
    ├── _targets.yaml                 # a YAML file to configure the pipeline
    │
    ├── R/                            # directory containing R functions
    │   ├── fn-process.R              # custom functions to process the data
    │   └── fn-utils.R                # custom utility functions
    │
    ├── man/                          # Contents are automatically created by roxygen2
    │
    ├── DESCRIPTION                   # Project metadata                              [*]
    ├── LICENSE.md                    # Content of the GPL3 license (replace as needed)
    ├── NAMESPACE                     # Automatically generated
    ├── .Rbuildignore                 # List of files/folders to be ignored while 
    │                                 # checking/installing the package
    │
    ├── README.md                     # GitHub README (automatically generated)
    ├── README.qmd                    # GitHub README                                 [*]
    │
    ├── data/                         # Raw and derived data
    │   ├── raw-data/                 # Read-only files
    │   ├── input-data/.              # Extracted and coerced from raw data
    │   └── valid-data/               # Edit and imputed from input data
    │
    ├── analysis/                     # R scripts (not function) to run analysis
    │
    ├── outputs/                      # Outputs 
    │   ├── statistics/               # Analysed results (R objects, .csv, etc.)
    │   ├── report/                   # Report format (delete if not applicable)
    │   ├── paper/                    # Paper format (delete if not applicable)
    │   └── thesis/                   # Thesis format (delete if not applicable)
    │
    ├── figures/                      # Figures (.png, .pdf, etc.)
    │
    ├── index.qmd                     # The main index file for the documentation website
    ├── about.qmd                     # An about page for the documentation website
    └── docs/                         # Documentation website (could be generated from pkgdown)

## Related

- [`rcompendium`](https://frbcesab.github.io/rcompendium/articles/working_with_a_compendium.html)
- [`rrrpkg`](https://github.com/ropensci/rrrpkg)
- [`targets`](https://books.ropensci.org/targets/projects.html)
- [`worflow`](https://workflowr.github.io/workflowr/articles/wflow-01-getting-started.html)
- The data structure used in this project follows the statistical value
  chain presented in the “Statistical data cleaning with applications in
  R”.
