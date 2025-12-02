# Top-n mtcars Explorer

## Description
An interactive Shiny application that lets users explore the classic `mtcars` dataset by ranking cars based on any numeric variable (e.g., mpg, hp, wt). Users can dynamically select a variable and choose how many top-performing cars to visualize. The app displays both a barchart and a sortable data table for quick comparison and exploratory analysis.

This mini-project demonstrates reactive programming in Shiny, tidy data manipulation, and dynamic visualization using **ggplot2**.

**Live App:** https://yuanying.shinyapps.io/stat133shiny_yuan_ying/

<img src="https://github.com/YennyYing/stat133_shinyapp3/blob/main/top1.jpg">

## Author
Yuan Ying  

## Date
Spring 2024

---

## How It's Made:

**Tech used:** R, Shiny, tidyverse, ggplot2

This app follows a simple but effective interactive data analysis workflow:

**1. Data Preparation**

Enhanced the built-in `mtcars` dataset by converting rownames into a proper column (`model`).

Cleaned and reorganized data to support reactive selection and ranking.

**2. Reactive Ranking Logic**

A Shiny reactive expression computes the top-n cars based on the user-selected variable.

The sorting is dynamic, updating instantly when the user changes the variable or slider.

**3. Visualization & UI**

A customizable barchart built with `ggplot2` displays the highest-ranking cars.

A data table allows users to inspect exact values and compare models.

A clean, minimal UI with dropdown selection and slider controls for smooth exploration.


## Features
- Choose any numeric variable in `mtcars` (mpg, hp, disp, wt, etc.)
- Interactively select the number of top models to display
- Auto-updated bar chart of the top-n cars
- Sortable data table for value comparison
- Built with tidyverse and Shiny’s reactive framework

---

## Packages
```r
library(shiny)
library(tidyverse)
```
## Lessons Learned:
This project strengthened my understanding of:
- Reactive expressions and how they optimize Shiny performance
- Integrating tidyverse pipelines within reactive logic
- Building clean, user-friendly Shiny interfaces
- Dynamically generating visualizations that respond to user input

Even though the dataset is small, this app demonstrates the core ideas behind interactive dashboards—reactive computation, tidy data transformation, and effective visualization—ideas that scale to more complex data science applications.


