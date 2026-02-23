# How the NBA Became a 3-Point League

STAT 3280 Final Project  
Author: Thad Felten  

## Overview

Over the past several decades, the NBA has undergone a major strategic transformation. While common explanations for modern offensive growth focus on pace or improved shooting efficiency, this project investigates a different hypothesis: that the true shift lies in how teams allocate shots, particularly the rise of the three-point attempt.

This analysis traces how three-point adoption reshaped offensive strategy and evaluates whether leaning into the three-point shot is associated with winning in the modern NBA.

---

## Central Question

In the modern NBA, is increased three-point volume associated with winning?

---

## Analytical Structure

The project progresses through five stages:

1. **League-Wide Offensive Transformation**
   - Trends in offensive rating (points per 100 possessions)
   - Evaluation of pace and true shooting percentage over time
   - Demonstration that efficiency gains are not fully explained by these traditional metrics

2. **The Rise of the Three-Pointer**
   - Historical growth in three-point attempt volume
   - Transition from a marginal strategy to a central offensive feature

3. **Team-Level Divergence**
   - Season-normalized (z-score) three-point attempt rates
   - Era-separated analysis of three-point volume vs. win percentage
   - Binned comparisons of win distributions by three-point volume
   - Increasing strategic variance across teams

4. **Player-Level Adaptation**
   - Usage rate changes by position over time
   - Shifts in guard, wing, and big responsibilities
   - Role evolution supporting perimeter-focused offenses

5. **Championship Profiles**
   - Comparison of champions vs. league averages
   - Evidence that modern champions typically pair strong defense with elevated three-point volume

---

## Key Findings

- Offensive improvement is not primarily driven by pace or raw shooting efficiency.
- The major shift is in **shot allocation toward higher-value attempts**, especially three-pointers.
- In earlier eras, three-point volume was weakly associated with winning.
- In the modern era, higher three-point attempt rates are clearly associated with stronger win percentages.
- Most champions since 2000 attempt more threes than league average.
- The modern NBA became more efficient by prioritizing shot value, not simply by playing faster or shooting better.

This project emphasizes association rather than causation and discusses potential confounding factors such as roster talent and player skill.

---

## Implementation

- R and R Markdown
- Plotly for animated and interactive visualizations
- Shiny applications for team playstyle comparison
- Tableau for embedded visualizations
- Season-normalized metrics to account for league-wide contextual shifts

Interactive tools include:
- Team Playstyle Fingerprints (Shiny)
- NBA Team Comparison Tool (Shiny)

---

## Conclusion

The modern NBA did not become more efficient simply through increased pace or incremental shooting improvement. Instead, teams restructured offenses around higher-value shot selection, particularly three-point attempts. As this strategic shift accelerated, teams that embraced perimeter-oriented play more aggressively tended to see greater success.

The evolution of the league reflects strategic optimization rather than aesthetic change.
