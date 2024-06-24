

<!-- README.md is generated from README.qmd. Please edit that file -->

# A starter template for Quarto project

This is a starter template for a Quarto project. In general, your
project would involve data and analysis of data. The folder structure is
organised according to the consolidation of several recommended
practices. Some of these are included under the [Related](#related)
section.

This template is primary geared for the [R](https://www.r-project.org/)
user but can be adapted to other programming languages,
e.g. [Python](https://www.python.org/) and
[Julia](https://julialang.org/), with little effort. Note that
[Quarto](https://quarto.org/) is language agnostic and works well with
Python, Julia and some other programming languages as well.

The template has the following structure.

    quarto-anu-project/               # Root of the project folder (rename this)
    │
    ├── .git/                         # Git tracking folder
    ├── .gitignore                    # List of files/folders to be ignored by GIT
    │
    ├── LICENSE.md                    # Content of the GPL3 license (replace as needed)
    │
    ├── README.md                     # GitHub README (automatically generated)
    ├── README.qmd                    # GitHub README                                 [*]
    │
    ├── data/                         # Raw and derived data
    │   ├── data-raw/                 # Read-only files
    │   ├── data-input/               # Extracted and coerced from raw data
    │   └── data-valid/               # Edit and imputed from input data
    │
    ├── code/                     # Scripts (not functions) to run analysis
    │
    ├── outputs/                      # Outputs 
    │   ├── stats/                    # Analysed results (R objects, .csv, etc.)
    │   ├── report/                   # Report format (delete if not applicable)
    │   ├── paper/                    # Paper format (delete if not applicable)
    │   └── thesis/                   # Thesis format (delete if not applicable)
    │
    ├── figures/                      # Figures (.png, .pdf, etc.)
    │
    ├── misc/                         # Misc
    │
    ├── index.qmd                     # The main index file for the documentation website
    ├── about.qmd                     # An about page for the documentation website
    └── docs/                         # Documentation website (could be generated from pkgdown)

The R bit:

``` r
quarto-anu-project/               # Root of the project folder (rename this)
│
├── quarto-anu-project.Rproj      # RStudio project (rename this to the root folder name)
│
├── .Rprofile                     # project R profile
├── .Renviron                     # project R environment
├── renv/                         # renv package management folder
│
├── _targets/                     # targets outputs storage folder 
|                                 # (should not be triacked by Git as it can be large)
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
├── NAMESPACE                     # Automatically generated
└── .Rbuildignore                 # List of files/folders to be ignored while 
                                  # checking/installing the package
```

## Preqrequisites

- Install Quarto
- Optionally install R and RStudio IDE (the project works well with
  Python, Julia or generally other programming langauges)
- Install Git
- Make a GitHub account

## Getting started

- Install the following R packages

``` r
install.packages(c("devtools", "usethis", "renv", "quarto"))
remotes::install_github("ropensci/targets")
```

- Click on “use this template” to create a new repository from this
  template. Don’t clone this repository. If you do so, be sure to delete
  the `.git` folder and re-initialise the repository with `git init`. If
  you’re unfamiliar with Git and GitHUb, check out [Happy Git and GitHub
  for the useR](https://happygitwithr.com/).

- Once you

### Using Git and GitHub

``` r
usethis::use_git_config(user.name = "", user.email = )
```

### Using `renv`

``` r
renv::init()
```

``` r
renv::snapshot()
```

``` r
renv::restore()
```

``` r
renv::update()
```

## Related

- [`rcompendium`](https://frbcesab.github.io/rcompendium/articles/working_with_a_compendium.html)
- [`rrrpkg`](https://github.com/ropensci/rrrpkg)
- [`targets`](https://books.ropensci.org/targets/projects.html)
- [`worflowr`](https://workflowr.github.io/workflowr/articles/wflow-01-getting-started.html)
- The data structure used in this project follows the statistical value
  chain presented in the “Statistical data cleaning with applications in
  R”.
