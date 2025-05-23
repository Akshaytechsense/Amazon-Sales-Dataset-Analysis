🛍️ Amazon Sales Dataset Analysis
📌 Project Overview
E-commerce has revolutionized the way consumers shop, offering convenience, variety, and competitive pricing—all from the comfort of their homes. Among the industry giants, Amazon stands out for its data-rich environment and diverse product catalog. In this project, we dive deep into a curated Amazon product dataset to uncover meaningful patterns and insights that can guide business decisions, improve user experience, and optimize marketing strategies.

Our analysis primarily focuses on customer behavior through product ratings and reviews. We also examine variables like pricing, discounts, product categories, and sentiment to draw conclusions about what drives customer satisfaction. This exploratory data analysis (EDA) forms the foundation for understanding market trends and helps stakeholders—including sellers, marketers, and product teams—take data-driven actions.

📁 Dataset Description
The dataset used in this project includes a wide variety of Amazon products and spans multiple key attributes that describe customer sentiment and product details. It contains the following features:

Product Title: The name or title of the product as listed on Amazon.

Price: The retail price of the product.

Discount Percentage: The amount of discount (if any) offered on the product.

Rating: Average user rating on a scale of 1 to 5.

Review Text: Textual reviews left by customers.

Category: The type or segment the product belongs to, such as Electronics, Office Supplies, Books, etc.

Each of these variables was cleaned and preprocessed to ensure the quality of analysis. This included removing missing values, standardizing data formats, and transforming data types to appropriate formats.

🧹 Data Preprocessing
Before conducting the analysis, several preprocessing steps were performed:

Null Values Handling: Missing values were removed or imputed depending on the context.

Text Normalization: For the review text, stopwords were removed, and words were tokenized for further NLP analysis.

Data Types: Converted string representations of numbers into appropriate numerical formats for analysis.

Outlier Treatment: Outliers in price and ratings were analyzed but retained, as they represented valid business scenarios.

These steps ensured that the dataset was ready for rigorous statistical and visual exploration.

🔍 Key Questions & Analytical Insights
1. How does the discount percentage affect product ratings?
To explore this, we generated scatter plots and correlation matrices between the discount percentage and average customer ratings. Interestingly, we found no significant correlation. This challenges the common assumption that higher discounts equate to better customer satisfaction. It suggests that product value and quality hold more weight than just price reductions.

Business Implication: Retailers should focus on maintaining quality and service, as customers are willing to pay more for products that meet expectations.

2. Which category has the highest average rating?
By grouping data by product category and calculating mean ratings, we identified that the “OfficeProducts” category enjoys the highest average customer satisfaction. This could be due to consistent quality, utility-based purchases, or less subjective preferences in this segment.

Visualization: A bar chart representing average rating per category showed clear leaders and laggards.

Business Implication: Insights like this can help sellers target high-trust categories for new product launches.

3. Is there a correlation between product price and rating?
Price was another key variable of interest. The analysis showed no strong correlation between the price of a product and how well it was rated. Some high-priced products had mediocre reviews, while some low-cost items scored highly.

Business Implication: Sellers should not assume that higher pricing reflects better perceived quality. Instead, customer experience, value for money, and reliability are more impactful.

4. Most common words in positive and negative reviews?
We performed sentiment analysis and created Word Clouds from the review texts. The dataset showed a 98% dominance of positive reviews, reflecting high satisfaction levels. Common positive words included "good," "quality," "value," and "useful."

Word Cloud Visualization: A visual representation of the most frequent words gave immediate insight into customer sentiment and repeated themes in user experiences.

Business Implication: Textual analysis helps identify what features matter most to customers—information that's often lost in quantitative ratings alone.

5. What is the overall rating distribution?
A histogram of ratings showed a high concentration of values between 4.0 and 4.5, indicating a largely satisfied customer base. Few products were rated below 3.0.

Visualization: A density plot helped showcase the skew towards positive ratings.

Business Implication: If customer service or product quality dips, it will likely stand out more starkly against this positively skewed backdrop.

6. Which product received the most reviews, and what is its rating?
By aggregating review counts, we identified the top-reviewed product and its rating. This product maintained a high average rating, reflecting both popularity and performance.

Business Implication: Products with high review counts serve as benchmarks for others. Studying them can reveal strategies that work—be it packaging, pricing, delivery time, or product quality.

📊 Tools & Libraries Used
To perform this end-to-end analysis, the following tools and Python libraries were utilized:

Python – Programming language used for analysis

Pandas – Data manipulation and preparation

NumPy – Numerical computing

Matplotlib & Seaborn – Data visualization

WordCloud – Textual data visualization

Jupyter Notebook / Google Colab – Coding environment

These tools enabled us to carry out efficient, reproducible, and scalable analysis workflows.

📈 Visualizations
Several types of visualizations were used to understand patterns, trends, and relationships:

Bar Charts: To compare average ratings across categories.

Histograms: To display rating distributions.

Scatter Plots: To study relationships like price vs rating.

Word Clouds: To visualize frequent terms in reviews.

Boxplots: To detect distribution and outliers in prices.

Visualization not only made the insights more digestible but also facilitated stakeholder communication.

🧠 Feature Importance (Advanced Analysis)
Although the primary focus was on EDA, basic feature importance techniques were applied using simple regression models to identify which features most affect the purchase decision (proxied by ratings).

Category and Review Text-derived sentiment had more predictive power than price or discounts.

Future Scope: You can extend this project into a supervised machine learning model predicting rating or purchase intent.

🚀 How to Run This Project
Clone or download the repository from GitHub.

Open the Jupyter Notebook (.ipynb) file using Jupyter or Google Colab.

Upload the dataset or connect it via Google Drive.

Execute each cell sequentially to see the full analysis in action.

💡 Business Insights Summary
Discounts are not everything – Customers don’t necessarily give higher ratings when discounts are bigger.

Office Products win on ratings – They are consistently well-received by users.

Price ≠ Quality (in perception) – Customers are smart shoppers and judge quality beyond cost.

Text reviews are gold – Valuable qualitative feedback lies in textual reviews.

Positive bias in data – Most users leave favorable reviews, and deviations from this trend should be examined carefully.

🔮 Future Enhancements
This project can be extended in several directions:

Build a sentiment classifier using NLP techniques like TF-IDF and Logistic Regression.

Cluster similar products based on review content using unsupervised learning.

Develop a recommendation system using collaborative filtering.

Deploy a dashboard using Power BI or Streamlit for real-time business users.

🤝 Acknowledgments
Special thanks to the open-source data community and GitHub contributors whose datasets and discussions made this project possible.

