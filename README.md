[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/UUgKTvv0)
# DA 351 Lab 1: Exploratory Data Analysis 

## Assignment Summary 

For this project, students will use Python code (specifically Pandas) to conduct Exploratory Data Analysis (EDA) on a dataset of Airbnb listings in the Columbus area. This is an individual assignment 
where students will communicate ideas through a mxture of writing and Python code in the form of a Jupyter Notebook (`.ipynb`) file, as well as a static page (`.html`) version that you will turn in on Canvas. Students will be evaluated based on the quality of their technical implementations and their writing.

## Learning Goals

This assignment asks students to fulfill the following learning goals:

1. Demonstrate the ability synthesize tabular data competencies from DA 101 and DA 210 
2. Use tidy data structures and the split-apply-combine strategies in Python (using Pandas) to perform effective manipulations of your data, and support such code, where appropriate, with idiomatic Python
3. Prepare to use Python to support data analytics workflows, including loading and manipulating data, implementing machine learning models, evaluating model performance, and gaining interpretive insights from a model's predictions.     
4. Effectively communicate what we have learned using code, visuals, and text, culiminating with a polished `.html` report document
5. Use Github for collaboration and version control to generate and document reproducible code

These learning goals are crucial to advanced descriptive methods in data analytics because they are all foundational skills upon which the bulk of our work for the class is based. 

## Assignment Files

To get started on this assignment, you will visit the Github Classroom link and follow the assignment checkout process for individual assignments. The Github Classroom link will be shared on Canvas. Assignment files include this README.md, the assignment dataset, and a Jupyter Notebook assignment template  (`submission.ipynb`).

Some of you may recognize the assignment dataset, as it is drawn from a commonly taught DA 101 lab that asks students to train and evaluate a linear regression model using data for Airbnb listings in the Columbus area. There are several version of the original assignment, but the most common aspects of that assignment include cleaning up the data, displaying maps of the listings, forming a hypothesis about a variable that might best predict a listing's price, and testing your hypothesis using a linear regression model. All aspects of the DA 101 lab are conducted in R using the `dplyr` package, so it makes sense for us to test our knowledge by seeing if we can perform many of the same tasks using `pandas`.

## Assignment Components

The core task of this assignment is to load Columbus listings and landmarks datasets using pandas, perform a range of pandas operations to make the data tractable, and to use exploratory data analysis (EDA) methods (e.g., descriptive statistics and data visualizations) to tell a data-driven story about the dataset.

Your submission will mix Python code and markdown text to tell a compelling story focused on a topic or question. You will create your narrative using a Jupyter Notebook file, and you will submit your work in `.html` format on Canvas. 

Submissions should have the following components: 

| Component        | Description                                       |
|------------------|---------------------------------------------------|
| Title            | Brief and informative, gives some idea of your core question or topic area. This block should also include student names and the date of the submission.|
| Introduction     | Include core background information and ethical considerations relevant to your use of the data. Articulate a core area focus.|
| Data Exploration | Use a blend of descriptive statistics and data visualizations to explore your core area focus. Include code blocks.|
| Uses of Python   | Take a step back and analyze your own use of code. Provide some rationale for choices you've made. Considerations may include performance, human readability, code dependencies, and reproducibility.|
| References       | List all works cited and consulted. Use proper APA format. (Note that this assignment does not require outside sources, but all sources you draw upon must be given proper credit.)|

__Technical Components:__

In your submission, you are required to include the following:

- use pandas to read Airbnb listings (`Columbus_listings.csv`) into your Jupyter Notebook as a DataFrame
- convert all price information columns to float types by removing special characters, dollar signs, etc.
- use pandas for most or all data transformations
- use pandas' `apply` method at least once to transform or create a variable  
- use pandas' `.loc`, `iloc`, or `.at` to filter data
- use three of the following in pandas: `sort_values`, `reset_index`, `set_index`, `fillna`, `dropna`, `astype`,  `rename`, `drop`, `head`, `tail`, `describe`, `cut` (or `qcut`) 
- use pandas `groupby` with an aggregation method (`agg`, `count`, `first`, `max`, `sum`, `mean`, etc.)
- display inline at least three different visualization types, such as one histogram, one scatter plot, one line plot, one boxplot or sequence of boxplots, etc.
- use at least one text manipulation method (python standard, regex) to convert one of the raw text fields into nominal or continuous data that can be analyzed or visualized

You are also encouraged __but not required__ to try these more difficult tasks:

- use pandas to load the second CSV file (`cbus_landmarks.csv`), which conatins some Columbus area landmarks and their locations
- merge the two data files so that the distance from each listing to each landmark can be calculated
- implement Vincenty Ellipsoid Great Circle Distance or Haversine Formula Great Circle Distance to calculate the distance from each listing to each landmark
- add a column representing, for each Airbnb listing, the distance from that listing to its nearest landmark

You are __strongly encouraged__ to complete all required tasks before attempting the more difficult ones! 

## Assessment Criteria 

Submissions will be evaluated on technical content; research and writing; and how well the submission comes together as a whole. The following descriptive rubric will be used when grading.

### Technical Content

- data files imported properly 
- attention is paid to the complexities of the source data (missing data, coded values, sample weighting, etc.)
- pandas operations and any helper functions are used properly
- submission uses all required code components correctly
- data visualizations are properly coded, sufficiently polished, and used effectively

### Research and Writing

- sufficient attention has been paid to proofreading
- the project is well organized, flows logically, and follows the all formatting guidelines
- the submission's use of language is appropriate for a well-informed, less technical reader

### Big Picture 

- all materials are turned in on time and in the right place
- assignment directions are followed, and all required components are included in the submission

## Assignment Specifications

__Accessing assignment files:__ via Github Classroom (linked on Canvas site)

__Required files:__ Jupyter Notebook (`.ipynb`) file and .html` version (using "Download as" feature)

__How to turn it in__: Upload `.html` file on Canvas; upload Jupyter Notebook (`.ipynb`) file and any imported `.py` files to Github. 

__Deadline:__ By 11:59 p.m. on Sunday, January 28, 2024.

