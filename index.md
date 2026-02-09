# Court Reminder Experiment
**Designing and evaluating reminder interventions to reduce missed court appearances**

## Overview
People often miss court appearances not because they are unwilling or defiant, but because court systems are confusing, intimidating, and easy to forget. When a court date is missed, the consequences can include arrest warrants, detention, and cascading harms, especially on low-income individuals. This project documents the design and decision-making process behind a large-scale court reminder field experiment currently in recruitment and pre-implementation.

## Problem Statement
Traditionally, failure to appear (FTA) in court and missed dates is viewed as willful noncompliance. This framing overlooks a critical reality, that court systems are complex, intimidating, and poorly designed for the people navigating them. 

This project reframes FTA as a usability problem and investigates whether reminder intervention, particularly frequency of those reminders, can help individuals successfully attend court. However, evaluating such interventions through a randomized controlled trial introduces an ethical challenge. A traditional RCT requires a control group that receives no treatment, which in this context could expose individuals to avoidable harm, including arrest warrants and detention.

To address this concern, we employ a stepped-wedge randomized experiment that ensures all participants will eventually receive reminders while still allowing for causal evaluation. This approach enables us to study how reminder presence and frequency affect court attendance, while respecting ethical constraints inherent to the justice system. 

## Research Questions
1. Do reminder messages reduce failure to appear?
2. How does **frequency** of reminders affect outcomes?
3. How can we evaluate these interventions ethically in real court settings?

## Study Design
| Group   | Period 1 | Period 2 | Period 3 | Period 4 | Period 5 | Period 6 | Period 7 |
|---------|----------|----------|----------|----------|----------|----------|----------|
| Group A | 0        | 1        | 1        | 2        | 2        | 3        | 3        |
| Group B | 0        | 0        | 1        | 1        | 2        | 2        | 3        |
| Group C | 0        | 0        | 0        | 1        | 1        | 2        | 2        |
| Group D | 0        | 0        | 0        | 0        | 1        | 1        | 2        |
| Group E | 0        | 0        | 0        | 0        | 0        | 1        | 1        |

*Note: 0 refers to control group; 1 refers to baseline reminders only; 2 refers to once-weekly reminders only; 3 refers to twice-weekly reminders.*

An important issue to note is that because we are not able to randomly assign a selected group of people into a traditional control group, we opted for a stepped-wedge design. Under this design, instead of randomly assigning people to either receive treatment or not, we randomly assign courts to the various treatment group. Then we stagger the implementation of the reminders to the courts randomly. This means that some courts will start the experiment first while others wait and stay in the control condition. After a period of time, they too will also receive treatment. This ensures that we do not withhold anyone from treatment just because we needed a control group, thus bypassing that ethical concern. 

To further illustrate the design, all groups will start as control conditions at Period 1. During Period 2, only courts in Group A will receive the baseline reminder treatment. Baseline reminders consists of a single reminder sent prior to the court date, reflecting current best practices used by many courts. Then in Period 3, Group B will join Group A in receiving the baseline reminder treatment while the rest still remain in the control condition. Once we get to Period 4, both Group B and C will receive baseline reminders while Group A transitions to an additional once-weekly reminder on top of the baseline reminder. This pattern repeats until all groups receive some form of treatment, with most groups receiving increasingly intensive reminders (i.e., moving from baseline to once-weekly then to twice-weekly). 

### Power and Feasibility 
Because this study operates under real-world constraints, power calculations were used to balance statistical sensitivity with ethical and operational feasibility. Using anticipated court participation, the study is powered to detect modest but policy relevant reductions in failure to appear. 

We utilized a simulation-based power analysis to decide how many courts we would need to recruit in total to detect a modest effect. First, we used historical data to estimate the baseline rate of FTA. We then specified a minimum of 3 percentage point reduction in FTA. Because outcomes are clustered within courts over time, we incorporated within-court correlation via an intraclass correlation (ICC) values. The ICC captures how correlated outcomes are within the same court over time (i.e., how much clustering reduces the effective sample size). We run several plausible values of 0.01, 0.02 and 0.05 to see how power changes under different scenarios. 

In each simulation, courts are randomly assigned to Group A to E and we apply our period-by-period rollout (0, 1, 2, or 3 reminders). We generate the FTA rate using the FTA baseline, assumed effect, court differences, and time effects. Each simulated dataset is then analyzed using our planned generalized linear model with court fixed effects and period fixed effects. We repeat this process across a range of assumptions about the number of courts, study duration, and expected case volume. Power was defined as the proportion of simulated trials in which the treatment effect was detected at α = 0.05.


## Analysis of Results
The experiment will be analyzed with a generalized linear model with court and month fixed effects so that causal identification comes from within-court changes in reminder exposure over time while controlling for system-wide or time shocks. The primary outcome is failure to appear. The resulting estimated coefficients will reflect changes in FTA and detention rates that are attributable to changes in reminder dose, net of both court-specific and time-specific confounds. 

Results will directly inform court communication policies by identifying the minimum reminder intensity needed to reduce missed appearances without increasing administrative burden. 

## My Role
## My Role
I led the study design, ethical review framing, randomization strategy, and analysis plan, working closely with court stakeholders to ensure feasibility and compliance with operational constraints.

## Project Status
- Study design: ✅ complete  
- Court recruitment: 🟡 in progress
- Power calculation:  🟡 in progress
- Implementation: ⏳ upcoming  
- Analysis & results: 🔜 future update

