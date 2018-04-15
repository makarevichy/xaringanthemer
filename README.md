
<!-- README.md is generated from README.Rmd. Please edit that file -->

# xaringanthemer

Easily style your [xaringan](https://github.com/yihui/xaringan) slides
with **xaringanthemer**

## Installation

Currently, this is a work in progress. Try it yourself:

``` r
devtools::install_github("gadenbuie/xaringanthemer")
```

## Make it work

To make it work, add `css: xaringan-themed.css` to your xaringan slides
YAML header under `xaringan::moonreader:`

``` yaml
output:
  xaringan::moon_reader:
    lib_dir: libs
    css: xaringan-themed.css
```

Then, in the first knitr chunk, try this:

```` markdown
```{r setup}
options(htmltools.dir.version = FALSE)
library(xaringanthemer)
mono_dark(
  base_color = "#b6174b",
  header_font_google = google_font("Josefin Sans"),
  text_font_google = google_font("Montserrat", "300", "300i"),
  code_font_google = google_font("Droid Mono")
)
```
````
