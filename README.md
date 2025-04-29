# Multilevel Modeling for UX Research (Fabricated Data Example)

This repository demonstrates how multilevel (mixed-effects) models can be applied in UX research, using fabricated but naturalistic task completion data.  
It shows why flattening the data (simple averaging) can hide important user differences, and how multilevel modeling offers a more accurate and detailed picture.

## Project Structure

- **Fabricated Dataset:** Simulated UX task times for participants using two designs (Old vs New).
- **Multilevel Model:** Random intercept model to account for repeated measurements within participants.
- **Visualizations:**
  - Boxplot with individual user points (flattened view)
  - Participant-level trajectories (multilevel view)
  - Histogram of improvement across users
  - Side-by-side plot comparing flattened vs multilevel approaches
- **Outputs:** High-quality, transparent PNG files ready for LinkedIn carousel posts, teaching, or presentations.

## Why Multilevel Modeling?

In UX research, repeated measures (like task performance across different designs) are common.  
Traditional methods like t-tests or simple linear regression often **flatten** the data, ignoring individual variability.  
Multilevel modeling respects the nested structure of UX data - allowing users to have their own baseline and improvement pattern while still estimating the overall design effect.

## Key Libraries Used

- `tidyverse`
- `lme4`
- `broom.mixed`
- `ggplot2`
- `patchwork`
- `ggrepel`
- `gridExtra`

## How to Reproduce

1. Clone the repository.
2. Open the `.Rmd` file or `.R` script.
3. Run the code to simulate the data, fit the models, and generate the visualizations.
4. Output plots are saved automatically in `.png` format with transparent backgrounds.

## Example Plots

- **Boxplot:** Task times across Old and New designs with visible individual variation.
- **Trajectory Plot:** Each participant’s change from Old to New.
- **Histogram:** Distribution of improvements (Old minus New times).
- **Comparison Plot:** Flattened vs Multilevel views side-by-side.


## Acknowledgment

Inspired by *Martin Schmettow's* book  
*New Statistics for Design Researchers: A Bayesian Workflow in Tidy R* (Springer, 2021).

---
