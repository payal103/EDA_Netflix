# EDA_Netflix
Exploratory Data Analysis Report – Netflix Dataset
This EDA focuses on understanding key numerical features from the Netflix dataset — budget, IMDb rating, watch time, and revenue along with the influence of the type (Movie or Series).

1.Histograms with KDE (Kernel Density Estimation)
Purpose:
Histograms are used to visualize the distribution of a single numerical variable. The KDE curve overlays a smooth estimate of the probability distribution.

Variables Analyzed:
Budget

IMDb Rating

Watch Time

Revenue

Why This Graph:
To understand the spread, central tendency, and skewness of the data.

To identify if the distribution is normal, right-skewed, or left-skewed.

Insights:
Budget and Revenue are right-skewed — most titles had lower budgets and revenues, with a few extremely high ones (potential blockbusters).

IMDb Rating appears close to a normal distribution centered around ~6.2.

Watch Time ranges mostly from 60 to 180 minutes with slight uniformity, suggesting consistent content length.

2. Boxplots
Purpose:
Boxplots are used to identify the range, interquartile spread (IQR), median, and outliers in numerical data.

Why This Graph:
Great for spotting extreme values (outliers).

Helps compare variability and data concentration.

Insights:
All four variables (budget, rating, watch time, revenue) show the presence of outliers.

Revenue and Budget have large IQRs, meaning wide variability — not all expensive productions guarantee high revenue.

Watch Time is fairly consistent with minimal extreme values.

3. Correlation Heatmap
Purpose:
A heatmap of the correlation matrix shows the strength of linear relationships between pairs of numerical variables.

Why This Graph:
Quickly identifies which variables are related.

Helps in feature selection for modeling.

Insights:
Budget is moderately correlated with Revenue — higher spending often brings higher returns, but not always.

IMDb Rating has a weak correlation with revenue — audience ratings may not directly predict earnings.

Watch Time shows very little correlation with any other feature.

4. Scatter Plots
Purpose:
Scatter plots show the relationship between two numerical variables. Each point represents a title (movie/series).

Why This Graph:
Helps detect linear or nonlinear trends, clusters, and outliers.

Useful for observing real-world variability.

Insights:
Budget vs Revenue shows a positive but scattered trend — some low-budget content still earns high revenue (could be viral/low-cost hits).

IMDb Rating vs Revenue has a very loose trend, reaffirming that popularity doesn't always equal profitability.

5. Boxplot by Type (Movies vs Series)
Purpose:
Compares the distribution of a numerical variable (e.g., revenue) between categories.

Why This Graph:
Allows side-by-side comparison of statistics like median, spread, and outliers.

Great for categorical group comparison.

Insights:
Movies tend to have higher median revenue than Series.

Series show slightly more variance in revenue.

Helps inform whether production type influences profitability.

6. Countplot of Type
Purpose:
Displays the frequency count of each category in a categorical variable (e.g., number of Movies vs Series).

Why This Graph:
Useful for detecting imbalance in dataset categories.

Important for understanding dataset composition.

Insights:
One category (likely Movies) dominates the dataset, which may bias predictive models if not addressed.

Imbalance may require techniques like resampling or weighted models in further analysis.

Summary of Key Insights
Feature Insight: Budget & Revenue Positively skewed; few high-budget blockbusters drive massive returns. IMDb Rating Not strongly tied to revenue; critical acclaim ≠ financial success. Watch Time Consistent length for most content (60–180 min). Type Impact Movies usually earn more than Series; but Series are more variable. Data Imbalance Movies likely overrepresented; should be accounted for in modeling.


