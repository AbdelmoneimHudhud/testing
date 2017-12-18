
## Add an accommodation api  

* **url**:  
`https://{BACKEND_api}.yamsafer.me/properties/{PROPERTY_ID}/accommodations/`  

* **request type**:  
POST  

* **Body**:
    - accommodation_type: {ACCOMMODATION_TYPE}// you can get the options throug .../accommodations/template api
    - furnitures: []
    - images: []
    - isMultipleUnit: true || false
    - is_connected: 1 || 0
    - max_children: {CHILDREN_COUNT}
    - max_occupancy: {MAX_OCCUPANCY}
    - occupancy: {OCCUPANCY}
    - quantity: {QUANTITY}
    - size: {SIZE}
    - smoking_preferences: 
    - suppliers: []
    - icalendars:  
        ```
        {  
            hash: ''
        }  
        ```
    - facilities:  
        ```
        [
            {
                code: {CODE},
                is_ensuite: true || false,
                name: {NAME},
                occupancy: {OCCUPANCY},
                size: {SIZE},
                furnitures: 
                    ```
                    [
                        {
                            code: {CODE},
                            id: {ID}
                        }
                    ]
                    ```
            }
        ]
        ```
    - ar: 
        ```
        {
            description: {ARABIC_DESCRIPTION},
            name: {ARABIC_NAME}
        }
        ```
    - en:
        ```
        {
            description: {ENGLISH_DESCRIPTION},
            name: {ENGLISH_NAME}
        }
        ```
* **example**:  
`https://api-staging.yamsafer.me/properties/15252/accommodations/`  
