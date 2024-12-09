
# Data Analysis Project Environment

This repo contains a template directory structure and quarto configuration files for a [PRISM](https://prism.center/) data analysis project run at [Gustave Roussy](https://www.gustaveroussy.fr/en/institute). There are three main top-level directories.

* `data/` to store raw and preprocessed data
* `analyses/` to hold analysis module directories. Each analysis module directory contains the following elements:
  * A Quarto document outlining the analysis module
  * `snippets/` to hold scripts to generate computationally intensive results. This pre quarto document processing speeds up the rendering time of the analysis module report. 
  * `run\` holds local processing scripts such as HPC submission scripts.
  * `objects\` holds processed results objects that are used to render the final quarto document.
* `results\` This directory contains links to the qmd files in `analyses`. These files are rendered here. Paths to dependent data objects are handled using the here package. This directory contains all the quarto configuration files. 


## Acknowledgements

@christopherbarrington was responsible for building the quarto configuration structure used here.