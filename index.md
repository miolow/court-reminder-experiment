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
3. How do **communication modes** (e.g., text, email, or both) compare?
4. Does providing **courthouse directions** improve attendance?
5. How can we evaluate these interventions ethically in real court settings?

## Study Design
There are a total of three proposed experimental designs for studies examining key factors shown to influence failure to appear rates: format of reminders (email or text), frequency (once a week or twice a week), and the provision of courthouse directions.

Another important issue to note is that because we are not able to randomly assign a selected group of people into a traditional control group, we opted for a cluster-type design. Under this design, instead of randomly assigning people to either receive treatment or not, we randomly assign courts to the various treatment group. In other words, randomization is now happening on the court level rather than individual level. We utilize the stepped-wedge experimental design and its variations for our purposes. The implications of this design is discussed further down below. 

### Study 1: Format of Reminders
In this study, we utilize the multi-arm stepped-wedge cluster randomizaed design. Courts will be randomized to different groups. Each group will have a reminder format (no reminder, text reminders, email reminders, or both text and email reminders), and a rollout timing that determines when they transition from control to an active reminder condition. All groups will begin in the control condition and transition into their assigned reminder frequency at staggered time points, after which they remain in that condition for the remainder of the study period. 

| Group   | Period 1 | Period 2 | Period 3 | Period 4 | Period 5 | Period 6 |
|---------|----------|----------|----------|----------|----------|----------|
| Group A | 0        | 1        | 1        | 1        | 1        | 1        |
| Group B | 0        | 2        | 2        | 2        | 2        | 2        |
| Group C | 0        | 3        | 3        | 3        | 3        | 3        |
| Group D | 0        | 0        | 1        | 1        | 1        | 1        |
| Group E | 0        | 0        | 2        | 2        | 2        | 2        |
| Group F | 0        | 0        | 3        | 3        | 3        | 3        |

*Note: 0 refers to control group; 1 refers to text reminders only; 2 refers to email reminders only; 3 refers to both email and text reminders.*

## Project Status
- Study design: ✅ complete  
- Court recruitment: 🟡 in progress  
- Implementation: ⏳ upcoming  
- Analysis & results: 🔜 future update

