Comprehensive Report on Halloween Candy Data Analysis
Summary Overview
The goal of this analysis is to determine the top three candies to distribute on Halloween, ensuring that trick-or-treaters will find a variety of treats they’ll love. This project utilizes Python-based techniques along with various statistical models, including hypothesis testing, clustering, and regression analysis. We analyzed 85 candy types based on their win percentage in online voting contests, combined with other factors such as chocolate, fruity, price, and sugar content. The insights gathered were used to narrow down the best candy options for Halloween distribution.
 
1. Data Exploration
We started by exploring the dataset, which contains 85 candy types with features such as:
•	Flavor profiles: Chocolate, fruity, caramel, nougat.
•	Win percentage: A continuous variable representing a candy’s popularity based on an online voting contest.
•	Price percentage: Indicating the relative affordability of each candy.
•	Sugar percentage: Offering insights into sweetness levels.
Key Insights:
•	Chocolate, Peanut/Almond, and Bar Candies: These categories showed strong positive correlations with price, suggesting that consumers are willing to pay more for these candies.
•	Fruity, Hard, and Pluribus Candies: These flavors displayed minimal impact from price, implying that factors like taste, texture, and brand recognition play a larger role in their popularity.
•	Combination Flavors: Candies that combine elements (e.g., chocolate with nuts or caramel) tended to show stronger correlations with both price and popularity.
 
2. Methodology
Data-Driven Approach Using Python:
We employed the following Python-based methods to identify key trends and candy preferences:
•	Hypothesis Testing: To determine if more popular candies were generally more expensive or had higher sugar content.
•	Linear Regression: Analyzed the relationship between candy attributes (e.g., price, flavor) and their popularity.
•	Clustering Analysis: Grouped candies into logical clusters based on characteristics like sweetness and texture, using K-Means clustering and Principal Component Analysis (PCA).
•	Feature Importance Analysis: Utilized RandomForestClassifier to identify which factors (e.g., chocolate, price, sugar content) most influenced candy popularity.
 
3. Detailed Candy Flavor Analysis
Chocolate:
•	Correlation with Price: Strong positive correlation (R-squared: 0.304).
•	Insight: Consumers are willing to pay more for high-quality chocolate treats, making chocolate a solid choice for Halloween.
Fruity:
•	Correlation with Price: Weak negative correlation (R-squared: 0.009).
•	Insight: Price does not significantly impact the popularity of fruity candies, suggesting taste and brand drive consumer choices.
Caramel:
•	Correlation with Price: Moderate positive correlation (R-squared: 0.156).
•	Insight: There is a preference for higher-priced caramel candies, but this trend is less strong than for chocolate.
Peanut/Almond:
•	Correlation with Price: Strong positive correlation (R-squared: 0.298).
•	Insight: Consumers associate higher prices with better-quality peanut/almond candies, making them premium options.
 Candy Rankings Based on Flavor Analysis:
Candy	Ranking	Rationale
Reese’s Peanut Butter Cups	1st	High in both chocolate and peanut butter flavors, making it the top performer.
Twix	2nd	Combines chocolate, caramel, and wafer, offering variety in texture and flavor.
Snickers	3rd	A combination of chocolate, peanuts, and caramel makes it a solid performer in multiple categories.
Peanut M&Ms	4th	A simple yet effective mix of chocolate and peanuts.
Sour Patch Kids	5th	Top non-chocolate option due to its sour and fruity appeal.

4. Analysis of Price-Performance (Win Percentage) Relationship
A joint plot of price percentage versus win percentage (popularity) revealed key insights:
•	Weak Positive Correlation: A weak relationship exists between price and popularity, indicating that higher-priced candies are slightly more popular overall, but price is not the only determining factor.
•	Clustering: A group of candies in the lower-middle price range (0.2-0.6 price percent) showed win percentages between 30-60%.
•	Outliers: Some lower-priced candies, such as fruity or multi-piece varieties, had very high win percentages, indicating they perform well despite lower costs.
 Candy Rankings Based on Price-Performance:
