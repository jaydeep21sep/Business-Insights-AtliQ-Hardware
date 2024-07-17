# Business-Insights-AtliQ-Hardware

**Objective**: Develop a strategic framework to generate actionable insights that will transform Atliq Hardware's operations. These insights, derived from an in-depth analysis of customer behavior, transaction history, product trends, and regional dynamics, aim to drive significant business improvements and competitive advantage.this data-driven approach ensures evidence-based decisions, reducing risks and maximizing opportunities.

### AtliQ Business model:

AtliQ has a manufacturing unit and supplies gadgets to customers globally. AtliQ sells hardware gadgets to customers like Croma, BestBuy, Amazon, Staples, and Flipkart, who then sell these products to end users. Here, "customer" refers to Atliq's direct buyers, while "consumer" refers to the end users.

AtliQ uses 3 channels to sell their products
  - Retailer
  - Direct via their own stores
  - Distributors

### Data Set Information

#### Table Data
1. dim_customer: contains customer-related data
2. dim_product: contains product-related data
3. fact_gross_price: contains gross price information for each product
4. fact_manufacturing_cost: contains the cost incurred in the production of each product
5. fact_pre_invoice_deductions: contains pre-invoice deductions information for each product
6. fact_sales_monthly: contains monthly sales data for each product.

#### Column Description for dim_customer table:
1.customer_code: Unique ID for each customer.
2.customer: Names of customers (e.g., Atliq Exclusive, Flipkart).
3.platform: Sales method (Brick & Mortar(Offline), E-Commerce(Online)).
4.channel: Distribution method (Retailers, Direct, Distributors).
5.market: Countries where the customer is located.
6.region: Geographic region (APAC, EU(Europe), NA(North America), LATAM).
7.sub_zone: Sub-regions (India, ROA, ANZ, SE, NE, NA, LATAM).

#### Column Description for dim_product table:
1.product_code: Unique ID for each product.
2.division: Product groups (P & A, N & S, PC).
3.segment: Product categories (Peripherals, Accessories, Notebook, Desktop, Storage, Networking).
4.category: Specific subcategories within the segment.
5.product: Names of products.
6.variant: Product versions (Standard, Plus, Premium).

#### Column Description for fact_gross_price table:
1.product_code: Unique ID for each product.
2.fiscal_year: Fiscal period of sale (starting in September).
3.gross_price: Initial product price before deductions/taxes.

#### Column Description for fact_manufacturing_cost:
1.product_code: Unique ID for each product.
2.cost_year: Fiscal year of product manufacture.
3.manufacturing_cost: Total production cost (materials, labor, overhead).

#### Column Description for fact_pre_invoice_deductions:
1.customer_code: Unique ID for each customer.
2.fiscal_year: Fiscal period of sale.
3.pre_invoice_discount_pct: Pre-invoice discount percentage.

#### Column Description for fact_sales_monthly:
1.date: Sale date (monthly format for 2020 and 2021).
2.product_code: Unique ID for each product.
3.customer_code: Unique ID for each customer.
4.sold_quantity: Number of units sold.
5.fiscal_year: Fiscal period of sale.




