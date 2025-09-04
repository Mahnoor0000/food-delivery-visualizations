# Food Delivery Data Analysis

##  Project Overview
This project explores **online food delivery trends** using a dataset of customer orders.  
The analysis focuses on understanding **ordering behavior, delivery performance, and customer satisfaction**.  
Through data preprocessing, exploratory data analysis (EDA), and visualizations, meaningful insights are derived to help optimize food delivery services.  

---

##  Dataset
The dataset contains the following key columns:
- `order_id` → Unique identifier for each order  
- `customer_id` → Unique identifier for customers  
- `restaurant_name` → Restaurant fulfilling the order  
- `cuisine_type` → Type of cuisine ordered  
- `cost_of_the_order` → Total cost of the order  
- `day_of_the_week` → Whether the order was placed on a weekday/weekend  
- `rating` → Customer rating (1–5 scale, some missing values handled)  
- `food_preparation_time` → Time taken by the restaurant to prepare food  
- `delivery_time` → Time taken to deliver the order  

---

##  Preprocessing Steps
- Handled missing ratings (`Not given` → replaced with median).  
- Dropped irrelevant identifiers (`customer_id`).  
- Created new features:
  - `total_time = food_preparation_time + delivery_time`  
  - `cost_category` using cost bins.  

---

## Visualizations & Insights
The following visualizations were created to analyze the dataset:

1. **Count Plot of Cuisine Types**  
   → Shows most popular cuisines.  

2. **Boxplot of Delivery Time by Cuisine**  
   → Highlights delivery speed differences across cuisines.  

3. **Heatmap of Delivery Time by Cuisine and Rating**  
   → Examines how delivery times vary with customer satisfaction.  

4. **Trend of Delivery Time Across Orders**  
   → Sequential view of delivery times (proxy for time series).  

5. **Dashboard-style Summary**  
   - Avg delivery time per cuisine  
   - Distribution of food preparation times  
   - Ratings distribution  

**Key Findings:**
- **Korean cuisine** is delivered fastest (~20 mins), while **French and Vietnamese** are slower (~26–27 mins).  
- Most orders are delivered in **23–26 minutes**, showing consistency.  
- Ratings are strongly skewed toward **5 stars**, meaning high customer satisfaction.  
- High-cost orders do **not strongly affect delivery times**, though premium orders may be prioritized.  



---

## License
This project is licensed under the MIT License.  
