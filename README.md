## 🗂 Dataset Description
The project is based on structured data stored in multiple tables:

- **customers**: Customer details and city information  
- **sales**: Transaction data (amount, product, date)  
- **products**: Coffee product details  
- **cities**: City data including population and rent  

---

## 🛠 Tools Used
- SQL (MySQL)
- Excel

---

## 📊 Business Problems Solved
- Estimated coffee consumers (25% of population)
- Total revenue in Q4 2023
- Units sold per product
- Average sales per customer in each city
- Top 3 selling products per city
- Unique customers per city
- Average sale & rent per customer
- Monthly sales growth rate
- Top 3 cities based on sales performance

---

## 🔍 Key SQL Queries

### Estimated Coffee Consumers
```sql
SELECT 
    city,
    population,
    population * 0.25 AS estimated_coffee_consumers
FROM cities;
