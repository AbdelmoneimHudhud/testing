
## Update property accommodations availability as bulk availability api  

* **url**:  
`https://{BACKEND_API}.yamsafer.me/properties/{PROPERTY_ID}/availabilities`  

* **request type**:  
PUT  
 
* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **Body**:
    - accommodation_ids: 
        ```
        ['ACCOMM1_ID', 'ACCOMM1_ID']
        ```
    - allotment: {ALLOTMENT}
    - force: null
    - dates:
        ```
        ['date0', ..., 'endDate']// example : ["2017-12-19", "2017-12-20", "2017-12-21"]
        ```
    
* **example**:  
`https://api-staging-3.yamsafer.me/properties/12188/availabilities`  
