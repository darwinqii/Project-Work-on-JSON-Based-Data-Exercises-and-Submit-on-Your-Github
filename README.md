# Project-Work-on-JSON-Based-Data-Exercises-and-Submit-on-Your-Github
SpringBoard_Chapter 4 Data Wrangling_4.2_Working with data in files

****
## JSON exercise

Using data in file 'data/world_bank_projects.json' and the techniques demonstrated above,
1. Find the 10 countries with most projects
2. Find the top 10 major project themes (using column 'mjtheme_namecode')
3. In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.

## Approach
### Data Overview, and focus on the column 'mjtheme_namecode' for problem 2 and 3

### problem 1
count the times of entries for each country, and slice the first ten rows to get the top10 country with most projects.

### Problem 2:

Because there are different number of theme entries for project, we make a for loop to iter over every project this column, and record the occurance of every code number in a dict. Then we combine the dictionaries into a dataframe from sorting and output.

### Problem 3:
Approach: make a copy of the original dataframe,<br>
           iterate over the 'mjtheme_namecode' column in for loop, <br>
           and fill in the blacks with the 'name_dict' dictionary when solving Probelm 2

## Answer: Please see the file `sliderule_dsi_json_exercise.ipynb`
