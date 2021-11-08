# Nordcloud Machine Learning Engineer recruitment excercise solution
This repository contains an attempt at solving the Nordcloud Machine Learning recruitment task. The description of the task was provided as specified in the following sections. This repository contains both the CSV file with prediction results for the test dataset (unseen data), as well as a Jupyter Notebook where the full code and a detailed description of the reasoning is provided.  

## Problem Statement
During this phase of the recruitment process, your task is to use the digital marketing campaign to log
level data in order to score entries according to their likelihood of being attributed as a click event.
You will be evaluated on your ability to predict click events and also to explain the rationale behind
your methodology: the methods used and the extracted relevant output.

## Data Description

A dataset with 463.291 entries from a 2021 online advertising campaign is provided.
The training set pertains to the time period of 9.04.2021 - 12.04.2021, while the test set only
contains the day of 14.04.2021.

The training set consists of the following attributes:

1. **Session Id** – refers to session identifier
2. **DateTime** – refers to date and time of the entry
3. **User Id** – refers to the user identifier
4. **Product Type** – refers to the product type
5. **Campaign Id** – refers to the campaign identifier
6. **Webpage Id** - refers to the webpage identifier
7. **Product Category** – refers to the product category
8. **Advertisement Size** – refers to the advertisement size
9. **User Depth** - refers to user’s duration of exposure to the advertisement during the respective entry (`3` being the longest, `1` being the shortest and `NA` being the inability to measure the time spent)
10. **Internet Browser Id** – refers to the identifier of the Internet browser type and version
11. **Gender** – refers to the gender
12. **Age Group** – refers to the age group
13. **City Size** – refers to the city size
14. **Device Used** – refers to the device used (could be Mobile or PC/Laptop)
15. **Clicked** – refers to the fact that the user clicked on the advertisement
16. **Interested in Cars** - refers to the fact that the person is interested in cars

17. **Interested in Food** - refers to the fact that the person is interested in food
18. **Interested in News** - refers to the fact that the person is interested in news
19. **Interested in Technology** - refers to the fact that the person is interested in technology
20. **Interested in Medicine** - refers to the fact that the person is interested in Medicine
21. **Interested in Politics** - refers to the fact that the person is interested in Politics
22. **Interested in Fashion** - refers to the fact that the person is interested in fashion
23. **Interested in Astronomy** - refers to the fact that the person is interested in Astronomy
24. **Interested in Animals** - refers to the fact that the person is interested in animals
25. **Interested in Travel** - refers to the fact that the person is interested in travelling

## Scoring and Evaluation
In order to be evaluated for this task, please send your solution as a `.py` or a `.ipynb` file and also a
`.csv` file with two columns: `Session Id` and `Clicked`. The first column in the ensuing `.csv` file
should match the column of the same name in the submission file provided. We will use these
identifiers to match your entries to the reference ones. The identifiers should be the same as those
used in the original file. Additionally, in the event of a smaller number of rows than in the original file,
the score will be 0.
The second column should be a numeric column consisting of float values between 0 and 1, which
represent the probabilities of successful click events. The aforementioned being valued as follows: `1`
meaning that the entry will definitely have a click attributed to it, while `0` meaning there is no chance
of a click happening.
