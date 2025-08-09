## The 2024-2025 season MVP was robbed from Nikola Jokic


Let’s begin by defining what MVP means as the definition tends to be subjective in each conversation. In this article, the MVP will be defined as the Most Valuable Player in the league, meaning that the player is able to influence winning or losing the most in the league.

A common tool that is used to determine MVPs tend to be stats. We tend to look at stats in the upper percentile to even qualify for the MVP. For example, in the 2024-2025 NBA season, a common stat that would be brought up would be SGA led the league in scoring with 32.7PPG which ultimately contributed to the decision of him selected for 24/25 MVP.

Diving further into the 24/25 season, the MVP debate commonly landed between Jokic and Shai with the comparison of stats to back up the decision to choose one over the other. However, this system of comparison is ultimately flawed when it comes to dictating value, as inherently each metric holds a different weighting of importance when it comes to its contribution to winning. This is why almost all advance metrics such as game score, +/-, PER all have some kind of hyperparameter on each stat to determine value.

The easiest way to determine the effect of a stat on winning is to identify the correlation between them. Using the below formula for point biserial correlation:

$$
r_{pb} = \frac{M_1 - M_0}{s_n} \cdot \sqrt{\frac{n_1 n_0}{n^2}}
$$

**Where:**

- $r_{pb}$ = the correlation coefficient  
- $M_1$ = mean of the metric when there is a win  
- $M_0$ = mean of the metric when there is a loss  
- $s_n$ = standard deviation of the population  
- $n_1$ = number of datapoints given a win  
- $n_0$ = number of datapoints given a loss  
- $n_2$ = total number of datapoints 

<br>

We can identify the correlation between the following stats and winning:

| Stat  | r_pb    | p         |
|-------|---------|-----------|
| MP    | 0.1693  | 0.1283    |
| TS%   | 0.2863  | 0.009116  |
| eFG%  | 0.2647  | 0.01625   |
| ORB%  | 0.1928  | 0.08269   |
| DRB%  | 0.2514  | 0.02273   |
| TRB%  | 0.3022  | 0.005794  |
| AST%  | 0.2088  | 0.05974   |
| STL%  | 0.2650  | 0.01612   |
| BLK%  | 0.1720  | 0.1223    |
| TOV%  | 0.1237  | 0.2682    |
| USG%  | 0.1299  | 0.2448    |
| ORtg  | 0.3276  | 0.002663  |
| DRtg  | 0.0999  | 0.372     |
| GmSc  | 0.2512  | 0.0228    |
| BPM   | 0.2653  | 0.01599   |
| FG   | 0.1032   | 0.375      |
| FGA  | 0.0608   | 0.6017     |
| FG%  | 0.0872   | 0.454      |
| 3P   | 0.1350   | 0.2451     |
| 3PA  | 0.1870   | 0.1058     |
| 3P%  | 0.0299   | 0.7979     |
| 2P   | 0.0518   | 0.6567     |
| 2PA  | -0.0434  | 0.7096     |
| 2P%  | 0.1190   | 0.3058     |
| eFG% | 0.0994   | 0.393      |
| FT   | -0.0018  | 0.9877     |
| FTA  | -0.0377  | 0.7465     |
| FT%  | 0.1654   | 0.1561     |
| ORB  | 0.0525   | 0.6527     |
| DRB  | 0.1038   | 0.3721     |
| TRB  | 0.1108   | 0.3405     |
| AST  | -0.0597  | 0.6087     |
| STL  | 0.1461   | 0.208      |
| BLK  | 0.1412   | 0.2238     |
| TOV  | -0.2387  | 0.03783    |
| PF   | -0.1023  | 0.3791     |
| PTS  | 0.1068   | 0.3584     |
| GmSc | 0.1974   | 0.08748    |
| +/-  | 0.5885   | 2.262e-08  |
