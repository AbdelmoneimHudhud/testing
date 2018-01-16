## Add dynamic rule api

* **url**:  
`https://{BACKEND_API}.yamsafer.me/properties/{PROPERTY_ID}/rates/rules`


* **request type**:  
POST  

* **headers**:
    - Accept: 'application/json'
    - cookie: {cookie}  

> There are 4 types of rules and each rule has several options.  
> Example on adding a Same day booking rule so rate turns to be cardless.   

* **body**:  
    ```
    {  
        action: 
        {
            is_cardless: true,
            is_prepaid: false,
            remarks: "RATE_BECOMES_CARDLESS",
        },
        actionCode: "RATE_BECOMES_CARDLESS",
        bwTime: {bwTime},
        daysList: {
        1:{title: "MON"}
        2:{title: "TUE", status: true}
        3:{title: "WED"}
        4:{title: "THU"}
        5:{title: "FRI"}
        6:{title: "SAT"}
        7:{title: "SUN"}
        },

        dates:{},
        expanded: false,
        expandedActions: {},//here your can do an example on extranet with expanded action,
        id: null,
        is_published: true,// set value to false, rule will be created but unpublished,
        moreConditions: false,
        rates_templates: [], //array of rate templates ids to apply rule on,
        trigger: 
        {
            time: 3, // notice value in other examples
        },
        type:"BOOKING_WINDOW",
    },  
    ```

* **example**:  
`https://api.yamsafer.me/properties/411296/rates/rules/`  
