# dependencyA

This package uses magrittr's `extract()` with `Depends` directive, which causes this error:

```r
devtools::install_github("yutannihilation/dependencyA")

library("dependencyA")

# this works
take1(1:10)

# a package that has another extract()
library(tidyr)

# this fails
take1(1:10)
```
