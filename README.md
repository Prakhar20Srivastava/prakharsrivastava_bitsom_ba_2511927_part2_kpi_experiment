# prakharsrivastava_bitsom_ba_2511927_part2_kpi_experiment

###### A/B Testing Experiment Analysis

###### Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user activation, engagement, and paid conversions. An A/B test was conducted by dividing users into a **Control** group (existing onboarding) and a **Treatment** group (new onboarding experience). The objective was to determine whether the new onboarding campaign should be rolled out to all users while ensuring it does not negatively impact key business metrics.

\---

###### Dataset Description

The dataset contains user-level experiment data, including:

* Experiment group (Control or Treatment)
* Landing page visits
* Trial starts
* Onboarding completion
* Paid conversion
* Revenue
* Refund requests
* Support tickets
* Engagement score
* Days to convert
* User segments (Region, Device Type, Traffic Source, Plan Type)

Before analysis, the dataset was validated by checking for missing values, duplicate user IDs, invalid binary values, revenue outliers, and balanced segment distribution across experiment groups.

\---

###### North Star Metric Selected

**User Activation Rate (Onboarding Completion Rate)**

This metric was selected because it directly measures whether users successfully complete the onboarding process and experience the product's core value. Higher activation is expected to increase engagement, paid conversions, retention, and long-term customer value.

\---

###### KPI Tree Summary

The KPI tree was built around the North Star Metric.

**North Star Metric**

* User Activation Rate

**Primary Drivers**

* Onboarding Completion
* Feature Adoption
* Early User Engagement

**Sub-Drivers**

* Profile Setup Completion
* Tutorial Completion
* Core Feature Usage
* First Value Achieved
* Session Frequency
* Feature or Content Interactions

**Guardrail Metrics**

* Refund Rate
* Support Ticket Rate
* Revenue Quality

\---

###### Experiment Analysis Approach

The experiment compared the Control and Treatment groups using key business metrics, including:

* User Count
* Landing Page Visit Rate
* Trial Start Rate
* Onboarding Completion Rate
* Paid Conversion Rate
* Average Revenue per User
* Average Revenue per Converted User
* Refund Rate
* Support Ticket Rate
* Average Engagement Score
* Average Days to Convert

Segment-level analysis was also performed by Region, Device Type, and Traffic Source to ensure consistent treatment performance across different user groups.

\---

###### Hypothesis Test Summary

A one-tailed Two-Proportion Z-Test was conducted on the **Onboarding Completion Rate**.

* **Null Hypothesis (H₀):** The treatment does not improve the onboarding completion rate.
* **Alternative Hypothesis (H₁):** The treatment improves the onboarding completion rate.
* **Significance Level:** 0.05
* **P-value:** < 0.05

The null hypothesis was rejected, indicating that the treatment significantly improved user activation compared to the control group.

\---

###### Guardrail Metrics Considered

To ensure the recommendation was not based solely on conversion improvements, the following guardrail metrics were evaluated:

|Metric|Observation|
|-|-|
|Refund Rate|Slight increase in the treatment group.|
|Support Ticket Rate|Increased noticeably, suggesting additional onboarding support may be required.|
|Average Revenue per Converted User|Lower than the control group, indicating reduced revenue quality.|
|Average Days to Convert|Improved, with users converting faster.|
|Engagement Score|Increased, indicating stronger early product engagement.|

These guardrail metrics highlight both the benefits and potential risks of the new onboarding experience.

\---

##### Final Recommendation

**Recommendation: Launch with a Phased Rollout (Continue Testing During Rollout)**

The treatment significantly improved the North Star Metric (User Activation Rate) as well as paid conversion, engagement, and conversion speed. However, higher support ticket rates and lower average revenue per converted user suggest that the rollout should be gradual while these guardrail metrics are closely monitored.

\---

###### Assumptions and Limitations

###### Assumptions

* Users were randomly assigned to the Control and Treatment groups.
* Data accurately represents user behavior during the experiment.
* Binary variables were correctly recorded.
* External factors did not significantly influence experiment results.

###### Limitations

* The experiment reflects a single testing period and user sample.
* Long-term retention and customer lifetime value were not evaluated.
* Increased support tickets may affect operational costs after rollout.
* Additional testing may be needed for specific customer segments.

\---

###### Screenshots Included

The project includes screenshots of:

* KPI Tree
* Experiment Summary Tables
* Segment Analysis
* Hypothesis Test Results
* Guardrail Metric Analysis
* Recommendation Summary
* Excel calculations and supporting visualizations

These screenshots provide evidence supporting the analysis and final recommendation.
