# Note

The Jupyter notebook is not rendered correctly on github. Please use an **nbviewer** based service to view it. Example: https://kokes.github.io/nbviewer.js/viewer.html

You can copy paste the URL of **PyCitySchools_Challenge.ipynb** in the above to view it.

# Overview

In this exercise, we are provided with the data containing math and reading scores of all high schoolders for 15 schools in a county. Additionally, for each school, we are provided with the enrollment numbers and its allocated budget. The analysis exercise requires us to present the passing percentages for both reading and math (as well as overall), and analyze those passing percentages along different dimensions such as:

* Grade level (9th, 10th, 11th and 12th)
* Budget per student
* Enrollment numbers
* Type of school (district versus charter)

Ultimately, the goal of the exercise is to determine if any (or several) of the aforementioned factors influence the passing rate of the students.

# Methodology

We used the Jupyter notebook and Python's pandas module to analyze the data. In a nitshell, the pandas model provides us with:

* Dataframes: A fataframe is a table where each row is indexed. This is Excel's equivalent of a spreadsheet.
* Series: A series is a specific column from the dataframe, where each entry is indexed as well. This is Excel's equivalent of a column.

Using Python's pandas module and the Jupyter notebook gives us several advantages over using Excel. Some of them are listed below.
* Python is a widespread and a general purpose programming language with a lot of inbuilt support for various data structrutes (such as lists, tuples, dictionaries), string manipulation and offers many add-on packages. Python is superior to VBA (Excel's programming language) in that regard.
* Jypyter offers an integrated environment for coding and visualizing the output in a single pane.
* Jupyter and python are available for free.

## Working with datasets
We are given two datasets in the csv format. One containing schools and the second containing students. In total, there are 15 schools and 39,170 students. The first step is to load these datasets in pandas **dataframes**, and **join** them in a single dataframe (this is Excel's equivalent of Vlookup, or the sql equivalent of join). The key to join them on is the **school_name**.
