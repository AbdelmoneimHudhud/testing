## Set properties/rooms images rank api

* **url**:  
`https://{BACKEND_API}.yamsafer.me/properties/{PROPERTY_ID}/images/ranks`


* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **body**:  
    ```
    [  
        {  
            id: {IMAGE_ID},  
            path: {IMAGE_PATH},  
            rank: {INDEX_IN_ARRAY},  
            score: 1,  
            response: 
                ```
                link: 'photos/'
                ```  
        },  
    ]  
    ```

* **example**:  
`https://api-staging.yamsafer.me/properties/15252/images/ranks`  
