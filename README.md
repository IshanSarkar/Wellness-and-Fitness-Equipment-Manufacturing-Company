# Wellness and Fitness Equipment Manufacturing Company - Product Analysis
Language; Python <br>
Libraries: NumPy, Pandas, Matplotlib, Seaborn)

## Business Problem:
The market research team in the company wants to identify the characteristics of the target audience for each type of treadmill offered by the company, to provide a better recommendation of the treadmills to the new customers. The team decides to investigate whether there are differences across the product for customer characteristics.

## Data Characteristics
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/82f66597-924f-4f53-a89a-d0923c910676)<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/dcb2c3cd-ecc2-4cee-a983-ef78fdcfaaad)<br>

## Detection of Outliners
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/5238bea8-5c72-4916-82c6-a672f1af6080)<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/0cc4ddd3-227c-45fa-b304-feaad9fe5d35)<br>
We observe variances between the mean and median (50th percentile) across all the columns above which can be shown in the table as well as the graph.<br>
Positive skewness is evident in Age (in years), Usage (every week), Fitness (self-rated fitness on a 1-to-5 scale), Income, and Miles (distance covered by walking/running), while negative skewness is apparent in Education (total number of years).<br>

- Age: A younger population demographic is more inclined to purchase most of the products, with some exceptions.
- Usage: The majority of users exhibit low to moderate engagement in a week, with a few highly engaged outliers.
- Income: There is a larger segment with lower income, potentially suggesting affordability as a key factor in purchasing decisions with multiple outliers above 80000.
- Miles: Most users walk/run shorter distances, although a few outliers are covering significantly longer distances.

Understanding these trends could inform targeted marketing strategies or product development tailored to different age groups or income brackets.<br>
Negative skewness is observed in Education, signifying a concentration of individuals with fewer years of schooling and a smaller proportion with higher educational attainment. This suggests a potential focus on individuals with lower educational backgrounds when targeting the audience. But when checked for each product in a box plot then we do not see any outliner <br>

***Manually adjusting the Percentile range based on outliners of each column to get the least biased data frame as much as possible by using Clipping/clip()*** <be>

![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/d01d1950-018f-4b90-9528-765039e15f20)<br>

#### Business Insights: <br>
 - The average age of customers is approximately 28 years old, with the majority having an education level of around 15 years. This suggests that the target audience might be young adults who have completed some form of higher education. The youngest customer is 18, and the oldest is approximately 45.63 years old. Understanding this age distribution can help businesses target specific age groups for marketing campaigns or product development.<br>
 - Customers' education level varies, with a minimum of 12 years and a maximum of 18.84 years. This suggests a diverse customer base with varying preferences and needs. Businesses can conduct further market research to understand how education level correlates with product preferences and tailor their offerings accordingly.<br>
 - The average product usage is around 3.4 days per week, and customers have an average fitness level of 3.32. This indicates that customers are moderately engaged with the product and are moderately fit. These insights underscore the importance of promoting features that encourage consistent product usage while aligning with the fitness goals and preferences of the customer base.<br>
 - The average income is approximately 51,987 dollars with a standard deviation of 12,571 dollars. This indicates that the target market has a moderate to moderate-high income level. Businesses can use this information to price their products accordingly and offer appropriate discounts or financing options.<br>
 - On average, customers cover around 99.58 miles. This information is valuable, as it allows us to understand the average distance customers travel by walking/running and tailor our services or products to accommodate this.

## Correlation:
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/b0248799-2880-4499-b942-09c66b1ea9a6)<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/391c651b-d06a-4143-be80-3d5767b513fc)<br>
#### Conclusion and Insights:<br>
 - Income and Education: There is a strong positive correlation (0.65) between income and education. This suggests that individuals with higher levels of education tend to have higher incomes.<br>
 - Fitness and Usage: There is a strong positive correlation (0.66) between fitness and usage. This implies that individuals who use fitness-related products or services tend to be more fitness-conscious. <br>
 - Fitness and Miles: There is a very strong positive correlation (0.83) between fitness and miles. This indicates that individuals who are more fitness-conscious tend to cover more miles, likely indicating higher levels of physical activity. <br>
 - Usage and Miles: There is a strong positive correlation (0.78) between usage and miles. This suggests that individuals who use a particular product or service tend to cover more miles, potentially indicating frequent usage or engagement with the product/service. <br>
 - Income and Age: There is a moderate positive correlation (0.55) between income and age. This implies that older individuals tend to have higher incomes, which could be due to factors such as career advancement or accumulation of wealth over time.

