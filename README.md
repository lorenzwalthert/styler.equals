
<!-- README.md is generated from README.Rmd. Please edit that file -->

# styler.equals

This is a GitHub template to create and distribute a custom {styler}
style guide. For more info, see the [{styler}
documentation](https://styler.r-lib.org/dev/articles/distribute_custom_style_guides.html).
You can use this template to create a GitHub repo by pressing the green
button:

<img src="https://raw.githubusercontent.com/lorenzwalthert/some_raw_data/master/styler.yours.png" width="500" />

Here’s what you have to do once you created your repo from the template.

-   search for `equals_style` and replace it with the
    name of your style guide.

-   Adapt the authors field in `DESCRIPTION`.

-   In `create_style_guide()`, ensure the `style_guide_name` matches the
    expected format, e.g. styler has
    `"styler::tidyverse_style@https://github.com/r-lib"`. See
    `help(create_style_guide, package = "styler")` for details.

-   adapt the function `equals_style()` (the drop-in for
    `styler::tidyverse_style`) such that it does what you want.
    Currently, all the style guide is doing is to replace `<-` with `=`

-   add tests.

-   remove all of the above instructions.

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
[![R-CMD-check](https://github.com/equals/styler.equals/workflows/R-CMD-check/badge.svg)](https://github.com/equals/styler.equals/actions)
<!-- badges: end -->

The goal of {styler.equals} is… It is a third-party style
guide for [{styler}](https://styler.r-lib.org).

## Installation

You can install the released version of {styler.equals}
from [GitHub](https://github.com) with:

``` r
remotes::install_github("equals/styler.equals")
```

## Example

This is a basic example of how to style code with it.

``` r
library(styler.equals)
cache_deactivate()
text <- "x <- 4
y = 3
a;
"

style_text(text)
```
