# ecommerce-transaction-analysis

## Project Objective
This project analyzes e-commerce transaction data to uncover trends in sales performance, customer behavior, and refund dynamics across products, channels, and geographies.

## Key Business Questions
- Which products, countries, regions, and channels drive the highest net revenue?
- How do discounts, taxes, and currency conversion affect final USD revenue?
- What refund patterns emerge by product, payment method, region, and time?
- Which geographic areas underperform or outperform on revenue and refund rates?

## Dataset Description
The transaction dataset includes the following fields:

- `event_id`: Unique transaction event identifier
- `event_type`: Type of event (e.g., purchase, refund)
- `event_date`: Date/time of the event
- `customer_id`: Unique customer identifier
- `product_id`: Product identifier
- `country`: Customer or transaction country
- `latitude`: Geographic latitude of the transaction
- `longitude`: Geographic longitude of the transaction
- `region`: Regional grouping of the transaction
- `channel`: Sales channel (e.g., web, mobile, marketplace)
- `payment_method`: Payment method used
- `currency`: Local transaction currency
- `quantity`: Number of units purchased
- `unit_price_local`: Unit price in local currency
- `discount_code`: Applied discount code (if any)
- `discount_local`: Discount amount in local currency
- `tax_local`: Tax amount in local currency
- `net_revenue_local`: Net revenue in local currency
- `fx_rate_to_usd`: Exchange rate from local currency to USD
- `net_revenue_usd`: Net revenue converted to USD
- `is_refunded`: Refund status flag
- `refund_datetime`: Date/time of refund (if refunded)
- `refund_reason`: Reason for refund (if refunded)

## Methodology
The analysis follows four phases:

1. **Data Cleaning**
   - Validate schema and data types
   - Handle missing/invalid values
   - Standardize date/time and categorical fields
   - Remove duplicates and resolve inconsistent records

2. **Feature Engineering**
   - Create derived time features (day, week, month, quarter)
   - Compute revenue and refund KPIs
   - Build discount and tax impact metrics
   - Construct geographic and channel-level aggregates

3. **Exploratory Analysis**
   - Analyze revenue trends over time
   - Compare performance by product, channel, payment method, and geography
   - Visualize refund distributions and outliers
   - Investigate relationships among discounting, refunds, and net revenue

4. **Insights Generation**
   - Identify key revenue drivers and risk areas
   - Surface refund hotspots and likely operational causes
   - Recommend opportunities for pricing, channel optimization, and regional strategy

## Expected Insights
- **Revenue analysis**: Top/bottom segments by product, channel, region, and country, with trend-based seasonality insights.
- **Refund patterns**: High-risk combinations of products, payment methods, and geographies associated with elevated refund rates.
- **Geographic performance**: Location-level performance mapping using latitude/longitude to highlight strong and weak markets.
