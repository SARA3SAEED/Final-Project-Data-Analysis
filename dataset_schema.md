## **BigQuery** For Our DataSet:

[Access Dataset on BigQuery](https://console.cloud.google.com/bigquery?project=smart-bite-final-da-project&folder&organizationId&p=smart-bite-final-da-project&d=Tiller_Dataset)

# Dataset Schema

## `order_data` Table
- **id_order**: Order ID
- **id_store**: Store ID
- **id_table**: Table ID
- **id_waiter**: Waiter ID
- **id_device**: Device ID where the order has been placed
- **date_opened**: Table open date
- **date_closed**: Table close date
- **dim_status**: Order status
- **dim_source**: Name of device where the order has been placed
- **m_nb_customer**: Number of customers associated with the order
- **m_cached_payed**: Price paid
- **m_cached_price**: Price to pay

## `order_line` Table
- **id_order_line**: ID of ordered item
- **id_order**: Order ID
- **date_opened**: Date item is ordered
- **date_created**: Date item is saved
- **m_quantity**: Quantity
- **m_unit_price**: Price
- **m_unit_price_exc_vat**: Price without VAT
- **m_total_price_inc_vat**: Price with VAT
- **m_total_price_exc_vat**: Total price without VAT
- **m_tax_percent**: VAT percentage applied
- **m_discount_amount**: Discount
- **dim_type**: Types (products, discounts, etc.)
- **dim_category**: Category (beverages, etc.)
- **dim_name**: Item’s name (risotto, etc.)
- **dim_status**: Item status
- **dim_feature_type**: Item type
- **dim_unit_measure**
- **dim_unit_measure_display**

## `payment_data` Table
- **id_pay**: Payment ID
- **id_order**: Order ID
- **dim_status**: Payment status
- **dim_type**: Payment type
- **m_amount**: Payment amount
- **m_cashback**
- **m_credit**
- **date_created**

## `store_data` Table
- **id_store**: Store ID
- **date_created**: Subscription date
- **dim_zipcode**
- **dim_country**
- **dim_currency**