## Column-wise Analysis
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/aeab2d65-4041-401d-a095-96d4081f1eda)<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/4124f99e-1851-4b9f-8b7d-64ba39ededd1)<br>
#### Analysis
 - Product Preferences: The KP281 treadmill seems to be the most popular choice among customers, with 80 units sold, followed by KP481 (60 units) and KP781 (40 units). This indicates a potential demand for features or price points offered by the KP281 model.
 - Age: Customers aged 25 and 23 represent the largest segments, followed by ages 24, 26, and 28. This suggests that the target demographic for these treadmills is primarily younger adults.
 - Gender: Males account for a larger portion of sales (104 units) compared to females (76 units). The company may want to explore marketing strategies to attract more female customers.
 - Education: Majority of customers have completed 16 years of education, followed by 14 and 18 years. This could indicate that customers with higher education levels are more likely to purchase these treadmills.
 - Marital Status: Partnered individuals (107 units) seem to purchase more treadmills compared to single individuals (73 units). This could imply that partnered individuals are more inclined towards fitness or have higher disposable income for such purchases.
 - Usage: Most customers use the treadmills for 3 or 4 times a week, with fewer users engaging in more frequent usage. This information can guide the company in designing features tailored to these usage patterns.
 - Fitness Level: Customers with a fitness level of 3 represent the largest segment, followed by level 5. This indicates that the treadmills are attracting customers with moderate to high fitness levels, suggesting the treadmills cater well to fitness enthusiasts.
#### Recommendation
 - Develop marketing campaigns targeting females and single individuals to potentially increase sales in these demographics.
 - Consider incorporating features or pricing strategies that appeal to a broader age range to capture older customers.
 - Offer programs or incentives to encourage more frequent usage, potentially increasing customer satisfaction and loyalty.
 - Educate potential customers about the benefits of using treadmills for fitness, especially targeting demographics with lower fitness levels.
## Product-Wise Deep Analysis
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/2d216f27-33ca-491c-9ddd-1d38958ac0dc)<br>
Young Explorers: Ages 18-25 <br>
Active Achievers: Ages 26-35 <br>
Prime Trailblazers: Ages 36-45 <br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/d6731179-e903-49a4-a23a-95bff349722b)<br>
We can conclude that 44.44% of total cosumers will buy KP281 and out of which 40% will be Active Achievers, 17.5% will be Prime Trailblazers and 42.5% are Youthful Explorers<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/84646f47-1486-4c90-ac66-5da8d40ea590)<br>
#### Analysis and Insights: 
**Overall Distribution:**
- The total number of customers across all age groups for all products is 180.
- The percentage distribution of customers across age groups shows that Youthful Explorers form the largest segment, followed by Active Achievers and then Prime Trailblazers.

**Product-wise Distribution:**
- KP281: This product has the highest number of customers across all age groups compared to the other two products, indicating it might have broader appeal or better marketing reach compared to the other products.
- KP481: While having fewer customers overall, it still maintains a considerable presence across different age groups, suggesting it has its own niche or specific target audience. Further analysis is needed to understand why it attracts fewer customers across other age groups.
- KP781: This product has the fewest customers, with the majority being Youthful Explorers and some exception which are at the Prime Trailbrazers group