Candy	Ranking	Rationale
Reese’s Peanut Butter Cups	1st	High win percentage across all price ranges, proving its universal popularity.
Twix	2nd	Strong win percentage regardless of its slightly premium price.
Snickers	3rd	High price-performance correlation, showing consumers are willing to pay more for Snickers.
Sour Patch Kids	4th	Excellent win percentage despite a lower price, making it a value pick.
Peanut M&Ms	5th	Consistent performance across various price ranges.
5. Clustering and Principal Component Analysis (PCA)
By clustering the candies, we identified major groupings based on flavor, price, and texture:
Key Clusters:
•	Cluster 1 (High Sweetness and Popularity): Includes chocolate-based candies like Reese's Peanut Butter Cups and Twix, which are top performers.
•	Cluster 2 (Moderate Sweetness): Features candies like Snickers and Milky Way, which appeal to a different segment of consumers.
•	Cluster 3 (Low Sweetness, Lower Popularity): Contains candies like Almond Joy and 3 Musketeers, which are less popular overall.
PCA Results:
The Principal Component Analysis (PCA) reduced the dataset to four key components, explaining 66.7% of the variance. The most significant drivers of variance were chocolate content, sugar percentage, and price.
Candy Rankings Based on Clustering & PCA:
Candy	Ranking	Rationale
Reese’s Peanut Butter Cups	1st	Falls in the highest-performing cluster (high sweetness, high popularity).
Twix	2nd	Also ranks in Cluster 1 with high appeal due to its caramel and chocolate combination.
Snickers	3rd	Falls into Cluster 2, appealing to those who prefer moderate sweetness with nutty flavors.
Peanut M&Ms	4th	Clusters alongside Snickers in moderate sweetness but remains popular.
Sour Patch Kids	5th	Sits in Cluster 3, providing a contrasting flavor (sour/fruity) to the chocolate-heavy options.
6. Feature Importance and Correlation Analysis
Through feature importance analysis and RandomForestClassifier, we identified the most important predictors of candy popularity:
Top Features:
1.	Chocolate: The most significant factor driving candy popularity.
2.	Price Percentage: Higher-priced candies tend to be more popular, particularly for chocolate and peanut/almond varieties.
3.	Sugar Percentage: Higher sugar content is associated with higher popularity.
4.	Peanut/Almond: Nut-based candies rank highly, especially when combined with chocolate.
Correlation Insights:
•	Fruity Candies: Showed a slight negative correlation with price, indicating that lower-priced fruity candies tend to be more popular.
•	Peanut/Almond Candies: Showed a positive correlation, with higher-priced options performing better in popularity rankings.
 The win percentage distribution showed a clear distinction between high-win candies (median around 75-80%) and low-win candies (median around 40-45%).
Candy Rankings Based on Feature Importance:
Candy	Ranking	Rationale
Reese’s Peanut Butter Cups	1st	Top performer due to high chocolate and peanut content, both key drivers of popularity.
Twix	2nd	Excels due to its chocolate, caramel, and texture combination.
Snickers	3rd	Performs well in the chocolate, peanut/almond, and sugar categories.
Peanut M&Ms	4th	Strong in both chocolate and peanut categories, with high sugar content adding to its appeal.
Sour Patch Kids	5th	Strong in the fruity and pluribus categories, but lower in chocolate and price impact.

7. Final Candy Recommendations
Based on the comprehensive analysis, the following three candies emerge as the top recommendations for Halloween distribution:
1. Reese’s Peanut Butter Cups
Rationale: Reese’s consistently ranks at the top in all analyses, excelling in both win percentage and feature importance. Its classic combination of chocolate and peanut butter appeals to a broad demographic, making it an unbeatable choice. The high consumer willingness to pay a premium for Reese’s reflects its universal appeal across age groups, securing its position as a top favorite.
2. Twix
Rationale: Twix provides a satisfying mix of chocolate, caramel, and a crisp wafer, delivering a unique variety of textures in one candy. This combination makes it highly appealing, offering layers of flavors that resonate with a wide audience. Twix performs strongly in popularity rankings due to its complex taste and texture, making it a standout choice for Halloween treats. Its balanced combination of sweetness and crunch enhances its broad appeal.
3. Snickers
Rationale: Snickers combines chocolate, peanuts, nougat, and caramel into one bar, making it a satisfying choice for those seeking both sweet and salty flavors. Its rich combination of ingredients makes Snickers a hit with consumers who enjoy nut-based treats, and its popularity holds strong across various analytical methods. Snickers offers a heartier candy option that appeals to trick-or-treaters looking for a substantial snack.
Rationale for this Combination:
1.	Diversity in Flavors and Textures:
This selection offers a range of taste experiences—peanut butter and chocolate (Reese’s), chocolate and caramel with a crisp wafer (Twix), and the nutty, chewy richness of Snickers. This variety caters to different preferences and enhances the likelihood of satisfying a broader demographic of trick-or-treaters.
2.	Consistent Popularity:
All three candies rank highly across multiple analyses (flavor analysis, price-performance, clustering, and feature importance), indicating broad consumer appeal. They consistently score well in win percentages and feature high on the popularity scale.
3.	Alignment with Key Features:
The chosen candies align with the most important drivers of candy popularity identified in the analysis—chocolate content, price point, and unique textures. The combination of these features ensures that these candies stand out in terms of consumer preferences.
4.	Wide Demographic Appeal:
With the combination of chocolate-heavy treats (Reese’s, Twix, and Snickers) and multiple textures (smooth, crunchy, and chewy), this selection appeals to a wide variety of taste preferences, increasing the likelihood of satisfying trick-or-treaters of all ages and tastes.
5.	Data-Driven Decision:
This selection is backed by robust data analysis, including insights from win percentages, clustering, and feature importance, ensuring that these choices are not only popular but data-supported as well.
By offering these three popular and diverse options, you maximize the chances of appealing to trick-or-treaters with varying tastes, thereby positioning your house as the most popular Halloween destination on the block.
8. Conclusion
This data-driven approach, using Python for analysis and visualization, provides a clear strategy for selecting the best candies to distribute on Halloween. By offering a balanced mix of chocolate (Reese’s Peanut Butter Cups and Twix) and nut-based options (Snickers), you guarantee appeal to a wide range of candy lovers. These top-performing choices, backed by data, will make your house a favorite stop for trick-or-treaters, ensuring a successful and memorable Halloween candy distribution.

