# POLI 381 Data Project
**Author**: Adam Cheng

**Organization**: University of British Columnbia (UBC), Vancouver, Canada

**Email**: adamchengworkstation@gmail.com

## Project Overview
This project aims to study how economic performance influences public approval of national governments over time. The dataset contains 9 variables covering 111 countries between 1990-2023.

The variables include:
- `country_name`: Name of the country

- `country_code`: ISO 3166-1 alpha-3 code of the country

- `year`: Year of the observation

- `gdp_pc`: GDP per capita in 2021 PPP USD ($)

- `gdp_pc_growth`: % change of `gdp_pc` from the previous year

- `approval_smoothed`: Approval of national government (% of survey respondents) smoothed via exponential smoothing

- `approval_growth`: % change of `approval_smoothed` from the previous year

- `cpi_growth`: % change of consumer price index (CPI) from the previous year

- `unemployment_rate`: Unemployment rate (% of labor force)

## Data Source
The data is sourced from the following:
1. [World Bank](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators)

2. [Executive Approval Project (EAP)](https://www.executiveapproval.org/)

3. [International Monetary Fund (IMF)](https://data.imf.org/?sk=4c514d48-b6ba-49ed-8ab9-52b0c1a0179b)

## Directories
- `data`: Contains the dataset

    - `complete_dataset.csv`: The complete dataset used for analysis

- `syntax`: Contains the syntax files used for data quality control and analysis

    - `data_quality_control.qmd`: Quarto Markdown file in R code for data quality control

- `bibliography`: Contains the bibliography files used for citations

    - `*.bib`: BibTeX file containing references for documents

    - `citation_styles/*.csl`: Citation Style Language files used for formatting references


## Software Requirements
- [R](https://www.r-project.org/) version 4.2.2 or higher

- [Quarto](https://quarto.org/) for acceesing `.qmd` files

-  An Intergrated development environment (IDEs) or code editor of your choice ([VSCode](https://code.visualstudio.com/), [PyCharm](https://www.jetbrains.com/pycharm/), etc.) to run any R code
    - [RStudio](https://posit.co/downloads/) is recommended as it provides a user-friendly interface for R programming and data analysis

## Running the Code
- To run the code for `data_quality_control.qmd`:

    - Install [Quarto](https://quarto.org/docs/get-started/)

    - Open the `.qmd` file in RStudio or any [code editor supported by Quarto](https://quarto.org/docs/get-started/hello/vscode.html)

    - Run the code from top to bottom

    - To generate publication ready files:
        - Click on the "Render" button in RStudio or use the command line to render the file

        - The output will be saved in the same directory as the `.qmd` file unless specified otherwise
## References
Carlin, R. E., Hartlyn, J., Hellwig, T., Love, G. J., Martı́nez-Gallardo, C., Singer, M. M.,..Sert, H. (2023). *Executive Approval Database 3.0*. \[Annual and National Dataset\]. Retrieved from https://executiveapproval.org/

International Monetary Fund. (2025). *International Financial Statistics (IFS)*. \[Annual and National Dataset\]. Retrieved from https://data.imf.org/?sk=4c514d48-b6ba-49ed-8ab9-52b0c1a0179b

The World Bank. (2025). *World Development Indicators*. \[Annual and National Dataset\]. Retrieved from https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators

