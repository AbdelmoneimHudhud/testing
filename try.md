## Set properties surcharges api

* **url**:  
`https://{BACKEND_URL}/properties/{PROPERTY_ID}/surcharges`


* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **body**:  
[  
    {  
        id: {ITS_ID},  
        is_included: true || false,  
        code: {ITS_CODE},  
        amount_type: percent || amount,  
        code: {CODE}  
    }  
]  
 
* **example**:  
`https://api-staging.yamsafer.me/properties/12916/surcharges`  
