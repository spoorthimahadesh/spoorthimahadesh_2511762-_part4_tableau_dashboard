# spoorthimahadesh_2511762-_part4_tableau_dashboard
# Task 1: Connect and Inspect Data

## Dataset Overview
The dataset was imported into Tableau from the Excel file `dashboard_sales_data.xlsx`.

Total Fields: 20

---

## Field Classification

### 1. Date Fields
| Field Name | Data Type |
|------------|-----------|
| order_date | Date |
| ship_date | Date |

### 2. Geographic Fields
| Field Name | Data Type |
|------------|-----------|
| region | String (Geographic Role: Region) |
| state | String (Geographic Role: State/Province) |
| city | String (Geographic Role: City) |

### 3. Categorical Fields
| Field Name |
|------------|
| order_id |
| customer_id |
| customer_segment |
| category |
| sub_category |
| product_name |
| ship_mode |
| campaign_channel |

### 4. Numerical Measures
| Field Name | Data Type |
|------------|-----------|
| sales | Decimal Number |
| quantity | Whole Number |
| discount | Decimal Number |
| profit | Decimal Number |
| delivery_days | Whole Number |
| customer_rating | Decimal Number |

### 5. Binary / Flag Fields
| Field Name | Description |
|------------|-------------|
| return_flag | Binary indicator where 1 = Returned, 0 = Not Returned |

---

## Assumptions

1. `order_date` represents the date when the order was placed.
2. `ship_date` represents the date when the order was shipped.
3. `return_flag` is treated as a binary field:
   - `0` = Product not returned
   - `1` = Product returned
4. Geographic fields (`region`, `state`, `city`) are assigned appropriate geographic roles in Tableau for map visualizations.
5. `sales`, `profit`, and `discount` are considered continuous numerical measures.
6. `customer_rating` is assumed to be a score on a fixed scale and is treated as a numerical measure.
7. No missing values or duplicate records were identified during the initial inspection.
