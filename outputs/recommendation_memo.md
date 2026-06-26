1.	Executive summary
The experiment successfully achieved its objective of improving the North Star Metric, 30-Day Revenue Growth, with highly significant statistical evidence for engagement score in Treatment group. The treatment accelerated conversion, increased monetization, and improved overall business outcomes. However, the observed device-level disparities and potential revenue quality concerns warrant a controlled rollout supported by rigorous guardrail monitoring. A phased deployment focused on Mobile and Tablet segments offers the highest probability of capturing revenue upside while minimizing operational and customer experience risks.

2.	North Star metric
•	30-day Revenue Growth. This represents the overall business outcome and is directly influenced by acquisition, activation, conversion, and customer experience.

3.	KPI tree explanation
•	User Acquisition & Reach. Drivers – Traffic Quality, Landing Page Performance
•	User Activation & Engagement. Drivers – Trial Adoption, Onboarding Success
•	Paid Conversion & Monetization. Drivers – Trial to paid conversion, Avg Rev per paid User


4.	Experiment result summary
 	Control	Treatment
Mean	57.02953216	62.94002849
Variance	191.219068	193.9050573
Observations	684	702
Hypothesized Mean Difference	0	 
df	1383	 
t Stat	-7.928175369	 
P(T<=t) one-tail	2.27375E-15	 
t Critical one-tail	1.645956155	 
P(T<=t) two-tail	4.54751E-15	 
t Critical two-tail	1.961680769	 


5.	Hypothesis test interpretation
o	Null Hypothese: Null Hypothesis (H₀): Hypothesized mean difference between control group  & treatment  group is Zero   Ho: μ_control = μ_Treatment
o	Alternative Hypothesis (H₁): Mean difference between two  groups is not Zero  Ha: μ_control ≠ μ_Treatment

•	Since p-value is very small ( p-value: 4.54751E-15 <<0.05), we can reject the null Hypotheses
•	There is sufficient statistical evidence Treatment group has higher mean engagement rate than Control group

6.	Guardrail analysis

Refund Rate	Refund Requests ÷ Paid Conversions	High revenue growth may be driven by poor-quality conversions, misleading marketing, or customer dissatisfaction.
Support Ticket Rate	Support Tickets ÷ Active Users	Rising tickets can indicate onboarding friction, product bugs, or poor user experience despite increasing revenue.
Days to Convert	Average Days from Signup to Paid Conversion	A longer conversion cycle may signal reduced urgency, weaker value proposition, or inefficient funnel performance.
Engagement Score	Average engagement score across users	Users may convert initially but fail to realize product value, increasing future churn risk.
Segment-Level Decline	Conversion, engagement, or retention trends by region, device, traffic source, etc.	Aggregate metrics can hide severe performance deterioration in specific customer segments.


7.	Segment-level insight



Avg days to convert
region	Control	Treatment	Grand Total
East	9.3	6.7	7.4
North	10.0	6.5	7.6
South	6.5	6.2	6.3
West	9.8	6.1	7.4
Grand Total	8.9	6.4	7.2

ARPU – notice the anomalies in Control vs Treatment in Desktop, while it gets compensated in Tablet
device_type	experiment_group	Sum of revenue_30d	Count of user_id	ARPU
Desktop	Control	16989	200	84.9
	Treatment	8765	214	41.0
Desktop Total		25754	414	62.2
Mobile	Control	17911	428	41.8
	Treatment	25649	436	58.8
Mobile Total		43560	864	50.4
Tablet	Control	409	56	7.3
	Treatment	4107	56	73.3
Tablet Total		4516	112	40.3
Grand Total		73830	1390	53.1

Revenue by support tickets raised – 0 tickets raised has no material impact between 2 groups. 
Treatment group handles support well with 1 tickets raised
support_tickets_30d	Control	Treatment	Grand Total
0	31903	29787	61690
1	2907	6028	8935
2	1053	1507	2559
3	0	1199	1199
4	0	0	0
Grand Total	35862	38521	74383



8.	Final recommendation:
o	Launch only for selected segment
1.	Mobile & Tablet
2.	Subscriptions -  Free & Premium plans
3.	Through Email, Paid search & Referrals

9.	Risks and limitations

•	Revenue concentration. 
•	Loss of strategic markets. 
•	Bias in acquisition strategy.
•	Revenue Quality. Shouldn’t be because of discounts and promotions, with poor LTV, Retention


Guardrail Metric	Risk Level	Why
Refund Rate	High	Direct indicator of poor customer satisfaction and revenue reversal
Support Ticket Rate	Medium-High	Indicates operational scalability and product quality issues
Days to Convert	Medium	Signals funnel inefficiency and rising acquisition costs
Engagement Score	High	Strong leading indicator of retention and churn
Revenue Quality	High	Prevents misleading revenue growth
Segment-Level Decline	High	Protects against hidden deterioration in important customer groups


10.	Next steps

Identify the sub-drivers and track their improvement by segment. 
Identify key risks and plans to mitigate them
Find business opportunities in growing areas with experiments of different channel and subscription strategy 

