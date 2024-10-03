
# T20 Cricket Analysis Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/75106b0a-f353-47ec-97fb-b9ea4cc082b4/ab53b99188e2678b772b?experience=power-bi

## Problem Statement

This dashboard helps cricket analysts and enthusiasts delve deep into the performance of players and teams during T20 cricket matches. It offers insights into crucial aspects such as batting, bowling, and fielding performance. By identifying key performance metrics like batting strike rates, bowling economy rates, and fielding efficiency, teams can utilize this data to refine their strategies and boost on-field performance.

Additionally, the dashboard highlights both strengths and areas for improvement in players and teams, providing a roadmap for success in high-stakes matches. The interactive capabilities of Power BI allow users to filter and analyze data based on specific players, teams, and match conditions, making this an essential tool for strategic decision-making.

### Steps Followed


- Step 1: Imported JSON data files containing T20 cricket match statistics.

- Step 2: Cleaned and preprocessed the JSON files using Python, converting them into CSV format.

- Step 3: Uploaded the cleaned CSV files into Power BI for further processing and analysis.

- Step 4: In Power BI, performed data profiling to check for errors, empty values, and column quality.

- Step 5: Null values were handled in fields such as “Batting Strike Rate” and “Bowling Economy,” ensuring they did not impact the analysis.

- Step 6: Visual filters (Slicers) were added for fields like “Teams,” “Players,” and “Match Venues.”

- Step 7: Key performance metrics such as "Batting Strike Rate," "Bowling Economy," and "Fielding Efficiency" were represented using custom visuals.

- Step 8: Bar charts were used to show the number of runs scored by players, wickets taken by bowlers, and catches held by fielders, segregated by match conditions and player categories.

- Step 9: Two card visuals were added to show the average number of runs scored per match and the average wickets taken per match.

- Step 10: Player performance metrics were calculated and visualized across various roles (batters, bowlers, all-rounders) and conditions (power play, death overs, etc.).

Steps for Data Refinement in Power BI : 

- Step 11: Calculated columns were created to categorize players into different performance tiers based on their stats.

- Step 12: New measures were created to calculate metrics such as total runs scored, total wickets taken, and player contributions in key matches.

- Step 13: A dynamic filter was used to allow users to filter player performances based on specific conditions such as match type, venue, and opposition.

### DAX Expressions

Total Runs Scored = SUM(T20_Cricket_Data[Runs Scored])

Total Wickets Taken = SUM(T20_Cricket_Data[Wickets Taken])

Player Strike Rate = (DIVIDE(SUM(T20_Cricket_Data[Runs Scored]), SUM(T20_Cricket_Data[Balls Faced])) * 100)

### Key Insights
Total Matches Analyzed: 500

1. Top Performers:

- Top 5 run-scorers and top 5 wicket-takers were identified, offering insights into player impact across different match conditions.

2. Batting Analysis:
- Average Strike Rate: 135.2
- Centuries: 12
- Half-Centuries: 85

3. Bowling Analysis:
- Average Economy Rate: 8.2
- Top Wicket-Takers: Player A (28 wickets), Player B (26 wickets)

4. Fielding Analysis:
- Average Catch Rate: 93%
- Top fielders were identified based on their number of catches and run-outs.


### Visualizations and Analysis :

1. Bar Chart: Displays a comparison of the top run-scorers across various matches, segregated by batting positions and conditions.
2. Line Chart: Shows the trends in economy rates of bowlers across different overs (power play, middle overs, death overs).
3. Pie Chart: Provides a breakdown of match results (win/loss) based on teams and includes insights into teams' performance while chasing or defending.
4. Custom Visuals: Key metrics such as "Batting Strike Rate," "Bowling Economy," and "Fielding Efficiency" were visualized using tailored visuals for easy comparison.

### Report Snapshot (Power BI DESKTOP)
![Screenshot (26)](https://github.com/user-attachments/assets/5e6caba8-534e-4c4b-a13a-17bcbfffbfa9).

![Screenshot (27)](https://github.com/user-attachments/assets/c7674499-e9e0-4182-b7fa-94fd652f0000)


### Insights

1. Batting Performance: 
- Players with the highest strike rates excel in the middle overs, helping to accelerate the scoring rate.
- The number of boundaries hit is a key metric in measuring overall team performance.

2. Bowling Performance:
- Bowlers with low economy rates during the death overs have a crucial impact on match outcomes, especially when controlling run rates is critical.

3. Fielding Performance:
- Efficient fielding plays a pivotal role, particularly in close matches, where a single catch or run-out can change the momentum.