#### Recommendations:
- Targeted Marketing: Tailor marketing strategies to each age group's preferences. Highlight different product features and benefits that resonate with each segment. Invest more in reaching out to the Active Achievers segment, as they represent a potentially untapped market for growth.
- Product Development: Consider adjusting product features or branding to appeal to specific age groups where the product is underperforming. Conduct market research to understand why KP781 is less popular among certain age groups and make necessary improvements or adjustments.
- Diversification: Explore opportunities to diversify product offerings to cater to a wider range of age groups and preferences. Introduce product bundles or packages that appeal to multiple age groups simultaneously.
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/fadad43b-3fc6-42c9-92cf-12b983761c64)<br>
#### Analysis:<br>
**Product Distribution Across Education Levels:**<br>
- KP281: Shows a steady increase from education levels 12 to 16, then slightly dips at 18.<br>
- KP481: Similar to KP281 but with a slightly smaller distribution.<br>
- KP781: Low distribution until education level 16, where it sees a significant rise.<br>
**Total Distribution Across Education Levels:** Overall, there's an increasing trend in product distribution with the progression of education levels. Education level 16 has the highest overall distribution followed by 14 and 18.<br>
**Normalized Distribution:** The normalized distribution provides a clearer picture of the proportional representation of each product across education levels. KP281 and KP481 dominate the distribution, especially at education level 16. KP781 has a relatively lower but still noticeable presence, particularly at education level 18.<br>

#### Insights:<br>
- There's a notable shift in product preferences as education level progresses, with KP281 and KP481 being preferred at higher education levels. Also both the product seems to have successfully penetrated the market across various education levels and there is a dominance of both at education level 16 indicates a higher demand for these products among students at that stage.<br>
- KP781 gains traction in the later education years, suggesting it might cater to more advanced educational needs and shows potential for growth, particularly in higher education levels where it gains prominence and suggests a specific need or niche market within higher education institutions.

#### Recommendations:<br>
- Allocate more marketing resources towards KP281 and KP481 to maintain their stronghold, especially at education level 16. Invest in targeted marketing campaigns for KP781 to capitalize on its rising popularity at education level 18. <br>
- Conduct market research to identify specific features or functionalities that appeal to users at different education levels. Consider diversifying product offerings to cater to a broader range of educational needs and preferences.<br>
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/b3bb7317-8738-4c34-9f16-408503f25236)<br>
#### Analysis of Product Usage Distribution:<br>
- The table shows the usage of three different products (KP281, KP481, KP781) across different usage frequencies (2, 3, 4, 5 days/week).<br>
- The totals across all usage frequencies are also provided for each product.<br>

#### Insights:
- KP281: This product has the highest overall usage, with 80 instances reported across all frequencies. It is most commonly used for 3 days a week (37 instances), followed by 2 days a week (19 instances).<br>
- KP481: The second most used product with a total of 60 instances. Similar to KP281, it is also most commonly used for 3 days a week (31 instances).<br>
Both products exhibit similar usage distributions, with the highest proportions for 3 days a week, followed by 2 days a week. This suggests a consistent pattern of usage for these products.<br>
- KP781: This product has the lowest overall usage, with only 40 instances reported across all frequencies. Notably, it is primarily used for 4 and 5 days a week, with a total of 39 instances. Unlike KP281 and KP481, KP781 shows a more varied usage distribution, with significant proportions for both 4 and 5 days a week, indicating a different usage pattern compared to the other products.<br>

#### Recommendations:<br>
- **KP281 & KP481:** Focus marketing efforts, production optimization, and inventory management on KP281 and KP481, the most frequently used products. Investigate the reasons behind their popularity (effectiveness, affordability, unique features) to understand how to capitalize on their success. Conduct customer surveys or market research to identify areas for improvement and unmet needs.<br>
- **KP781:** KP781 has consistent usage across 4 and 5 days a week, indicating a niche market. Explore ways to expand the market by highlighting unique benefits or targeting specific customer segments. Consider adjusting marketing strategies or product positioning to better communicate the value proposition. Monitor customer feedback to ensure KP781 meets target audience needs.

![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/2f6369ff-1970-426a-980a-029001f7ba07)<br>
#### Analysis:
- KP281: This product has a relatively balanced distribution across income groups, with a significant portion of sales in the Medium-High income group.<br>
- KP481: It shows a similar pattern to KP281, with a substantial share of sales in the Medium-High income group but with fewer sales overall compared to KP281.<br>
- KP781: This product is mainly favored by the High-income group, with minimal to no sales recorded in the Low-Medium income group.<br>
**Overall Sales Distribution:** The majority of sales come from the Medium-High income group, followed by Low-Medium and High-income groups, in descending order.<br>

