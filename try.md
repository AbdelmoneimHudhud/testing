
## Properties page :: new property api

* **url**:
`https://{BACKEND_API}.yamsafer.me/en/admin/properties`  

* **request type**:
POST

 * **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

 * **body**:
    - business_model: 1 || 
    - city_id: {CITY_ID}
    - city_name: {CITY_NAME}
    - commission: {COMMISSION}
    - currency_code: {CURRENCY_CODE}
    - is_cardless: true || false
    - latitude: {LATITUDE}
    - longitude" {LONGITUDE}
    - low_rate: {LOW_RATE}
    - number_of_accommodations: {# OF ACC}
    - postal_code: {POSTAL_CODE}
    - rank: {RANK}
    - stars: {STARS}
    - type: {TYPE}
    - en: {
        - address: {EN_ADDRESS}
        - description: {<p>EN_DESCRIPTION</p>}
        - name: {EN_NAME}
        }
    - ar: {
        - address: {AR_ADDRESS}
        - description: {<p>AR_DESCRIPTION</p>}
        - name: {AR_NAME}
        }
    - translations: {
        - en: {
          - address: {EN_ADDRESS}
          - description: {<p>EN_DESCRIPTION</p>}
          - name: {EN_NAME}
          },
        - ar: {
          - address: {AR_ADDRESS}
          - description: {<p>AR_DESCRIPTION</p>}
          - name: {AR_NAME}
          }
      }
    - suppliers: 
      [
       - {// local
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 1
          },
       - {// expedia
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 2
          },
       - {// local-checkout
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 3
          }, 
       - {// hotelbeds
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 4
          }, 
       - {// google
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 5
          }, 
       - {// derbysoft
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 4
          },  
       - {// DOTW
          - active: 0 || 1
          - property_supplier_id: {ID} // only send the property if it has a value.
          - supplier_id: 4
          }, 
      ]

* **example**:  
`https://api.yamsafer.me/en/admin/properties`  
