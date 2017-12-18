
## Add rate template api  

* **url**:  
`https://{BACKEND_API}.yamsafer.me/properties/{PROPERTY_ID}/rates/templates`  

* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **Body**:
    - addButton: true
    - allow_cardless: true || false
    - code: ''
    - id: null
    - is_refundable: true || false
    - name: {NAME}
    - status: true || false
    - rates: {}
    - cancellation_policy_object: 
        ```
        [
            {
                amount: {AMOUNT}, 1, 100
                time: {TIME}, // can have one of the following values 24, 48, 72, 168
                type: {TYPE}, // can have one of the following values 'free', 'night', 'stay'
            },
        ]
        ```
    - benefits: [BENEFIT_ID]
    - payment_method: 2,3 :: 2 => POSTPAID, 3 => DEPOSIT_REQUIRED  
    
* **example**:  
`https://api-staging.yamsafer.me/properties/15252/rates/templates`  
