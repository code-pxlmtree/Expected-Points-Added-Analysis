# Expected-Points-Added-Analysis
Expected points added is a metric in American Football analytics for calculating how much a specific play contributed to a team's chance of winning. The 2 main ways to score points and win games being 1. Passing the ball and 2. Running the ball. We will use the 2022 NFL Season's play by play data in order to answer a couple of questions regarding expected points added relative to passing and rushing.

## Key Questions
1. Is the relationship between passing EPA vs rushing EPA positive or negative?
2. How did the teams with high passing EPA and high rushing EPA perform during the season?
3. Are there any outliers?
4. What is the correlation between passing EPA vs rushing EPA?

### Dataset
The data was imported from the nfl_data_py library which is available on Jupyter Notebook. The library can be installed using the command prompt: _pip install nfl_data_py_.

### Data Cleaning
After importing the data. I made sure to choose only the data that was necessary for my analysis. Code is available in the passing_epa_vs_rushing_epa_ipynb attached to this repository.

### 1. Passing EPA vs Rushing EPA
<img width="1120" height="704" alt="Screenshot (196)" src="https://github.com/user-attachments/assets/2099d1ea-047c-4ea1-8300-eb77667d35fa" />

We clearly see that the relationship between Passing EPA and Rushing EPA is positive, as the regression line is on an upward slope. Hinting that when Passsing EPA increases, so does Rushing EPA, and vise-versa. In simple terms this might indicate that when a team is great at passing the ball, the box (Area near the line of scrimmage) gets lighter as the defense allocates players to guard the explosive pass plays, thus freeing up space for running backs when they run the ball. 

### 2. High Passing EPA/High Rushing EPA Team Performance
Here is a plot allocating the teams to their designated plot in the data:
<img width="1082" height="760" alt="Screenshot (197)" src="https://github.com/user-attachments/assets/fd8e0e66-ddb9-4c47-b450-21175d638c60" />