#### Insights:
- **Income Group Preferences:** Products KP281 and KP481 seem to cater well to a wider income range, with a notable presence in both Medium-High and High-income groups. KP781 appears to be a premium product, targeting specifically the High-income group. There's room for expansion in the Medium-High income segment.<br>
- **Market Potential:** The data suggests untapped potential in the Low-Medium income group, especially for products like KP281 and KP481. There might be opportunities for targeted marketing or pricing strategies to attract this segment.<br>
- **Product Portfolio Optimization:** Given the dominance of Medium-High income sales, there's a possibility to introduce new products or variants catering to this segment's preferences to further capitalize on this market share.<br>

#### Recommendations:
- **Diversification of Marketing Strategies:** Develop targeted marketing campaigns to appeal to the Low-Medium income segment, highlighting affordability, value for money, or unique selling propositions of products KP281 and KP481.<br>
- **Product Development:** Consider expanding the product range within the Medium-High income segment, focusing on features or benefits that resonate with this demographic's preferences.<br>
- **Price Optimization:** Evaluate pricing strategies to ensure competitiveness across income groups without compromising profitability. Consider discounts, promotions, or bundled offers to attract price-sensitive customers.
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/e39a779d-3b90-4fc3-a586-5ff7c4e753ee)<br>
#### Insights:
- **KP281 Performance:** KP281 has a minimal presence across all mileage ranges. This suggests that it might not be as popular or as well-performing as the other two products in these categories.<br>
- **KP781 Performance:** KP781 shows exceptional performance in the medium range miles group. It might be beneficial to focus marketing efforts on promoting KP781 for medium-range applications.<br>
- **KP481 Performance:** KP481 leads slightly in the short range while being present moderately in other ranges. It could be worth analyzing why KP481 is not performing as well as the others and consider improvements or repositioning in the market.<br><br>
**Overall Distribution:** Long Range products constitute the highest percentage of the total product count (23.33%), followed by Medium Range products (60%) and Short Range products (16.67%). This indicates a significant focus on Medium Range products, followed by Long Range, with less emphasis on Short Range offerings.<br>
**Consistent High Performance:** The box plot indicates that KP781 has a higher median value, suggesting consistent high performance. This could be a selling point when marketing KP781.<br>

#### Recommendations:
**Product Development:** Considering the significant portion of products falling into the Medium Range category, there may be an opportunity for product development or enhancement in this segment to cater to the existing demand. Assessing the market demand for Long Range products and potentially investing more resources in this category, especially if there's a growing trend towards longer distance travel.<br>
**Marketing and Sales Strategy:** Tailoring marketing and sales strategies to highlight the strengths of each product in its respective mileage category. For example, emphasizing the endurance and efficiency of Long Range products. Conducting market research to understand customer preferences and trends in different mileage categories, enabling more targeted marketing efforts.
![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/8d1ee635-bee2-4a0c-a141-72c6f5987e33)<br>
#### Analysis:
- **KP281:**  Most respondents rated their fitness level as 3, followed by 2 and 4. Very few rated themselves as 5. KP281 has the highest count at level 2; product counts decrease as fitness levels increase. This suggests that it might not be as popular or as well-performing as the other two products in these categories. It could be beneficial to investigate why KP281’s performance is lagging behind the other products.<br>
- **KP481:** Similar to KP281, most respondents rated their fitness level as 3, followed by 2 and 4. There were no respondents who rated themselves as 5. KP481 shows moderate counts across all fitness levels but peaks at level 3. It could be worth analyzing why KP481 is not performing as well as KP781 and consider improvements or repositioning in the market.<br>
- **KP781:** Here, the majority of respondents rated their fitness level as 5, followed by 3. There were very few ratings of 4 and none for 2. KP781 shows exceptional performance at a fitness level of 3 across all three graphs. It might be beneficial to focus marketing efforts on promoting KP781 for applications requiring higher fitness levels.<br>
**Overall Fitness Distribution:** Across all products, most respondents rated themselves as 3, followed by 2 and 5. There were fewer respondents who rated themselves as 4.<br>
#### Insights:
- **Product Performance Perception:** The ratings suggest that different products might have different impacts or perceived benefits on fitness levels. For instance, KP781 seems to be associated with higher self-reported fitness levels compared to the other products.<br>
- **Gap in High Fitness Perception:** There's a noticeable gap in the perception of high fitness levels (rating 5) across products. While KP781 has a significant portion of respondents rating themselves as 5, KP281 and KP481 have very few or none at all. This could indicate differing effectiveness or marketing strategies between the products.<br>
- **Consistency in Mid-level Ratings:** Across all products, the most common fitness rating is 3. This suggests a consistent perception of average fitness levels among respondents regardless of the product used.<br>

