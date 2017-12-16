## Set properties surcharges api

> This details for edit and delete surcharges, deleting a suracharge is the same as update but you don't send the surcharge record in the body.

* **url**:  
`https://{BACKEND_URL}/properties/{PROPERTY_ID}/surcharges`


* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **body**:  
```
[  
    {  
        id: {ITS_ID},  
        is_included: true || false,  
        code: {ITS_CODE},  
        amount_type: percent || amount,  
        code: {CODE}  
    },  
]  
```

* **CODE options**:  
    * VAT for TAXES, id: 972
    * per_night for HOTEL FEE, id: 137
    * There is more options, you can open extranet:: property page:: and try to add/edit surcharges for more options

* **example**:  
`https://api-staging.yamsafer.me/properties/12916/surcharges`  
