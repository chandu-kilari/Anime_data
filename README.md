# Anime Dataset Analysis

## Overview
This project involves analyzing a dataset of anime from 2023 to uncover trends, insights, and relationships within the data. Python was used for data cleaning, exploration, and answering specific analytical questions.

---

## Key Insights

### 1. Longest Synopsis
- **Question:** Which anime has the longest synopsis?  
- **Answer:** `<Fangyu Quan Kai>`  
- **Method:** Used the `str.len()` function to calculate the length of the 'Synopsis' column and identified the maximum.

---

### 2. Average Score of Studio Ghibli Anime
- **Question:** What is the average score of anime produced by Studio Ghibli?  
- **Answer:** 6.79 (excluding 'UNKNOWN' scores).  
- **Method:** Filtered rows containing 'Studio Ghibli' in the 'Studios' column, excluded 'UNKNOWN' scores, and calculated the mean.

---

### 3. Unique Anime Titles Starting with 'A'
- **Question:** How many unique anime titles start with the letter 'A'?  
- **Answer:** 666  
- **Method:** Filtered rows where 'English name' starts with 'A' and counted the unique titles.

---

### 4. Year with the Most Anime Releases
- **Question:** Which year had the highest number of anime releases?  
- **Answer:** 2021  
- **Method:** Converted the 'Aired' column to datetime, extracted the year, and counted occurrences for each year.

---

### 5. Genre with the Highest Average Episodes
- **Question:** Which genre has the highest average number of episodes?  
- **Answer:** `<Fantasy>`   
- **Method:** Split the 'Genres' column into individual genres, calculated the mean number of episodes for each genre, and identified the maximum.

---

### 6. Most Members for R-17+ Rated Anime
- **Question:** Which anime has the highest number of members and is rated 'R-17+'?  
- **Answer:** `<Shingeki no Kyojin>`  
- **Method:** Filtered rows with 'R-17+' in the 'Rating' column and identified the anime with the maximum 'Members'.

---

### 7. Highest Score with Less Than 1000 Members
- **Question:** Which anime has the highest score with fewer than 1000 members?  
- **Answer:** `<Little Susie and Marvy>`   
- **Method:** Filtered rows with fewer than 1000 'Members' and excluded those with 'UNKNOWN' scores, then found the maximum score.

---

### 8. Top 5 Most Common Genres
- **Question:** What are the top 5 most common genres and their counts?  
- **Answer:**  
  - Comedy: 7,142  
  - Fantasy: 5,306  
  - UNKNOWN: 4,929  
  - Action: 4,730  
  - Adventure: 3,842  
- **Method:** Exploded the 'Genres' column to separate multiple genres into individual rows and counted occurrences.

---

### 9. Correlation Between Popularity and Favorites
- **Question:** What is the correlation between 'Popularity' and 'Favorites'?  
- **Answer:** -0.163 (weak negative correlation).  
- **Method:** Calculated the Pearson correlation coefficient using the `corr()` function.

---

## Technologies Used
- **Programming Language:** Python  
- **Libraries:**
  - `pandas` for data manipulation
  - `numpy` for numerical computations
  - `matplotlib` and `seaborn` for visualization (optional for trends)

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy
   ```
3. Run the script/notebook to reproduce the analysis.

---
