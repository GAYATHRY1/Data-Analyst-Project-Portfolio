**Viewer Retention in OTT Platforms**

Diagnosing Engagement Patterns
Winter Consulting Program – IIT Guwahati (Dec 2025 – Jan 2026)

**Project Overview**

This project was completed as part of the Winter Consulting Program at IIT Guwahati. The objective was to diagnose viewer retention challenges in OTT platforms, specifically focusing on early drop-off during Season 1 episodes. The analysis identifies the content and behavioral factors that influence whether viewers continue watching or disengage early.
The project combines data science, predictive modeling, and consulting-style strategic recommendations to help OTT platforms improve engagement and lifetime value.

**Business Problem**

OTT platforms experience significant early viewer drop-off in Season 1, which reduces lifetime value, affects renewal decisions, and weakens content ROI.
“Significant viewer disengagement during Season 1 reduces lifetime value and complicates renewal decisions.”
The goal of this project is to identify the drivers of early drop-off, segment episodes into meaningful clusters, and recommend actionable interventions.

**Analytical Objectives**

Diagnose episode-level factors influencing viewer continuation

Build predictive models to identify high-risk episodes

Segment episodes using clustering to uncover engagement archetypes

Recommend content and product interventions to improve retention
“Objective: identify drivers of drop-off, segment episodes into actionable groups, and recommend feasible content and product interventions.”

**Key Insights and Findings**

1. Drivers of Viewer Continuation
   
Predictive modeling identified pacing_score, hook_strength, and attention_required as the strongest predictors of continuation.
Episodes with strong hooks in the first 3–5 minutes and balanced pacing show higher continuation. Dense dialogue and high cognitive load correlate with elevated drop-off.
“Episodes with strong hooks in the first 3–5 minutes and balanced pacing show materially higher continuation.”
Model performance was exceptionally strong (ROC-AUC ~ 0.98–0.99).

2. Episode Segmentation (K-Means Clustering)
Using K-Means (k = 4), episodes were grouped into four actionable clusters:

Cluster 0 – Benchmark
Characteristics: High pacing, strong hooks
Engagement Outcome: Highest average watch percentage (70.65), low drop-off

Cluster 1 – Risk
Characteristics: Low pacing, high cognitive load, high attention required
Engagement Outcome: Highest drop-off (0.43), lowest average watch percentage (44.65)

Cluster 2 – Mixed
Characteristics: Moderate pacing and hooks, high dialogue density
Engagement Outcome: Mixed outcomes

Cluster 3 – Niche
Characteristics: High pacing, weaker hooks, high visual intensity
Engagement Outcome: Moderate watch percentage, low drop-off

This segmentation confirms that episodes fall into distinct archetypes with different engagement patterns.

**Conclusions**

Content design choices such as pacing, hook strength, and cognitive load are consistent predictors of early drop-off.
Clustering reveals clear episode archetypes with measurable engagement differences.
Targeted interventions on high-risk clusters, especially Cluster 1, can improve retention with minimal creative disruption.
“Targeted interventions on high-risk clusters (primarily Cluster 1) can improve retention with limited creative disruption and high ROI potential.”

**Methodology**

Exploratory Data Analysis (EDA)

Predictive Modeling (Decision Trees, Permutation Importance)

Clustering (K-Means)

Feature Engineering

Business Interpretation and Strategy Development

**Recommendations and Roadmap**

Priority 1 – High Impact, High Feasibility

Hook optimization pilot

Skip-Intro nudges

Fast A/B testing cycles

Priority 2 – High Impact, Medium Feasibility

Cognitive load reduction

Recommendation tuning

UX and editorial collaboration

Priority 3 – Medium Impact, Lower Feasibility

Creative playbooks

Production guidelines

Execution Plan:
“Run 2–3 concurrent pilots with clear success criteria and decision gates.”

**Risks and Mitigation**

Creative Disruption
Mitigation: Pilot changes on a small sample and run A/B tests

Nudge Annoyance
Mitigation: Personalize nudges and monitor opt-out rates

Resource Constraints
Mitigation: Prioritize high-ROI episodes and automate recaps or chapter markers

Monitoring Framework
Weekly KPIs include:

Average watch percentage

Drop-off at 5, 10, and 20 minutes

Retention cohort lift
Decision gate at 4–6 weeks.

**Final Outcome**
This project demonstrates strong capabilities in advanced analytics, predictive modeling, clustering and segmentation, and consulting-style strategic recommendations.
It provides a clear, data-driven roadmap for improving viewer retention and maximizing content ROI for OTT platforms.
