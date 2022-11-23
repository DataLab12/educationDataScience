# Tabular Data in the Wild: Gradient Boosting Modeling Improvement
**DData Science Pipeline for Integrating, Analyzing and Modeling Open Source Tabular Data**

_Data Science Pipeline developed for the [Mitigating U.S. Public School Teacher Attrition Crisis](TeacherAttrition/docs/2022-DS-Poster-SASS.pdf) project_  by [June Yu](https://j-y-yu.github.io/), (data integration and modeling), [Li Feng](https://lifeng.wp.txstate.edu/) (domain expert), and [Jelena Tešić](jtesic.github.io) (project lead). 

_Data Science Pipeline developed for the [Identifying Resilience Factors in Texas Public Schools](LearningLoss/docs/2022Fall-CHERR-Poster.pdf) project_  by [June Yu](https://j-y-yu.github.io/), (data integration and modeling), [Daniel Payan](https://github.com/danielpayan13) ([dashboard author](https://github.com/DataLab12/resilienceDashboardsTX)), [Li Feng](https://lifeng.wp.txstate.edu/) (domain expert), and [Jelena Tešić](jtesic.github.io) (project lead). The work has been supported by [The Center of Excellence for Community Health and Economic Resilience Research](https://www.cherr.txst.edu/) and [Data Lab](https://DataLab12.github.io) @ Texas State University.

## Data Science Pipeline - Project #1 [Mitigating U.S. Public School Teacher Attrition Crisis](TeacherAttrition)
### Directory 
* [data](TeacherAttrition/data) - All raw data and documents, cleaned data
* [docs](TeacherAttrition/docs) - Projects related documents
* [src](TeacherAttrition/src) - Python Jupyter notebooks
  * [processing](TeacherAttrition/src/processing) - Integrating and preprocessing raw data
    * [Data_Integration.ipynb](TeacherAttrition/src/processing/Data_Integration.ipynb) - integrating data into single dataframe 
    * [EDA.ipynb](TeacherAttrition/src/processing/EDA.ipynb) - EDA for Public teachers, principals, and schools
    * [Feature_Selection_1.ipynb](TeacherAttrition/src/processing/Feature_Selection_1.ipynb) - correlation filtering
    * [Feature_Selection_2.ipynb](TeacherAttrition/src/processing/Feature_Selection_2.ipynb) - automated scoring for feature importance
  * [modeling](TeacherAttrition/src/modeling) - Predicting Teacher Retention
    * [Modeling_BL.ipynb](TeacherAttrition/src/modeling/Modeling_BL.ipynb) - State-of-and-art prediction modeling
    * [Modeling_GB.ipynb](TeacherAttrition/src/modeling/Modeling_GB.ipynb) - Advanced gradient boosting prediction modeling
    * [Unlabeled_Data_Integration.ipynb](TeacherAttrition/src/modeling/Unlabeled_Data_Integration.ipynb) - Integrating unlabeled data to predict teacher attrition for teachers whom did not participate TFS 
    * [Unlabeled_Modeling_GB.ipynb](TeacherAttrition/src/modeling/Unlabeled_Modeling_GB.ipynb) - Predicting teacher attrition with unlabeled data using the best gradient boosting model
    * [Modeling_NA_GB.ipynb](TeacherAttrition/src/modeling/Modeling_NA_GB.ipynb) - Experimenting Advanced gradient boosting prediction modeling with raw data


## Data Science Pipeline - Project #2 [Identifying Resilience Factors in Texas Public Schools](LearningLoss)
### Directory 
* [data](LearningLoss/data) - Cleaning all raw data
* [docs](LearningLoss/docs) - Project related documents 
* [src](LearningLoss/src) - Python Jupyter notebooks for CHERR project
  * [processing](LearningLoss/src/processing) - Integrating and preprocessing all raw data
    * [Data_Integration.ipynb](LearningLoss/src/processing/Data_Integration.ipynb) - integrating all data from 8 diffferent sources
    * [EDA.ipynb](LearningLoss/src/processing/EDA.ipynb) - including EDA, labeling, normlization
    * [Feature_Selection_Math.ipynb](LearningLoss/src/processing/Feature_Selection_Math.ipynb) - automated scoring for feature importance for math subject
    * [Feature_Selection_Reading.ipynb](LearningLoss/src/processing/Feature_Selection_Reading.ipynb) - automated scoring for feature importance for reading subject
  * [modeling](LearningLoss/src/modeling) - Predicting Learning Loss 
    * [Modeling_BL_Math.ipynb](LearningLoss/src/modeling/Modeling_BL_Math.ipynb) - State-of-and-art prediction modeling for math 
    * [Modeling_BL_Reading.ipynb](LearningLoss/src/modeling/Modeling_BL_Reading.ipynb) - State-of-and-art prediction modeling for math 
    * [Modeling_GB_Math.ipynb](LearningLoss/src/modeling/Modeling_GB_Math.ipynb) - Advanced gradient boosting prediction modeling for math
    * [Modeling_GB_Reading.ipynb](LearningLoss/src/modeling/Modeling_GB_Reading.ipynb) - Advanced gradient boosting prediction modeling for reading
    * [Modeling_NA_GB_Math.ipynb](LearningLoss/src/modeling/Modeling_NA_GB_Math.ipynb) - Experimenting the gradient boosting models with missing values for math
    * [Modeling_NA_GB_Reading.ipynb](LearningLoss/src/modeling/Modeling_NA_GB_Reading.ipynb) - Experimenting the gradient boosting models with mssing values for reading


## SETUP
  1. Download Anaconda/Juptyer Notebook for your device's operating system from [here](https://www.anaconda.com/products/distribution#Downloads)
  2. Run Anaconda Prompt app with administrative privileges
     * make sure all the conda packages are up to date: ```conda update --all```
       * answer Yes to install all packages   
     * install/check versions of needed packages (as of October 31, 2022)
        * Python: 3.10.4 
        * IPython: 8.4.0
        * pandas: 1.4.3
        * NumPy: 1.23.1
        * matplotlib: 3.5.2
        * seaborn: 0.11.2
        * mlxtend: 0.20.0
        * SciPy: 1.9.1
        * Scikit-learn: 1.1.1
        * XGBoost: 1.6.2
        * LightGBM: 3.2.1
        * CatBoost: 1.0.6
  3. close the anaconda prompt and open it up as a regular user , type ```>>jupyter notebook```
     * navigate in the browser to this folder and double click on any file with the _ipynb_ extension listed above to open them (separate windows will open)
     * in separate windows, click `Cell` on the top taskbar and then `Run All`. This will open the the tabbed dashboard.
