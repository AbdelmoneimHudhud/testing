
## Update rate template availability api 
> To add a rate template to an accommodation, send the same request with the new rate template details. 

* **url**:  
`https://{BACKEND_API}.yamsafer.me/properties/{ACCOMM_ID}/accommodations/{ACCOMM_ID}/availabilities`  

* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **Body**:
    - allotment: {ALLOTMENT}
    - dates:  
        ```
        ['date0', ..., 'endDate']// example : ["2017-12-19", "2017-12-20", "2017-12-21"]
        ```
    - availabilities: // contains object of the rate template intended to be changed
        ```
        {
            {//firt rate templete to be changed
                occupancy: {OCCUPANCY},
                promotion_rate: {PROMO_RATE},
                rate: {RATE},
                rate_template_id: {RATE_TEMPLATE_ID}
            },
            {//second rate template to be chnaged, can be as the same previous rate template but with different occupancy.
                occupancy: {OCCUPANCY},
                promotion_rate: {PROMO_RATE},
                rate: {RATE},
                rate_template_id: {RATE_TEMPLATE_ID}
            },
        }
        ```
    
* **example**:  
`https://api-staging-3.yamsafer.me/properties/12188/accommodations/4942/availabilities`  
