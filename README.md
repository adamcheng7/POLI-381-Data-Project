# POLI 381 Data Project
**Author**: Adam Cheng

**Organization**: University of British Columnbia (UBC), Vancouver, Canada

**Email**: adamchengworkstation@gmail.com

## Project Overview
This project aims to study how economic performance influences public approval of national governments over time. The dataset contains 9 variables covering 111 countries between 1990-2023.

The variables include:
- `country_name`: Name of the country

- `country_code`: ISO 3166-1 alpha-3 code of the country

- `year`: Calendar year

- `gdp_pc`: GDP per capita in 2021 PPP USD ($)

- `gdp_pc_growth`: % change of `gdp_pc` from the previous year

- `approval_smoothed`: Approval of national government (% of survey respondents) smoothed via exponential smoothing

- `approval_growth`: % change of `approval_smoothed` from the previous year

- `cpi_growth`: % change of consumer price index (CPI) from the previous year

- `unemployment_rate`: Unemployment rate (% of labor force)

## Data Source
The data is sourced from the following:
1. [Executive Approval Project (EAP)](https://www.executiveapproval.org/)

2. [International Monetary Fund (IMF)](https://data.imf.org/?sk=4c514d48-b6ba-49ed-8ab9-52b0c1a0179b)

3. [World Bank](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators)

## Directories
- `data`: Contains the datasets used in the project

    - `complete_dataset.csv`: The complete dataset used for analysis

        - `complete_dataset.dta`: The complete dataset in Stata format

        - `complete_dataset.RData`: The complete dataset in R data format

    - `original_datasets`: Contains the original datasets collected from the listed data sources and used to create `complete_dataset`

        - `eap_data.csv`: Original dataset retrieved from the Executive Approval Project

        - `imf_data.csv`: Original dataset retrieved from the International Monetary Fund

        - `wb_data.csv`: Original dataset retrieved from the World Bank

- `syntax`: Contains the syntax files created and used for this project

    - `dataset_construction.qmd`: Quarto Markdown file in R code documenting the project dataset construction process

    - `data_quality_control.qmd`: Quarto Markdown file in R code for data quality control

    - `data_analysis.qmd`: Quarto Markdown file in R code for data analysis

    - `*.html and *.pdf`: Files rendered from the Quarto Markdown files. File format depends on the available output format(s) specified in the YAML of the Quarto Markdown files

- `syntax`-specific files: 
    - `bibliography`: Contains the bibliography files used for citations

        - `*.bib`: BibTeX file containing references for documents

        - `*.csl`: Citation Style Language files used for formatting references

    - `tex`: Contains the LaTeX files used for generating publication-ready documents

        - `*.tex`: LaTeX files containing the code for generating publication-ready documents

        - `*.cls`: LaTeX class files used for formatting the documents


## Software Requirements
- [R](https://www.r-project.org/) version 4.2.2 or higher

- [Quarto](https://quarto.org/) for acceesing `.qmd` files

-  An Intergrated development environment (IDE) or a code editor of your choice ([RStudio](https://posit.co/downloads/), [VSCode](https://code.visualstudio.com/), [PyCharm](https://www.jetbrains.com/pycharm/), etc.) to run R code
    - [RStudio](https://posit.co/downloads/) is recommended as it provides a user-friendly interface for R programming and data analysis

## Running the Code
**To run code for the `*.qmd` files**:

- Install [Quarto](https://quarto.org/docs/get-started/)

- Ensure the appropriate programming language is installed (e.g., R, Python)

- Open the `*.qmd` file in RStudio or any [code editor supported by Quarto](https://quarto.org/docs/get-started/hello/vscode.html)

- Run the code from top to bottom

- **Note**: To generate publication ready documents from the `*.qmd` files...
    - Click on the "Render" button in RStudio or use the command line to render the file

    - The output will be saved in the same directory as the `*.qmd` file unless specified otherwise

## References
Carlin, R. E., Hartlyn, J., Hellwig, T., Love, G. J., Martı́nez-Gallardo, C., Singer, M. M.,..Sert, H. (2023). *Executive Approval Database 3.0*. \[Annual and National Dataset\]. Retrieved from https://executiveapproval.org/

International Monetary Fund. (2025). *International Financial Statistics (IFS)*. \[Annual and National Dataset\]. Retrieved from https://data.imf.org/?sk=4c514d48-b6ba-49ed-8ab9-52b0c1a0179b

The World Bank. (2025). *World Development Indicators*. \[Annual and National Dataset\]. Retrieved from https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators

