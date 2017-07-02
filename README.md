# dependencyA

This package uses magrittr's `extract()` with `Imports` directive, which is ok when doing this:

```r
devtools::install_github("yutannihilation/dependencyA@use-imports")

library("dependencyA")

# this works
take1(1:10)

# a package that has another extract()
library(tidyr)

# this still works
take1(1:10)
```
