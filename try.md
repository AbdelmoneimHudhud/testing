## Get property api  
### Two variations  
1. recent 
* **url**:  
`https://{BACKEN_API}.yamsafer.me/properties/{PROPERTY_ID}/orders/recent?limit={LIMIT}&order={asc|desc}&page=1&sort={SORT_OPTION}`  

* **sort options** :  
    - confirmation_code
    - created_at
    - checkin_date
    - checkout_date
    - taxed_total_price
    - status_description
    - customer.first_name
    - nights

* **request type**:  
GET  

* **example**:  
https://api-staging.yamsafer.me/properties/12916/orders/recent?limit=25&order=asc&page=1&sort=checkout_date

2. between start-end dates  
* **url**:  
https:{BACKEND_API}/properties/{PROPERTY_ID}/orders/?{FILTER_CRITERIA}_start={START_DATE}&{FILTER_CRITERIA}_end={END_DATE}&limit={LIMIT}&order={SORT_OPTION}&page=1&sort={asc|desc}&api_key=bfdd9c41d51bfdd04bdb096631ed8e3f  

* **filtering criteria options** :  
    - created_date
    - checkin_date
    - checkout_date

* **sort options** :As in the list for the first request.

* **request type**:  
GET  

* **example**:  
https://api-staging.yamsafer.me/properties/12916/orders/?checkout_date_end=2017-12-17&checkout_date_start=2017-12-16&limit=50&order=created_date&page=1&sort=dsc&api_key=bfdd9c41d51bfdd04bdb096631ed8e3f

