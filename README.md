# Mental Health in Tech

## 01 Dataset

This project analyzes the mental health survey results in technology industry. This data comes from Open Source Mental Illness (OSMI) and provides survey data from years 2014, 2016, 2017, 2018 and 2019. The data was collected using open online survey (with the help of Typeform tool), so the sample is not-probability, as no randomization was ensured during its collection. This is important to bear in mind when drawing wider conclusions about the technology sector, let alone the population in general.

The dataset has 4218 observations with features ranging 26 to 76, depending on the data collection year:

| Year | n | Questions n |
|------|------| ---------|
| 2014 | 1260 | 26 |
| 2016 | 1433 | 60 |
| 2017 | 756 | 76 |
| 2018 | 417 | 76 |
| 2019 | 352 | 76 |
|__Total:__| __4218__| - |

The features in the dataset can be summarized in the following categories:

1. __Socio-demographic questions__ – age, country, gender, race, etc.;
2. __Personal medical history__ – questions related to personal mental health, family diagnosis history, etc.;
3. __Organization-related questions__ – industry, company size, benefits provided;
4. __Employment questions__ - employment roles, status, etc.;
5. __Workplace culture and policy__– questions related to mental health support in workplace, benefits provided, sentiment of co-workers and supervisors, etc.

The full overview of questions can be accessed here: [Question mapping](https://scientific-splash-c94.notion.site/Questionnaire-mapping-ad670f918ad745e89362b8475181b5ba?pvs=4)

## 02 Data access 

The open source data is avalailable on Kaggle website. It should be downloaded and put into a project directory:

1. Download the `sqlite` database  [Here](https://www.kaggle.com/datasets/anth7310/mental-health-in-the-tech-industry)
2. Put the file in `~project_dir/dataset` folder in the directory
3. Make sure to install and import `sqlite` library. All required modules are listed in `requirements.txt` file

## 03 Repository contents

### Main file
The main file of data analysis and charting is a Jupyter Notebook file mental_health_tech.ipynb. The analysis is split into five parts:

1. Loading and cleaning a dataset;
2. Sociodemographics of the data;
3. Exploratory deep-dive;
4. Attempt at inference and counting disease prevalence;
5. Summary

### Requirements

The key requirements and dependencies are contained in requirements.txt file. Some of the prominent ones:

- `sqlite` module for reading SQL queries and loading tables onto dataframe;
- `pandas` library for data manipulation and analysis;
- `numpy` library adding support for large, multi-dimensional arrays and matrices;
- `matplotlib`, `seaborn` and `plotly` for charting and visualisation of the data;
- `statsmodels` for counting confidence intervals of data and other statistical parameters.