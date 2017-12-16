## Set properties payments api
> Basicaly it's same as the set property details api, but here you put the payments ids in the payments array , example : `payments:["188"]`  


* **url**:  
`https://{BACKEND_URL}/properties/{PROPERTY_ID}`


* **request type**:  
PUT  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

* **body**:
    - currency_code: {CURRENCY_CODE}
    - cvc: true || false
    - is_cardless: true || false
    - latitude: {LATITUDE}
    - longitude: {LONGITUDE}
    - low_rate: {LOW_RATE}
    - number_of_accommodations: null
    - payments: []
    - postal_code: {POSTAL_CODE}
    - propertyID: {PROPERTY_ID}
    - stars: {STARS}
    - type: {PROPERTY_TYPE}
    - ar: ```{  
        address: {ADDRESS},  
        description: {DESCRIPTION},  
        id: {ID},  
        locale: 'ar',  
        name: {PROPERTY_NAME},  
        property_id: {PROPERTY_ID},  
        should_follow: 0 || 1,  
        slug: {slug}  
    }```  
    - en: ```{  
        address: {ADDRESS},  
        description: {DESCRIPTION},  
        id: {ID}.  
        locale: 'en',  
        name: {PROPERTY_NAME},  
        property_id: {PROPERTY_ID},  
        should_follow: 0 || 1,  
        slug: {slug}  
    }  ```
    - images: ```[  
        {  
            category: normal || cover  
             id: {IMAGE_ID}  
            path: {IMAGE_PATH}  
             rank: {IMAGE_RANK}  
        },  
    ]  ```
* **example**:  
`https://api-staging.yamsafer.me/properties/12916`  

