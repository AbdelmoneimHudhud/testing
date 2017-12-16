## Get property api  
###recent
* **url**:  
https://{BACKEN_API}.yamsafer.me/properties/{PROPERTY_ID}/orders/recent?limit={LIMIT}&order={asc|desc}&page=1&sort={SORT_OPTION}  

**sort options** :  

- confirmation_code
- customer.first_name
- created_at
- checkin_date
- checkout_date
- nights
- taxed_total_price
- status_description

* **request type**:  
GET  

* **example**:  
https://api-staging.yamsafer.me/properties/12916/orders/recent?limit=25&order=asc&page=1&sort=checkout_date

###between start-end dates 
* **url**:  
https://{BACKEND_API}/properties/{HOTEL_ID}/orders/?limit={LIMIT}&checkout_date_start={START_DATE}&checkout_date_end=${endDate}&order=created_date&page=1&sort=dsc&api_key=bfdd9c41d51bfdd04bdb096631ed8e3f  
* **request type**:  
GET  

* **example**:  
https://api-staging.yamsafer.me/properties/12916/orders/recent?limit=25&order=asc&page=1&sort=checkout_date

