
#Overview
This project analyzes 12 months of sales data to identify trends, patterns, and key performance indicators (KPIs). The analysis includes data cleaning, exploratory data analysis, time series analysis, segmentation. The goal is to gain valuable insights into sales performance and generate actionable recommendations for business improvement.

#Tools I used
- Programming Languages: Python (with libraries like Pandas)
- Data Visualization Libraries: Matplotlib, Seaborn.

# Analysis
## 1. What are Monthly Sales and how it differs over the year?

### Visualize Data
```python

sns.set_theme(style="ticks")
sns.barplot(data=df_monthly_sales, x='Month', y='Total Price', hue='Month', palette='dark:b_r')
plt.title('Monthly Sales')
plt.xlabel('2019')
plt.ylabel('Total Sales Per Month ($USD)')
ax = plt.gca()
ax.yaxis.set_major_formatter(plt.FuncFormatter(lambda x, loc: f'${int(x/1000000)}M'))
sns.despine()
plt.show()

```

### Results 
![Visulization For the above given code](plots/montly_sales.png)

### Insights 

- Seasonal Fluctuations: There's a clear peak in sales during December, suggesting a strong holiday season influence. This could be due to increased consumer spending during the festive season.
- Month-to-Month Variation: Sales fluctuate from month to month, with some months experiencing higher sales than others. This variation could be due to various factors like seasonal demand, marketing campaigns, or economic conditions.

###Business Strategies 

- Holiday Promotions: Leverage the high demand during the holiday season by offering attractive promotions and discounts.
- Targeted Promotions: Run targeted promotions or campaigns during low-performing months to stimulate demand.
- Inventory Management: Ensure adequate inventory levels to meet the increased demand during peak months.


