# ELECTIVE COURSE SELECTOR
Author: Johan Lindbjerg Skovbæk (s203801), MSc. Design & Innovation
\nContact: johan.skovbaek@gmail.com

© 2025 Johan Lindbjerg Skovbæk. All rights reserved.

_____________________________
### PURPOSE

The purpose of the Elective Course Selector tool is enabling students at the Technical University of Denmark (DTU) to easily identify and compare elective courses that fit their academic and practical demands.
In this alpha version, the tool has solely been developed for students at the master education of Design & Innovation.

_____________________________
### FURTHER DEVELOPMENT IDEAS

- Make applicable for all educations at DTU.
    1. Obtain a list of ALL courses taught at DTU (Contact DTU IT Service).
    2. Define relevance of a course for an education to assign it appropriate courses (consider combining a LLM with an API for analyzing the course descriptions).
    3. Run the "Data load.ipynb" script to obtain appropriate values.
    4. Make an educaiton-dropdown for the plot and adjust other aspect of the plot, i.e. categorization.

- Include the dataframe below the plot instead of the current setup (think excel style).
    - Should be used to ease the navigation and comparison between courses.
    - Should include the ability to sort the different values.
    - Should highlight the selected data point/course in the dataframe.

- Make a distribution chart for which educations are in each course.

_____________________________
### UPDATE GUIDE
If nothing fundamental changes, the tool can be updated each semester in accordance with the following guidelines:

Before you start, make sure that:
- You have Jupyter Notebook installed.
- You have Google Chrome installed (used for running selenium).
- Your computer doesn't go to sleep. The netscraping will run for a while, have patience :)

The new data should be:
- Placed in the folder "Data"
- Named "data_new.xlsx"
- Have these three columns with appropriate data (see "data_original.xlsx"): "Term", "Course code", "Passed DI"

Running the scripts:
- There are two notebook files (.ipynb) that should be run in this order:
    1. Data load.ipynb
    2. Tool creation.ipynb
- Each contain markdown titles called "Update info". Read those carefully and adjust the code.
- After this process, the plot file "Elective Course Selecter.html" should be updated and ready to be integrated on a website.

