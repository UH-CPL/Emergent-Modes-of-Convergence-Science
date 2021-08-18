# Emergent-Cross-Disciplinarity
This repository contains the R scripts related to "Grand challenges and emergent modes of convergence science" project.

## Getting Started
#### Prerequisites
- R and RStudio
- Required packages

#### Installing R Packages
Packages are available on CRAN and can be installed using a simple call to `install.packages()`:

    install.packages('PackageName')
	
## Data Set
Please download the dataset from [OSF Data Repository] (https://osf.io/3myt8/, https://osf.io/d97eu/).


## Script Set

##### Please run the following scripts sequentially

**Network Analysis (Fig 2B)**
- Edge_creator_3category.Rmd
   - generate edge files based on region
- Node_creator_3category.Rmd
   - generate node files based on region
- gephi_AUSTRALASIA.gephi
   - generate giant network plots for Australasia region
- gephi_EUROPE.gephi
   - generate giant network plots for Europe region
- gephi_NA.gephi
   - generate giant network plots for North America region
   
See redme.txt file for node size and coloring techniques.

**Fig 2B**
- Sankey_diagrams.Rmd
  - generate Sankey diagrams or Fig 2B.


**Panel Modeling (Table S1, S2, S3, S4, and S5)**
- Panel_modeling_Author_level.Rmd
  - generate Table S1, Table S2, and Table S3
- Panel_modeling_article_level.Rmd
  - generate Table S4, and Table S5

