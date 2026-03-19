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
Here is a graph allocating the teams to their designated plot in the data:

<img width="1082" height="760" alt="Screenshot (197)" src="https://github.com/user-attachments/assets/fd8e0e66-ddb9-4c47-b450-21175d638c60" />

Now we have more contect to the data as we see exactly which teams have an above average Passing EPA/Rushing EPA and which teams do not. There are 6 teams in the top right quadrant. These are the only teams in the league with above average figures in both metrics. These teams are the Kansas City Chiefs, San Francisco 49ers, Cincinati Bengals, Buffalo Bills, Philadelphia Eagles and the Miami Dolpins. Let us look at if these potent offenses helped translate these good offensive numbers into wins for their respective teams.

<img width="1542" height="737" alt="Screenshot (195)" src="https://github.com/user-attachments/assets/f04788a0-c05f-4e98-bbee-26db476da79a" />
image credit: https://www.nfl.com/standings/league/2022/reg

One thing that just jumps off the page, of the top 6 teams via win/loss record, 5 of them we mentioned prior as being above average in Passing EPA and Rushing EPA. The top 2, Kansas City Chiefs and Philadelphia Eagles, ended up being in the SuperBowl, with the Chiefs being victorious. So this clearly indicates that if your team is above average in both metrics, your team will perform very well, something coaches and GMs should take note of.

The only outlier in the group we mentioned are the Miami Dolphins. They made the playoffs, however they only had a record of 9 wins and 8 losses. With a point differential of -2. This indicates two possible scenarios, 1. The team has a bad defense that cannot prevent opposing offenses from scoring, thus offseting the Dolphin's offenses prowess. 2. The offense, though very potent in the Passing and Rushing EPA metrics, do not score enough in close games.

Graphic Key Note:
- "xz" - means the team clinched a playoff berth via winning their division
- "xy" - means the team clinched a playoff berth via wildcard

### 3. Data Outliers
An outlier of this data are the Chicago Bears, who posted the second highest rushing EPA, yet have a negative passing EPA. One way to explain this could be that the team is solely dependent on their running game because they don't have a competent throwing quarterback, thus inflating the runnng numbers.

### 4. Passing EPA vs Rushing EPA Correlation
<img width="731" height="269" alt="Screenshot (198)" src="https://github.com/user-attachments/assets/23d7a831-d9db-48fe-814e-3afca458e17a" />

The correlation coefficient between Passing EPA and Rushing EPA is 0.296578 which indicates that while there is a **weak positive relationship** between the two metrics. So, yes teams that are good at passing tend to me somewhat good at rushing, but this relationship isn't consistent. For one, the Minnesota Vikings, who won 14 games, have one of the best Passing EPAs, have one of the worst Rushing EPAs, showing that this is a pass-heavy team.

## Final Takeaways
1. Teams that are effective at passing the ball, tend to be affective at running it as well, probably due to the defense focusing on stopping explosive passes, leaving the offense more room to run the ball.
2. Passing EPA seems to be the more important metric as it provides more expected Expected Points Added than rushing. However, teams should still make it a point to run the ball in order to get easy yards and keep the defense honest. In this way the passing game sets up the running game 
3. Teams should make it a priority to have a good passing and rushing offense. The teams that suceeded in both not only made the ployoffs, but also made deep playoff runs. Something general managers and coaches should take into account when buildng their teams.

## Conclusion
When building teams, and strategising for the offense, one thing s blatantly obvious, **balance is key**. In the strategic and physical beautiful game that is the National Football League, the team that is able to find this balance in the passing and rushing game, gives themselves the best chance to win a Vince Lombardi trophy.

## References
_Eric A. Eager and Richard A. Erickson (2023) Football Analytics with Python & R. Sebastopol, CA: O’Reilly Media._
