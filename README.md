# Marketing-Campaign-and-Customer-Behaviour-Analysis-with-Python
Understanding customer behaviour is essential for businesses that want to improve marketing performance, increase customer engagement, and allocate campaign resources effectively.
This project presents an Exploratory Data Analysis (EDA) of 2,240 customers across 28 variables. The analysis focuses on customer demographics, income, purchasing behaviour, customer engagement, marketing campaign performance, and the characteristics associated with customers responding to marketing campaigns.

## Business Objective
The primary objective of this analysis is to understand customer behaviour and marketing campaign response and identify customer characteristics that can support more effective marketing targeting. The analysis addresses the following business questions:
- What does the overall customer profile look like?
- What are the dominant customer demographic groups?
- How do customers interact with different purchasing channels?
- Which customer characteristics are associated with campaign response?
- Are high-value customers more likely to respond?
- Does recent purchasing activity influence campaign engagement?
- How does campaign performance differ across customer groups?
- Which customer characteristics could support future customer segmentation?
- How can the business improve future marketing campaigns?

### Dataset
The dataset contains 2,240 customer records and 28 variables, covering:
- Customer ID
- Year of Birth
- Education
- Marital Status
- Income
- Household composition
- Customer tenure
- Recency
- Product spending
- Web purchases
- Catalogue purchases
- Store purchases
- Website visits
- Previous campaign acceptance
- Latest campaign response
- Customer complaints
- Country
A data dictionary was also provided to understand the meaning and business context of each variable.
### Tools and Technologies
- Python
- Pandas for data manipulation and analysis
- NumPy for numerical analysis
- Matplotlib for data visualisation
- Seaborn for statistical visualisation
### Key Findings
#### 1. Customer Demographic Profile
The customer base is predominantly made up of Graduation-level customers, with 1,127 customers, followed by PhD and master's-level customers. Married customers form the largest marital-status group, followed by Together and Single customers. Geographically, Spain is the largest customer market, accounting for 1,095 of the 2,240 customers.
This indicates that the business has a diverse customer base but is heavily concentrated in the Spanish market.
#### 2. Customer Income
Average customer income was approximately 52,238, while the median income was 51,381.50.The dataset also contained an unusually high income value of 666,666, which was identified as a potential outlier.Missing income values represented approximately 1.07% of the dataset and were handled using median imputation.
#### 3. Customer Spending
A new Total_Spending variable was created by combining spending across the major product categories. The results showed:
 ##### Metric	          Value
    Average Spending	    605.80
    Median Spending	      396.00
    Minimum              	5
    Maximum	              2,525
The spending distribution was strongly right-skewed. This indicates that while a large proportion of customers are low-to-moderate spenders, a smaller group represents high-value customers with significantly higher spending.
#### 4. Purchasing Channel Behaviour
Store purchases were the dominant purchasing channel.
##### Channel	        Average Purchases
      Store	          5.79
      Web	            4.08
      Catalogue	      2.66
Customers therefore interact with the business through multiple channels, but physical-store purchasing remains the strongest channel, followed by web purchasing. This provides an opportunity for an integrated omnichannel marketing strategy.
#### 5. Latest Campaign Performance
The latest marketing campaign recorded:
- 1,906 customers who did not respond
- 334 customers who responded
- 14.91% overall response rate
Although the majority of customers did not respond, the latest campaign performed considerably better than the previous campaigns.
Previous campaign acceptance rates were approximately:
##### Campaign	      Acceptance Rate
      Campaign 1	    6.43%
      Campaign 2	    1.34%
      Campaign 3	    7.28%
      Campaign 4	    7.46%
      Campaign 5	     7.28%
The latest campaign's 14.91% response rate was approximately twice the acceptance rate of the strongest previous campaign. This suggests that the latest campaign strategy may have been more effective.
#### 6. Higher-Income Customers Were More Responsive
Customers who responded to the latest campaign had a higher average income than non-responders.
- Non-responders: approximately 50,800
- Responders: approximately 60,000
This suggests that income is associated with campaign responsiveness and may be useful when developing customer segments.
#### 7. High-Spending Customers Were Much More Responsive
One of the strongest patterns identified was the difference in total spending.
-  Non-responders: approximately 540 average total spending
-  Responders: approximately 990 average total spending
Responders therefore represented a substantially higher-value customer group.This indicates that customer value is an important factor to consider when targeting future campaigns.
#### 8. Frequent Customers Were More Responsive
Responders also made more purchases across Web, Catalogue and Store channels.
-  Non-responders: approximately 12 purchases
-  Responders: approximately 15.3 purchases
This suggests that customers who purchase more frequently are more engaged with the business and more likely to respond to marketing campaigns.
 #### 9. Recent Customers Were More Responsive
