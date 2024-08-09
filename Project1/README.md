# Project 1: Analyzing Energy Consumption in the US

## Background
Energy plays a crucial role in economic growth in modern economies, with individuals and organizations relying on various energy sources to sustain their businesses. The energy sector, particularly electricity, significantly impacts economic development. This impact is seen in improved labor and capital productivity from a reliable energy sector and the consumption of electricity serving as an indicator of a healthy economy in developing countries.

## Objective
This study aims to examine the properties of energy consumption in the US from 1973 to 2022, exploring the following questions:
- What characteristics of the time series representing energy consumption contribute most to its predictability?
- What is the relationship between energy consumption trends and GDP?
- What external factors help in predicting energy consumption?

## Data
The datasets used in this study are as follows:

1. **Energy Consumption**:
   - **Source**: US Energy Information Administration
   - **Description**: Monthly energy consumption by sector from January 1973 to April 2023.
   - **Variables**: 15 variables measured in British Thermal Units (BTU).

2. **GDP**:
   - **Source**: FRED Economic Data
   - **Description**: Quarterly GDP figures measured in billions of dollars.
   - **Period**: 1973 to 2023.
   - **Purpose**: Serves as a proxy for economic activity and growth.

3. **Population Growth**:
   - **Source**: FRED Economic Data
   - **Description**: Monthly population figures.
   - **Period**: 1973 to 2023.
   - **Purpose**: Investigates the impact of demographic changes on energy consumption in various sectors.

### Files
- `Energy_Dynamics_US_Sector_Analysis.ipynb`: Jupyter Notebook with the analysis and code for the project.
- `Energy Consumption_r.csv`: Contains monthly energy consumption data by sector.
- `GDP-data.csv`: Contains quarterly GDP data.
- `population-data.csv`: Contains monthly population data.
- `Report.pdf`: A PDF report summarizing the analysis and findings.
- `activate.R`: Script to activate the `renv` environment for reproducibility.
- `renv.lock`: Lock file that records the state of the project's dependencies for reproducibility.

## Dependencies

To ensure that others can reproduce the results of this analysis, we use `renv` for package management. Follow the steps below to set up your environment:

1. **Clone the Repository**:
    Cloning the repository creates a local copy of the project on your machine, including all files and the directory structure. This ensures you have the exact same setup for reproducibility:
    ```sh
    git clone https://github.com/micchoi/micchoi-portfolio.git
    cd micchoi-portfolio/Project1  # Navigate to the desired project directory
    ```

2. **Open the Jupyter Notebook**:
    You can open the notebook in any IDE that supports Jupyter Notebooks, such as Jupyter, JupyterLab, VS Code, PyCharm, etc. For example, to open it in Jupyter:
    ```sh
    jupyter notebook Energy_Dynamics_US_Sector_Analysis.ipynb
    ```

    Alternatively, you can use Jupyter Lab:
    ```sh
    jupyter lab Energy_Dynamics_US_Sector_Analysis.ipynb
    ```

3. **Restore the `renv` Environment and Run the Notebook Cells**:
    In the Jupyter Notebook, run the first few cells that include:
    ```r
    library(renv)
    renv::restore()
    ```
    This command will read the `renv.lock` file and install the required package versions to match the environment used for this analysis. Continue running the remaining cells sequentially to complete the analysis.

4. **Run the Notebook Cells**:
    In the Jupyter Notebook, run the cells sequentially. The notebook already contains `library(renv)` and `renv::restore()` calls to set up the R environment as defined by the `renv.lock` file.
