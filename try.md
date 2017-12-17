
## Set properties policies api

* **url**:  
`https://{BACKEND_URL}/properties/{PROPERTY_ID}/policies`


* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **body**:  
```
[
    {
        characteristic_id: {ID},
        chargeable: 0 || 1, 
        price: {PRICE}, 
        metadata: 
            {
                {META_DATA_KEY}: {META_DATA_DESCRIPTION},
                {META_DATA_KEY}: {META_DATA_DESCRIPTION},
            }
    }
] 
```

* **meta data key options**:  
    * 'number_of_beds' for characteristic_id:221 
    * 'max_age' for characteristic_id: 222 and 220
    * 'number_of_children' for characteristic_id: 219 and 223

* **meta data descriotion options**:  
    * 6,7,8,12,16,17:: example: 'children 6 years or younger', for characteristic_id: 222
    * 'adults', for characteristic_id: 222
    * 1,2,3:: example: '2 infants', example: '1 infant', for characteristic_id: 219
    * 1,2,3,4:: example: '3 years or younger', for characteristic_id: 220
    * 3,4,...,12:: example: '10 years or younger', for characteristic_id: 223
    * 1,2,3,4:: example: '3 children', for characteristic_id: 223
* **example**:  
`https://api-staging.yamsafer.me/properties/12916/surcharges`  