#### Recommendations:
- **Product Improvement:** Analyze what aspects of KP781 contribute to higher fitness perception and consider incorporating similar features or strategies into other products to enhance their perceived effectiveness.<br>
- **Marketing Adjustments:** Tailor marketing strategies to highlight specific fitness benefits associated with each product. For instance, emphasize endurance and strength gains for KP781, while focusing on overall health improvements for KP281 and KP481.<br>
- **Diversification:** Consider diversifying product offerings to cater to different fitness goals and preferences. This could involve introducing new formulations or variations tailored to specific demographics or fitness objectives.<br>

![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/2bcf063d-4721-4006-b080-d695a1bd86e6)<br>
#### Insights:
**Gender Distribution:** The data shows that there were 76 female purchases and 104 male purchases, totaling 180 purchases overall. Males account for 57.78% of total purchases, while females account for 42.22%. This indicates that the product appeals slightly more to male customers.<br>

**Product Performance:** <br>
- **KP281:** This product has the highest sales, with 80 units sold. The gender distribution is equal, indicating its popularity among both genders.
- **KP481:** With 60 units sold, it's the second most popular product. The gender distribution is also fairly balanced.
- **KP781:** This product has the lowest sales volume, with only 40 units sold. However, it's notable that it has a higher proportion of male customers compared to females.
#### Recommendations:
- **Targeted Marketing:** Since there's a gender discrepancy in the popularity of certain products (like KP781), consider tailoring marketing strategies to appeal more to the gender that's less represented in the sales for each product.
- **Product Improvement:** Analyze why certain products are less popular among one gender. If there are specific features or aspects that appeal more to one gender, consider making adjustments to the product design or marketing to broaden its appeal.
- **Diversification:** While KP281 and KP481 seem to be performing well, consider expanding the product line to attract a more diverse customer base. Introducing new products with different features or price points could help capture additional market segments.

