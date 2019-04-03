# Is the SAT unfair?  
### Cleaning NYC high school data to start finding the answer
==============================  

## Goal of this project
The goal of this project is to clean and consolidate several datasets relating to the SAT (Scholastic Aptitude Test) and NYC (New York City) high schools. The final cleaned dataset will be used in separate projects to explore if the SAT is unfair to particular groups of students. The annual SAT is used by U.S. colleges and universities to determine which students to admit into their programs.  

## Approach
We will begin by exploring each of the datasets to understand the information they contain and how they can be consolidated.  We will then clean the datasets to make them ready for further analysis and modeling (i.e. correcting data types and errors, removing unnecessary characters and columns, filling in missing values etc...).  Finally, we will consolidate all of the data into a single cleaned dataset and export it to a csv (comma separated value) file that is ready to use for further exploratory data analysis, visualization and predictive modeling.  

## Summary of results  
The raw data consists of 8 separate datasets containing missing values, incorrect data types, data errors, unnecessary columns and a combined total of 65,875 rows and 3,861 columns.  The final result of this project is a single consolidated csv file containing 362 rows and 79 columns.  This final dataset is clean, consistent, relevant and ready to use for further analysis and modeling to explore the fairness of the SAT.

## Viewing the project  
For proper rendering, I recommend viewing the project in nbviewer [here](https://nbviewer.jupyter.org/github/JustinToribio/cleaning-nyc-hs-data/blob/master/notebooks/1.0-jt-clean-nyc-hs-data.ipynb).  

Alternatively, you can view the project directly in GitHub by going to the `"notebooks"` folder of this repository.  However, there are some rendering issues when viewing Jupyter Notebooks in GitHub.  

## Installing and running the project  

### Download the project  
* Download and extract, or clone this repository to your computer  
* Do not alter the folder/file structure or the file references in the Jupyter Notebook will break

### Make sure you have the `conda` package manager installed  
* If you don't already, follow the instructions [here](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)

### Reproduce the project environment and launch the Jupyter Notebook
* From your computer's command line interface, run the following commands:    
    * Make sure you are in the parent directory of this repository (i.e. ".../cleaning-nyc-hs-data", ".../cleaning-nyc-hs-data-master" etc..., whatever you named it when you downloaded or cloned it): `cd <path-to-repo-parent-directory>`  
    * Reproduce the project environment: `conda env create -f environment.yml`  
    * Activate the environment:  
        * On Windows: `activate project_env`  
        * On macOS and Linux: `source activate project_env`  
    * Launch the Jupyter Notebook: `jupyter notebook notebooks/1.0-jt-clean-nyc-hs-data.ipynb`

### Run the Jupyter Notebook
* From the Jupyter Notebook `"1.0-jt-clean-nyc-hs-data.ipynb"`:  
    * To run each cell one at a time: click `Run` in the top control panel or press `Shift + Enter`
    * To run all of the cells: click `Kernel` in the menu bar and then `Restart & Run All`
* After the last code cell is run, the final cleaned dataset will be exported to a csv file named `"nyc_hs_data_clean.csv"` in the `"data/processed"` folder of this project

## Project organization
------------

    ├── data
    │   ├── processed      <- The final cleaned dataset produced by running this project
    │   └── raw            <- The original and immutable data dump
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short "-" delimited description, e.g.
    │                         "1.0-jt-clean-nyc-hs-data"
    │
    ├── references         <- Data dictionaries
    │
    ├── .gitignore         <- Files and folders for Git to ignore tracking
    ├── LICENSE            <- The license governing the use and redistribution of this project
    ├── README.md          <- The top-level README for users of this project  
    └── environment.yml    <- The file for reproducing this project's environment


--------