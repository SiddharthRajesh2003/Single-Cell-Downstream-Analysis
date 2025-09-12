# Single-Cell-Downstream-Analysis

1. Please download the dataset from GEO Accession number: [GSE214865](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE214865)

2. After downloading the dataset, move the tar file to your project directory and run the following commmand
```bash
    mkdir -p data
    tar xvf *.tar.gz -C data/
```

3. Make sure you have downloaded the following packages: BiocManager, Seurat, tidyverse, ggplot2 else, run these lines in R.
```r
    install.packages('BiocManager')
    install.packages(c('tidyverse','ggplot2'))
    BiocManager::install('Seurat')
```

4. Make sure to install [Quarto](https://quarto.org/docs/get-started/) and run the following in the command line.
```bash
    quarto render analysis.qmd -t html
```