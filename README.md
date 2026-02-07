### Video Game Sales Analysis


## Overview

This project analyzes historical video game sales data to identify patterns and trends based on platform, genre, region, and ratings. Using Python and popular data science libraries (Pandas, NumPy, Matplotlib, Seaborn, SciPy), the study investigates:

Top-selling platforms and genres per region

The influence of ESRB ratings on sales

Correlation between critic/user scores and total sales

Comparative analysis of platforms and genres through hypothesis testing

The goal is to provide actionable insights for game developers, marketers, and analysts.

## Data

The dataset includes the following key columns:

Column	Description
name	Name of the game
platform	Platform (console)
year_of_release	Release year
genre	Game genre
publisher	Publisher of the game
na_sales	Sales in North America (millions)
eu_sales	Sales in Europe (millions)
jp_sales	Sales in Japan (millions)
other_sales	Sales in other regions (millions)
critic_score	Critic review score
user_score	User review score
rating	ESRB rating
###  Methodology

# Data Cleaning

Removed rows with missing game names

Filled missing ratings with "Unknown"

Converted year to numeric and extracted as integer

Calculated total sales across all regions

# Exploratory Data Analysis

Distribution of sales over time by platform

Top platforms and genres in recent years

Analysis of critic and user scores

# Regional Analysis

Sales distribution by platform, genre, and rating in NA, EU, and JP

# Hypothesis Testing

Compared user scores between platforms (XOne vs PC)

Compared average sales between genres (Action vs Sports)

Levene's test was applied to check equality of variances before t-tests

# Key Findings

Platforms with highest sales vary by region:

NA: X360, PS2, Wii

EU: PS2, PS3, X360

JP: DS, PS, PS2

Genres differ by region:

NA & EU: Action, Sports, Shooter

JP: Role-Playing

Critic scores are a better predictor of sales than user scores

Some genres/platforms have comparable performance; differences depend on region and market trends

# Libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import scipy.stats as st

## How to Run

Clone this repository:

git clone https://github.com/<your-username>/video-game-sales-analysis.git


Navigate to the folder:

cd video-game-sales-analysis


Install required libraries (if not already installed):

pip install pandas numpy matplotlib seaborn scipy


Open the Jupyter Notebook and run all cells.
