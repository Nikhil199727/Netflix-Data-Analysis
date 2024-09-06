# Netflix-Data-Analysis
### Introduction
In today’s entertainment landscape, Netflix is a dominant player, reaching millions of users worldwide. Understanding its user base is crucial for personalizing content and enhancing engagement. This project aims to analyze Netflix's user demographics, subscriptions, and revenue across various countries. By analyzing data such as the number of users per device, age groups, and total revenue by country, the project uncovers trends that may guide future business strategies. We’ll explore key patterns in user behavior and preferences using visual data representations.

### Dataset Description
The dataset for this project was sourced from **Kaggle** and contains data on Netflix users from different countries, including their age, device preferences, subscription types, and monthly revenue. Below is a detailed breakdown:

- **Type and Size**:
  - The dataset consists of rows representing individual Netflix users, with several columns containing demographic and usage information.
  
- **Variables**:
  - `Country`: The country of the user.
  - `Subscription Type`: Type of subscription (e.g., Basic, Standard, Premium).
  - `Device`: The primary device used by the user (e.g., TV, Mobile, PC).
  - `Age`: The age of the user.
  - `Gender`: The gender of the user.
  - `Monthly Revenue`: The monthly subscription revenue from the user.

- **Data Quality**:
  - **Missing values**: No missing values were found in the dataset, as confirmed by the `df_netflix.isna().sum()` check.
  - **Duplicates**: There are no duplicate entries in the dataset, as shown by `df_netflix.duplicated().sum()`.
  - **Measurement Scales**: 
    - **Nominal**: Country, Subscription Type, Device, and Gender.
    - **Numerical**: Age and Monthly Revenue, both measured as continuous variables.

### Objectives of the Project
The key objectives of this project are:
1. **To explore user distribution across different countries** and analyze the user base by gender, device usage, and subscription types.
2. **To identify which age groups are more inclined towards specific devices or subscription types**, and understand how revenue is distributed across these groups.
3. **To examine trends in user behavior based on country**, providing insights into how Netflix is consumed differently across the globe.

**Formulated Questions**:
- What are the most popular devices used by Netflix users across different countries?
- How does the user base differ between subscription types?
- What is the revenue distribution per country, and which countries generate the most income for Netflix?
- How does the age distribution of Netflix users vary by device and country?

### Tools
- **Libraries used**: 
  - `pandas` for data manipulation.
  - `numpy` for numerical computations.
  - `matplotlib` and `seaborn` for data visualization.
  
- **Programming Language**: Python was used for all data processing and visualization.

### Insights
1. **Number of Users in Different Countries**:
   The bar plot of Netflix users across countries shows that certain countries, like the U.S. and India, have a significantly higher number of users than others. This indicates Netflix's strong presence in these countries, which could suggest a larger market potential in those regions.

   ![download](https://github.com/user-attachments/assets/ba336acc-4ca2-4bfd-9a0d-85bc659cb03a)

2. **Subscription Type Analysis**:
   The majority of Netflix users prefer the **Standard** and **Premium** subscription tiers, as reflected by the bar chart on subscription types. This suggests a preference for higher-tiered services with more features, such as HD streaming and multi-device usage.

![download](https://github.com/user-attachments/assets/4cd7e8f3-9389-47a9-87e5-9373f8fb20b4)


3. **Device Preference**:
   The bar graph comparing devices shows a clear trend: most Netflix users access the service via **TVs** and **mobile devices**, with fewer using PCs. This highlights how users prefer the larger screens of TVs or the convenience of mobile devices for content consumption.

![download](https://github.com/user-attachments/assets/a33da492-147a-4d69-b930-0f15db5d1d4a)

4. **Age Group Analysis**:
   A breakdown of users by age group shows that the largest number of Netflix users falls within the **19-30** and **31-40** age ranges. These two groups constitute the bulk of the audience, indicating that Netflix appeals primarily to young adults and middle-aged individuals.

![download](https://github.com/user-attachments/assets/ad068798-902d-424a-8b7f-54ddd52840e3)

5. **Revenue Distribution Across Countries**:
   The revenue analysis reveals that countries with a larger user base, such as the U.S. and Canada, generate the highest revenues. This correlates with user count but also reflects the higher subscription costs in these regions. Countries with fewer users contribute significantly less to Netflix’s total revenue.

![download](https://github.com/user-attachments/assets/625e3c3c-7ede-4eb0-beff-76016497bb7b)

6. **Gender Analysis**:
   In the gender-based analysis across countries, it was found that male and female user distributions are fairly balanced, although some countries have slight gender disparities in user numbers.

![download](https://github.com/user-attachments/assets/d8c84022-660d-4832-8c4f-9844a88515b0)

7. **Pivot Tables**:
   - The first pivot table provides a detailed breakdown of users by country, subscription type, and gender, showing the distribution of males and females for each subscription type in every country.
   - The second pivot table examines the relationship between users' age group, country, and device preference. It highlights the tendency of younger users to favor mobile devices, while older users are more inclined towards using TVs.

Both Tables can be seen in the Analysis Code

### Recommendations and Future Analysis
1. **Device-Specific Promotions**: Netflix can target promotions and content recommendations based on device preferences. For instance, mobile users might appreciate more short-form or downloadable content.
   
   
3. **Regional Strategies**: Tailoring content and subscription models to countries with a smaller user base could increase user acquisition. Offering localized content in smaller regions might also enhance engagement.

4. **Subscription Type Insights**: Since Standard and Premium subscriptions dominate, Netflix could focus on promoting additional features (like 4K streaming or family accounts) to incentivize upgrades from Basic subscriptions.

5. **Further Research**: Future analyses could investigate:
   - **Content preferences** in different countries to determine what genres or types of shows drive user engagement.
   - **Churn rates** in each region to identify where Netflix might face challenges in retaining users.
   - **Price sensitivity**: Testing how changes in subscription prices affect user numbers and revenue per country.

These insights can help Netflix optimize its offerings, enhance user engagement, and tailor its strategy to meet the diverse needs of its global user base.
