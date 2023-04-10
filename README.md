# Lazy Data

## Put data
* in package project directory, create `data/`
* put `whatever.rda` in `data/`
* In DESCRIPTION, add `LazyData:true`
* Add [R script](whatever.R) to `R/`

In R console, run

```
devtools::document()
```
You will see `export(whatever)` in NAMESPACE.

then, run 
```
devtools::document()
```

## Use data

```
library(pkgname)
data("whatever")
head(whatever)
```