Recency showed another meaningful difference.
- Non-responders: approximately 51 days since last purchase
- Responders: approximately 35 days since last purchase
Customers who had purchased more recently were more likely to respond to the campaign. This makes recency an important customer-engagement indicator for future targeting.
#### 10. Education and Campaign Response
Campaign response varied considerably across education groups.
##### Education	          Approx. Response Rate
        Basic	                    3.6%
        2n Cycle	                10.8%
        Graduation	              13.5%
        Master	                  15.3%
        PhD	                      20.7%
The analysis showed a general increase in campaign response as education level increased. However, education should be considered alongside behavioural variables rather than used as the sole basis for targeting.
####  11. Geographic Differences in Campaign Response
Campaign response varied across countries. Spain recorded a relatively strong response rate among the major customer markets. Mexico recorded an extremely high response rate of approximately 66.7%, but this was based on only three customers. Therefore, the Mexico result should not be interpreted as evidence of a high-performing market.
This demonstrates an important analytical principle:
#### Response rate must always be considered alongside sample size.

#### 12. Marital Status and Campaign Response
Single and Divorced customers recorded higher response rates than Married and Together customers among the larger customer groups. Some smaller categories recorded extremely high response rates, but their customer populations were too small to support reliable conclusions. Therefore, marital status may provide useful segmentation information, but behavioural characteristics provide stronger practical targeting signals.
#### 13. Age Was Not a Strong Differentiator
Average age was approximately:
- Non-responders: 46 years
- Responders: 45 years
The difference was very small.
This suggests that average customer age alone does not strongly distinguish campaign responders from non-responders.
#### 14. Website Visits Showed Little Difference
Average monthly website visits were almost identical between campaign responders and non-responders. This suggests that website visit frequency alone is not a strong indicator of campaign response. Compared with spending, purchase frequency and recency, website visits provided much weaker evidence of campaign engagement. Very small categories such as Alone, YOLO and Absurd were identified and treated cautiously because their small sample sizes can produce misleading percentages.

### Customer Behaviour Insights
The analysis revealed a consistent behavioural pattern among customers who responded to the latest campaign.
Compared with non-responders, campaign responders generally had:
- Higher income
- Higher total spending
- More purchases
- More recent purchases
This is particularly important because these variables describe customer value and engagement, rather than simply customer demographics. The analysis therefore suggests that behaviour-based targeting may be more effective than relying primarily on demographic targeting.

## Business Implications
#### 1. High-Value Customers Should Receive Greater Attention
Customers with high spending and frequent purchases appear more receptive to marketing campaigns.
The business can therefore prioritise these customers for:
- Premium offers
- Cross-selling
- Upselling
- Loyalty programmes
- Exclusive promotions
#### 2. Recency Can Be Used to Identify Active Customers
Customers who purchased recently were more likely to respond.
Recency can therefore be used to distinguish:
- Recently active customers
- Moderately engaged customers
Customers requiring reactivation
#### 3. Marketing Should Become More Behaviour-Based
Instead of treating the entire customer base equally, marketing strategies can consider:
Recency + Spending + Purchase Frequency + Income + Demographics. This would allow the business to deliver more relevant offers to different customer groups.
#### 4. The Latest Campaign Should Be Investigated
The latest campaign achieved a substantially higher response rate than previous campaigns.
Management should investigate what was different about the campaign, including:
- Target audience
- Offer
- Communication
- Timing
- Marketing channel
- Customer selection
Successful elements can then be incorporated into future campaigns.
#### 5. Omnichannel Marketing Should Be Strengthened
Store purchases were the dominant purchasing channel, while web purchasing also represented significant customer activity. The business should therefore combine store-based engagement with digital marketing rather than relying exclusively on one channel.
## Conclusion
This analysis demonstrates that customer behaviour and customer value are important drivers of marketing campaign engagement.
-  The strongest patterns were observed among customers with higher spending, more frequent purchases, higher income and more recent purchasing activity. These characteristics were more informative for campaign response than average age or website visits.
-  The latest campaign also achieved a 14.91% response rate, significantly outperforming the five previous campaigns. This provides an opportunity for the business to investigate the strategy behind the campaign and replicate its successful elements. The analysis provides a data-driven foundation for customer segmentation, personalised marketing and campaign optimisation.
-  The key business opportunity is to move from broad marketing campaigns towards a behaviour-based and customer-value-driven strategy, where the right customers receive the right offer through the right channel at the right time.
