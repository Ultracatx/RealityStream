[Industry Timelines Pipeline](../../../data-pipeline/timelines) - [RealityStream](../../)

# Industries Input Data

**Our primary CoLab:**
[Run Models](https://colab.research.google.com/drive/1zu0WcCiIJ5X3iN1Hd1KSW4dGn0JuodB8?usp=sharing) (Includes XGBoost) - Merges Features with Targets based on parameters.yaml
Backup and run locally @ models/Run-Models-bkup.ipynb

**Initial Python** (matched Streamlit)
models/reality-or-fiction/reality-or-fiction.ipynb

**Cool processes we're implementing in the Run Models CoLab**
- Toggle between pulling data from Github and local files
- Choose to send results to display, Github and/or local files
- Allow user to save their own Github account in local storage
- Build a yaml file from localStorage that the user can paste or pull into CoLab.
- Run data updates automatically quarterly with Github Actions, send a report

## Features Data

**Industry Features Data Prep:**
[Generate Industry Features](https://colab.research.google.com/drive/1HJnuilyEFjBpZLrgxDa4S0diekwMeqnh?usp=sharing) (All years)  
GitHub Output: [community-timelines/training/all-years](https://github.com/ModelEarth/community-timelines/tree/main/training/all-years)  
Source: [Community-Timelines](https://github.com/ModelEarth/community-timelines/tree/main/training/naics2/US/counties)  
Backup and run locally @ input/industries/features/industries-features-bkup.ipynb

## Target Data

**External Targets (Google Data Commons)**

[Tree Canopy improvements](https://model.earth/data-commons/docs/conservation/), Improvements in [Emissions](https://model.earth/data-commons/docs/air/) by state and country, [Honey Bee Populations](../../input/bees/).

**Industry Targets**

[Our Industry Targets Colab](https://colab.research.google.com/drive/1dbB9RHaJba7AyiGbGugzpui5F9v4bJOQ?usp=sharing) for Job Growth and Wage Growth. - Ronan

[Initial CoLab](https://colab.research.google.com/drive/1urO9phMMt0GyAXRsowf2dbLjQ6DlWTKf?usp=sharing) - moving into link above

<!--
Blank [Industry target CoLab](https://colab.research.google.com/drive/19ReOauJDQHPU2a_Fln8-Kcgsd566IYtQ?usp=sharing)
-->
**Job Growth** - Increase in local jobs for states and counties.
Features: types of industries, education levels, employment levels, population density, environmental indicators

**Wage Growth** - Increases in local pay levels
Features: types of industries, education levels, employment levels, population density, environmental indicators

TO DO: Load features/industries-features-bkup.ipynb from models/Run-Models-bkup.ipynb

TO DO: Add python to run external -bkup.ipynb files from within our Streamlit app.py files to build models and save reports.

## Merging Data in Pandas

Avoid saving large feature datasets in local files, use Pandas to merge features and targets while processing.

Send merged data through multiple models (rbf.py, etc.)


