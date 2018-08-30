# gcapc: GC effects aware peak caller

### Introduction
ChIP-seq has been widely utilized as the standard technology to detect 
protein binding regions, where peak calling algorithms were developed 
particularly to serve the analysis. Existing peak callers lack of power 
on ranking peaks' significance due to sequencing technology might undergo
sequence context biases, *e.g.* GC bias. *gcapc* is designed to address 
this deficiency by modeling GC effects into peak calling.

### Installation

*gcapc* is an R/Bioconductor package, which can be installed with source
code documented in [GitHub](https://github.com/tengmx/gcapc) or simply
through [Bioconductor](https://bioconductor.org/packages/gcapc).

If GitHub source installation is selected, make sure dependency
R packages are pre-installed as shown in the
[DESCRIPTION](https://github.com/tengmx/gcapc/blob/master/DESCRIPTION) file.
Then, install *gcapc* with following code.
```s
library(devtools)
install_github("tengmx/gcapc")
```

Alternatively, installation through Bioconductor is as simple as follows.
```s
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("gcapc")
```

### Using *gcapc*

First, load the package into R.
```s
library(gcapc)
```

Then, follow the steps introduced in the package 
[vignette](https://bioconductor.org/packages/devel/bioc/vignettes/gcapc/inst/doc/gcapc.html)
to estimate GC-bias or peak calling.

### Help

You are very welcome to leave any questions/bug messages at
[GitHub issues](https://github.com/tengmx/gcapc/issues).
