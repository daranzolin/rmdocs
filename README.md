
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rmdocs

<!-- badges: start -->

<!-- badges: end -->

Browse help files as RMarkdown source documents.

## Installation

``` r
# install.packages("devtools")
devtools::install_github("milesmcbain/rmdocs")
```

## Usage

``` r
rmdocs::rmd_help(help)
```

Use option `rmd_doc_width` to control the text width of the
documentation output. Defaults to 80.

### VSCode

In `keybindings.json`:

``` json
[
    {
        "description": "Rmd helpfile for object",
        "key": "ctrl+shift+h",
        "command": "r.runCommandWithSelectionOrWord",
        "args": "rmddocs::rmd_help($$)",
        "when": "editorTextFocus"
    },
]
```

### RStudio

[Bind the
addin](https://www.infoworld.com/article/3327573/do-more-with-r-rstudio-addins-and-keyboard-shortcuts.html)
‘Rmarkdown help() on object’ to a choice keyboard shortcut and away you
go.
