**Cricket Analytics**
**About Dataset**
RCB Vs DC IPL 2024 Analysis: Dataset
The dataset we collected for this IPL match analysis contains the following columns:

- **team**: Indicates the batting team.
- **over**: Over number in the match.
- **batter**: The batsman facing the delivery.
- **bowler**: The bowler delivering the ball.
- **non_striker**: The batsman at the non-striker’s end.
- **runs_batter**: Runs scored by the batter off the delivery.
- **runs_extras**: Extra runs (like wides, no balls) conceded during the delivery.
- **runs_total**: Total runs scored from the delivery.
- **player_out**: Name of the player out on the delivery (if any).
- **wicket_kind**: Type of dismissal (if any).
- **fielders**: Names of fielders involved in the dismissal (if any).

**Analysis using Python**

Let's begin by visualizing the run distribution per over for both teams to illustrate the scoring trends throughout the innings:

![Figure_1](https://github.com/771salameche/Cricket-Analytics/assets/123024504/08188e77-005c-4b32-b294-3de886333aa5)

The plot above illustrates the run distribution per over for both teams. Here are some insights:

- The scoring rate for each team fluctuates throughout their innings, with spikes indicating overs with high scoring, likely due to boundaries or big hits.
- Royal Challengers Bangalore (RCB) appears to have a couple of overs with significantly higher runs, suggesting aggressive batting.

Next, I will analyze the top scorers from each team to highlight individual performances. Let's create a bar chart to visualize the top contributors in terms of runs:

![Figure_2](https://github.com/771salameche/Cricket-Analytics/assets/123024504/40fd689d-8b40-412c-82ec-09bc34b1341f)

Key observations from the graph include:

- AR Patel from Delhi Capitals is the top scorer of the match, significantly outscoring others with a little over 50 runs.
- RM Patidar is the top scorer for Royal Challengers Bangalore, closely approaching 50 runs.
- The graph shows a diverse contribution from both teams, with several players from both sides contributing notable scores.

Now, let’s move on to a bowling analysis. We’ll look at which bowlers took the most wickets and their economy rates. This will involve calculating the number of wickets each bowler took and the number of runs they conceded per over bowled. We’ll present this data in a combined bar and line plot for a comprehensive view of bowling performance.

![Figure_3](https://github.com/771salameche/Cricket-Analytics/assets/123024504/4a5ea32d-65e4-4934-b010-920568f12789)

The combined bar and line plot provides a comprehensive overview of each team's bowling performance:

- **Wickets Taken**: The bars represent the number of wickets each bowler took during the match. The height of the bars indicates how successful the bowlers were in taking wickets. Bowlers from both teams contributed to wicket-taking, with some standout performances reflected by higher bars.
- **Economy Rate**: The overlaid line graph shows each bowler's economy rate (runs conceded per over). The economy rate is crucial as it indicates how economically a bowler has bowled in terms of runs given away.

Next, let's analyze the types of dismissals that occurred during the match to understand how most wickets were taken (e.g., caught, bowled, run out). This can provide insights into the nature of the pitch and the playing conditions. We’ll visualize this using a pie chart:

![Figure_4](https://github.com/771salameche/Cricket-Analytics/assets/123024504/f1b1927f-8bdc-4d13-8b5b-f792e1bbedc1)

Now, let’s analyze the batting partnerships by calculating and visualizing the most productive partnerships in the match. We’ll examine the runs scored per partnership and the duration of each partnership in terms of balls faced:

![Figure_5](https://github.com/771salameche/Cricket-Analytics/assets/123024504/e8e3e764-53db-4902-833b-79c672b53bc8)

The bar chart displays significant batting partnerships from the match, highlighting those that scored more than 20 runs. Here’s how these insights contribute to our analysis:

- The chart identifies key partnerships that likely had a substantial impact on the match’s outcome, illustrating the effectiveness of batting pairs.
- It provides insights into which players were involved in pivotal stands, helping to assess player form and team strategy.

Next, let’s conduct a Phase Analysis to examine how teams performed during different stages of their innings: Powerplay (first 6 overs), Middle overs (7-15), and Death overs (16-20). We’ll look at scoring rates and wicket loss during these phases. This can offer insights into the team’s tactical approach and execution under varying conditions.

![Figure_6](https://github.com/771salameche/Cricket-Analytics/assets/123024504/5cc97cbd-0701-4b77-b3ce-37189555325d)

The plot above breaks down the match into distinct phases—Powerplay, Middle, and Death—and illustrates each team's performance during these segments:

- **Powerplay**: Both teams scored relatively fewer runs, with RCB losing more wickets than DC, as indicated by the height of the orange line.
- **Middle**: This phase witnessed the highest run-scoring for both teams, with DC slightly outscoring RCB. The wickets lost remained controlled, indicating stable innings from both sides.
- **Death**: RCB experienced a significant drop in runs compared to the Middle phase, while DC maintained a high run rate. RCB also saw a notable increase in wickets lost during this phase, marked by the orange line peaking near 4.5, suggesting either a collapse or aggressive batting that didn't yield desired results.

Next, let’s delve deeper by examining how the strike rate varied with the game's phases for these top performers. This analysis could provide insights into strategic scoring and game dynamics across different innings stages:

![Figure_7](https://github.com/771salameche/Cricket-Analytics/assets/123024504/ca5b126d-4e1b-4a96-9573-aec8473c78f9)

The bar chart depicts how the strike rates of top performers varied across different phases of the match:

- J Fraser-McGurk shows a notably high strike rate in the Middle phase, surpassing all other phases and players. This suggests a highly aggressive and effective batting performance during this crucial part of the innings.
- V Kohli and RM Patidar demonstrate high strike rates in the Death phase, indicating their ability to accelerate scoring towards the end of the innings, crucial for setting or chasing targets.
- AR Patel maintains consistent strike rates in the Powerplay and Middle phases, slightly reducing but remaining competitive, highlighting his role as a steady opener or middle-order batsman.
- KV Sharma exhibits a lower strike rate in the Middle phase compared to others, implying a more cautious approach or challenges in accelerating scoring during this period.

Identifying Turning Points in the Match
To identify where Delhi Capitals (DC) may have lost momentum and Royal Challengers Bangalore (RCB) gained the upper hand, we'll analyze:

1. **Cumulative Run Rates Comparison**: Plot the cumulative run rates of both teams throughout the innings to pinpoint where RCB started to outpace DC significantly.
   
2. **Wicket Analysis**: Examine the timings and impacts of wicket falls on DC's scoring rate and momentum.
   
3. **High-Impact Overs**: Identify any overs where RCB took multiple wickets or DC had a notably low scoring rate, indicating potential shifts in momentum.

Let’s begin by plotting the cumulative run rate for both teams and overlaying the wicket events to identify critical moments in the match:

![Figure_8](https://github.com/771salameche/Cricket-Analytics/assets/123024504/03cce633-89e8-4d23-bac9-b410402157d5)

The plot illustrates the cumulative runs scored by each team throughout their innings, with markers indicating wickets:

- **Momentum Shifts**: Key points where wickets are lost are pivotal. Despite these setbacks, RCB's run rate line shows consistent progress without significant downturns, suggesting effective recovery by subsequent batsmen.
  
- **Performance Analysis**: RCB's ability to maintain a steady run rate despite losing wickets may indicate robust batting depth or successful innings pacing strategies. In contrast, while DC also increases their score, the rate of increase appears less steep, possibly indicating fewer high-scoring overs.

Next, let’s calculate the run rate for each over for both teams and examine how these rates changed throughout the innings, particularly focusing on the overs where wickets fell:

![Figure_9](https://github.com/771salameche/Cricket-Analytics/assets/123024504/b93323d7-d1b1-4037-bf43-472b02d62d1e)

The plotted run rates for each over, alongside the marked moments of wicket-taking (indicated by large dots), offer insights into the evolving dynamics of the match:

- **RCB Run Rate Fluctuations**: RCB’s run rate exhibits notable fluctuations, reaching peaks of around 3.5 runs per ball towards the end of the innings. The presence of wicket markers (red circles) indicates that wickets were taken during overs where the run rate generally dipped, which is typical as wickets often disrupt batting momentum.

- **DC Run Rate Patterns**: DC’s run rate starts strong but experiences a sharp decline after the initial overs, stabilizing somewhat in the middle before another surge and subsequent decline towards the end. Wickets (blue circles) are taken during overs where the run rate decreases, suggesting effective bowling periods from RCB during these phases.



**Summary**

The RCB vs DC match demonstrated a combination of strategic batting, aggressive bowling, and crucial partnerships. RCB's sustained higher cumulative run rate and timely wicket-taking in key overs were pivotal to their victory. The in-depth analysis of match phases and individual player performances not only underscores the nuances of T20 cricket but also provides insights into how momentum shifts and strategic decisions influence the game's outcome.







