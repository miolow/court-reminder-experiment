# Court Reminder Experiment
**Designing and evaluating reminder interventions to reduce missed court appearances**

## Overview
People often miss court appearances not because they are unwilling or defiant, but because court systems are confusing, intimidating, and easy to forget. When a court date is missed, the consequences can include arrest warrants, detention, and cascading harms, especially on low-income individuals. This project documents the design and decision-making process behind a large-scale court reminder field experiment currently in recruitment and pre-implementation.

## Problem Statement
Failure to appear (FTA) in court is a common and costly problem for courts and communities. Traditional responses often treat missed appearance as willful noncompliance, rather than as a usability and communication failure issue. When attempting to estimate the causal impact of reminder interventions through large-scale field experiments, this framing introduces a critical ethical constraint, that is, maintaining a traditional control group would require withholding reimnders from a randomly selected group of individuals. This is unethical because it potentially exposes them to avoidable harm within the justice system. 

This project reframes it into a UX problem and examine how courts communicate expectations, timing, and logistics to people navigating an intimidating system. 

## Research Questions
1. Do reminder messages reduce failure to appear?
2. How does **frequency** of reminders affect outcomes?
3. How can we evaluate these interventions ethically in real court settings?

## Study Design
An important issue to note is that because we are not able to randomly assign a selected group of people into a traditional control group, we opted for a stepped-wedge design. Under this design, instead of randomly assigning people to either receive treatment or not, we randomly assign courts to the various treatment group. Then we stagger the implementation of the reminders to the courts randomly. This means that some courts will start the experiment first while others wait and stay in the control condition. After a period of time, they too will also receive treatment. This ensures that we do not withhold anyone from treatment just because we needed a control group, thus bypassing that ethical concern. 

### Study 1: Format of Reminders
In this study, we utilize the multi-arm stepped-wedge cluster randomizaed design. Courts will be randomized to different groups. All groups will start as control conditions at Period 1. During Period 2, only courts in Group A will receive treatment, specifically the baseline reminder treatment. Then in Period 3, Group B will join Group A in receiving the baseline reminder treatment while the rest still remain in the control condition. Once we get to Period 4, both Group B and C will receive baseline reminders while Group A transitions to once-weekly reminders. This pattern repeats until all groups receive some form of treatment, with most groups receiving increasingly intensive reminders (i.e., moving from baseline to once-weekly then to twice-weekly). 

| Group   | Period 1 | Period 2 | Period 3 | Period 4 | Period 5 | Period 6 | Period 7 |
|---------|----------|----------|----------|----------|----------|----------|----------|
| Group A | 0        | 1        | 1        | 2        | 2        | 3        | 3        |
| Group B | 0        | 0        | 1        | 1        | 2        | 2        | 3        |
| Group C | 0        | 0        | 0        | 1        | 1        | 2        | 2        |
| Group D | 0        | 0        | 0        | 0        | 1        | 1        | 2        |
| Group E | 0        | 0        | 0        | 0        | 0        | 1        | 1        |
*Note: 0 refers to control group; 1 refers to baseline reminders only; 2 refers to once-weekly reminders only; 3 refers to twice-weekly reminders.*

## Analysis of Results
The experiment will be analyzed with a generalized linear model with court and month fixed effects so that causal identification comes from within-court changes in reminder exposure over time while controlling for system-wide or time shocks. The resulting estimated coefficients will reflect changes in FTA and detention rates that are attributable to changes in reminder dose, net of both court-specific and time-specific confounds. 


## Project Status
- Study design: ✅ complete  
- Court recruitment: 🟡 in progress  
- Implementation: ⏳ upcoming  
- Analysis & results: 🔜 future update

