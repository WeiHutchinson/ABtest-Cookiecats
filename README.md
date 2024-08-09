### Project Description: Evaluating the Impact of Gate Placement on Player Retention in Cookie Cats

**Business Question:**  
In the mobile puzzle game *Cookie Cats*, players encounter gates that temporarily halt their progress, requiring them to either wait or make an in-app purchase to continue. The placement of these gates is crucial, as it can influence player retention and overall engagement. The primary question being addressed in this project is: **How does moving the first gate from level 30 to level 40 affect player retention, specifically 1-day and 7-day retention?**

**Approach:**  
To answer this question, an A/B test was conducted where a subset of players experienced the gate at level 30 (control group), while another subset encountered the gate at level 40 (test group). The analysis involves the following steps:

1. **Data Exploration:**  
   - The dataset includes player data such as the number of game rounds played and retention metrics for 1-day and 7-day periods.
   - Initial exploration involves checking the distribution of players across the two A/B groups and visualising the distribution of game rounds played.

2. **1-Day Retention Analysis:**  
   - Calculate and compare the 1-day retention rates between the two A/B groups to identify any initial differences.
   - Use bootstrapping to assess the uncertainty around the observed differences in 1-day retention rates. Bootstrapping involves repeatedly sampling the data with replacement and calculating retention for each sample, allowing for a more robust estimate of the difference.

3. **7-Day Retention Analysis:**  
   - Given that players may take longer to reach the first gate, it is also important to analyse the 7-day retention rates, which capture longer-term player engagement.
   - Similar to the 1-day retention analysis, bootstrapping is applied to evaluate the certainty of the observed differences in 7-day retention.

4. **Probability Assessment:**  
   - Calculate the probability that retention is higher when the gate is at level 30 versus level 40, based on the bootstrapped samples. This helps to quantify the likelihood that gate placement at level 30 leads to better retention.

5. **Conclusion:**  
   - The findings from the analysis will provide insights into whether keeping the gate at level 30 is more beneficial for retaining players compared to moving it to level 40.
   - The results will also consider the broader implications of gate placement on player experience and game enjoyment, using the concept of hedonic adaptation to explain why an earlier gate might help sustain player interest.

This project uses statistical analysis and bootstrapping techniques to provide data-driven recommendations on gate placement in the game *Cookie Cats*, aiming to optimise player retention and enhance overall game performance.