![image](https://github.com/IshanSarkar/Wellness-and-Fitness-Equipment-Manufacturing-Company/assets/160044904/a4ef11f4-7bcc-47c1-bf88-67ccb100fd1b)<br>
#### Insights:
**Market Segmentation:** <br>
- Partnered individuals account for approximately 59% of the total customer base, while single individuals constitute about 41%. This indicates that partnered individuals are a larger segment of the market.
- Among partnered individuals, KP281 is the most popular product, followed by KP481 and KP781.
- Among single individuals, the same trend holds with KP281 being the most popular product followed by KP481 and KP781.<br>

#### Recommendations:
- **Targeted Marketing:** While KP281 seems to have a universal appeal, there might be opportunities to tailor marketing efforts towards specific marital statuses. For instance, promotions highlighting the benefits of certain products in the context of partnerships or single life could be explored.
- **Product Development:** Given the consistent sales of KP281, it might be beneficial to invest in further developing this product line or introducing variations to capitalize on its popularity.
- **Diversification:** While KP281 is performing well, there could be a risk of overreliance on a single product. Exploring new product lines or diversifying offerings could mitigate this risk and tap into different market segments.

## Overall Report
#### Summarized Insights:
 - **Age:**
	- KP281: Broad appeal across all age groups.
    - KP481: Maintains presence across different age groups with a specific niche.
    - KP781: Fewest customers, mostly Youthful Explorers and some Prime Trailblazers.

 - **Education:**
	- KP281 and KP481 are preferred across all education levels, with KP281 being the most popular.
	- KP781 is less popular across all education levels, especially for higher education levels.

 - **Usage:**
	- KP281 and KP481 commonly used 3 days a week, while KP781 primarily used 4 and 5 days a week.

 - **Income:**
	- KP281 and KP481 cater to a wider income range, while KP781 targets the high-income group.
    - Untapped potential in the Low-Medium income group for KP281 and KP481.

 - **Miles:**
	- KP281 lacks presence across all mileage ranges.
    - KP781 performs exceptionally well in medium-range miles.
    - KP481 leads in short range but needs analysis for improvement.

 - **Fitness:**
	- KP281 and KP481 are preferred across all consumers with all fitness levels.
	- KP781 associated with consumers with higher self-rated fitness levels

 - **Gender:**
	- Slight male majority in purchases.
    - KP281 equally popular among genders.
    - KP781 has a higher proportion of male customers.

 - **Marital Status:**
	- Partnered individuals are the larger customer segment.
    - KP281 is the top-selling product across both marital statuses.
    - Consistent sales patterns for KP481 and KP781 across both segments.

#### Overall Insights:
- KP281 appears to have broad appeal across different demographics and usage patterns.
- KP481 serves a specific niche and maintains moderate presence across segments.
- KP781 targets higher-income, more advanced education, and fitness-oriented customers but with lower overall sales.
- There's potential for growth in untapped segments such as Low-Medium income and specific education levels.
- Gender and marital status don't seem to heavily influence treadmill preference. As market segmentation of Partnered being %59.45 and Single being %40.55 as well as Male being %57.77 and Female being %42.22.
- Marketing strategies could be tailored to enhance performance in areas where products are underperforming, such as increasing KP281's presence across mileage ranges or repositioning KP481 in the market.

#### Overall Product-wise Recommendation:
- **KP281:**
	- Age: Continue targeting all age groups but consider diversifying marketing to appeal to specific age segments.
	- Education: Allocate marketing resources to maintain stronghold, especially at education level 16.
	- Usage: Focus on optimizing production and inventory management for frequent users.
	- Income: Develop targeted campaigns for the Low-Medium income segment, highlighting affordability.
	- Miles: Assess market demand for product enhancement and diversify offerings accordingly.
	- Fitness: Tailor marketing to highlight overall health benefits.
	- Gender: Expand product line to attract a more diverse customer base.
	- Marital Status: Explore opportunities to tailor marketing efforts towards specific marital statuses.
- **KP481:**
	- Age: Tailor marketing strategies to resonate with different age groups' preferences.
	- Education: Invest in targeted campaigns to maintain stronghold, especially at education level 16.
	- Usage: Focus on production optimization for frequent users and conduct customer surveys for improvements.
	- Income: Develop campaigns targeting the Low-Medium income segment.
	- Miles: Tailor marketing and assess market demand for product enhancement.
	- Fitness: Focus on highlighting endurance and strength gains.
	- Gender: Expand product line to appeal to both genders.
	- Marital Status: Explore opportunities for targeted promotions based on marital status.
- **KP781:**
	- Age: Investigate reasons for lower popularity among certain age groups and make necessary improvements.
	- Education: Invest in targeted campaigns to capitalize on rising popularity at education level 18.
	- Usage: Explore ways to expand the market by highlighting unique benefits.
	- Income: Consider adjusting marketing strategies or product positioning to better communicate the value proposition.
	- Miles: Assess market demand for product enhancement.
	- Fitness: Analyze aspects contributing to higher fitness perception and incorporate similar features into other products.
	- Gender: Tailor marketing strategies to appeal more to the less represented gender.
	- Marital Status: Explore opportunities for targeted promotions based on marital status.

#### Business Decisions:
- **Product Focus:** Invest in enhancing features of the popular KP281 treadmill and maintaining competitiveness of KP481.
- **Targeted Marketing:** Tailor marketing campaigns to highlight the versatility of KP281 and niche appeal of KP781.
- **Market Expansion:** Explore new demographics and international markets based on identified preferences.
- **Pricing Strategy:** Price KP281 as a premium option and KP781 competitively to attract cost-conscious consumers.
- **Feedback Integration:** Continuously gather customer feedback to improve product offerings and customer satisfaction.
- **Distribution Optimization:** Optimize distribution channels to ensure availability and accessibility of products to target customers.
