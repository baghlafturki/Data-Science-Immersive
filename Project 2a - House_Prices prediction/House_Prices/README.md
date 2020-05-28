# Project 2 - Kaggle Challenges with Titanic Survival (Classification) and House Prices (Regression)

Welcome to Project 2! It's time to start EDA and modeling.

**Primary Learning Objectives:**
1. Creating and iteratively refining a regression model and classification model on two popular getting started datasets
2. Using [Kaggle](https://www.kaggle.com/) to practice the modeling process and document findings on Kaggle Kernels
3. Learn from community resources on the platform and collaborate with a physical team

Here are the two competitions you will be joining:

[House prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

[Titanic](https://www.kaggle.com/c/titanic)

Your deliverables are 2 public kernels (one for each competition) on Kaggle per team.

## Set-up

Here are some starting steps:

1. Sign up for an account on [Kaggle](https://www.kaggle.com/)
2. Join the 2 competitions
3. Form a team with the members assigned to you
4. Look at tutorials section of each competition to get started. 
5. Inspect the data.
6. Read about the evaluation metrics.
7. Create a new kernel each under the respective competition (data automatically imported) and start collaborating with your team (under sharing setting). Remember to commit often and submit often to iterate on your models.
8. Regression is due the Sunday of week 6 (30 March) and Classification is due that next Monday (6th April).

_NOTE_: At the moment, the new collaborative feature of Kaggle in-browser kernels only support commiting versions without the capability to "pull" to your draft. For a smooth collaborative workflow, we recommend a repo on GitHub Enterprise to collaborate with your team through a commit/push/pull/merge flow.

Some advanced usage of Kaggle kernel via Kaggle API: https://github.com/Kaggle/kaggle-api

## The Modeling Process

1. You need to retrieve your data from the respective data links on the competitions.
2. Generate your regression/classification model using the training data. We expect that within this process, you'll be making use of:
    - train-test split
    - cross-validation / grid searching for hyperparameters
    - strong exploratory data analysis to question correlation and relationship across predictive variables
    - code that reproducibly and consistently applies feature transformation (such as the preprocessing library)
3. Predict the values for your target column in the test dataset and submit your predictions to Kaggle to see how your model does against unknown data.
    - **Note**: Kaggle expects to see your submissions in a specific format. Check the challenge's page to make sure you are formatting your CSVs correctly!
    - **You are limited to models you've learned in class**. In other words, you cannot use XGBoost, Neural Networks or any other advanced model for this project.
4. Evaluate your models!
    - consider your evaluation metrics
    - consider your baseline score
    - how can your model be used for inference?
    - why do you believe your model will generalize to new data?

## Submission

Your submission will be the link to the 2 published Kaggle kernels per team, one for each competition.

There will be a form that collects the links.

---

## Rubric
Your instructors will evaluate your project (for the most part) using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

**Scores will be out of 24 points based on the 8 items in the rubric.** <br>
*3 points per section*<br>

| Score | Interpretation |
| --- | --- |
| **0** | *Project fails to meet the outlined expectations; many major issues exist.* |
| **1** | *Project close to meeting expectations; many minor issues or a few major issues.* |
| **2** | *Project meets expectations; few (and relatively minor) mistakes.* |
| **3** | *Project demonstrates a thorough understanding of all of the considerations outlined.* |

### The Data Science Process

**Problem Statement**
- Is it clear what the student plans to do?
- What type of model will be developed?
- How will success be evaluated?
- Is the scope of the project appropriate?
- Is it clear who cares about this or why this is important to investigate?
- Does the student consider the audience and the primary and secondary stakeholders?

**Data Cleaning and EDA**
- Are missing values imputed appropriately?
- Are distributions examined and described?
- Are outliers identified and addressed?
- Are appropriate summary statistics provided?
- Are steps taken during data cleaning and EDA framed appropriately?
- Does the student address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA?

**Preprocessing and Modeling**
- Are categorical variables one-hot encoded?
- Does the student investigate or manufacture features with linear relationships to the target?
- Have the data been scaled appropriately?
- Does the student properly split and/or sample the data for validation/training purposes?
- Does the student utilize feature selection to remove noisy or multi-collinear features?
- Does the student test and evaluate a variety of models to identify a production algorithm (**TRY AT LEAST:** linear regression, lasso, and ridge, KNN, Logistic Regression, Decision Trees, Ensembles)?
- Does the student defend their choice of production model relevant to the data at hand and the problem?
- Does the student explain how the model works and evaluate its performance successes/downfalls?

**Evaluation and Conceptual Understanding**
- Does the student accurately identify and explain the baseline score?
- Does the student select and use metrics relevant to the problem objective?
- Is more than one metric utilized in order to better assess performance?
- Does the student interpret the results of their model for purposes of inference?
- Is domain knowledge demonstrated when interpreting results?
- Does the student provide appropriate interpretation with regards to descriptive and inferential statistics?

**Conclusion and Recommendations**
- Does the student provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?
- Does the conclusion answer the original problem statement?
- Does the student address how findings of this research can be applied for the benefit of stakeholders?
- Are future steps to move the project forward identified?

### Organization and Professionalism

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the kernel provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files & directories organized correctly?
- Are there unnecessary files/libraries included?
- Do files and directories have well-structured, appropriate, consistent names?

**Visualizations**
- Are sufficient visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Are plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Does the code follows general best practices and style guidelines?
- Are Pandas functions used appropriately?
- Are `sklearn` methods used appropriately?

### REMEMBER:

This is a learning environment and you are encouraged to try new things, even if they end up failing. While this rubric outlines what we look for in a _good_ project, it is up to you to go above and beyond to create a _great_ project. **Learn from your failures and you'll be prepared to succeed in the workforce**.
