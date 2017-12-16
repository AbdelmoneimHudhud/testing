## Login api

* **url**:
https://{BACKEND_API}.yamsafer.me/en/users/login

* **request type**:
POST

* **body**:
    - username : {USER_NAME}
    - password : {PASSWORD}
    - scope : extranet
    - remember : true || false

* **response example**:
```
{
    "data": {
        "id": 3,
        "username": "walaa",
        "email": "walaa@yamsafer.me",
        "phone": null,
        "access_token": "7132972545f72cc1fa664e27b2d7b9e7",
        "roles": [
            {
                "id": 37,
                "name": "Admin"
            },
            
        ],
        "properties": [
            {
                "id": 12916,
                "name": "Palestine Plaza Hotel",
                "coverImage": "https://images.yamsafer.me/images/medium/296635/14731321_1168812513202946_2245808351646566489_n.jpg",
                "slug": "en/palestine/ramallah-and-al-bireh/hotel/palestine-plaza-hotel",
                "pre_paid": false,
                "stars": "4",
                "city_id": "625",
                "country_id": 170,
                "latitude": "31.9170391",
                "longitude": "35.2069801",
                "currency_code": "USD",
                "sync_with_ical": false
            },
        ],
        "permissions": [
            {
                "id": 82,
                "name": "MANAGE_OWNED_USERS",
                "display_name": "Can only manage his owned users"
            },
        ],
        "fire_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJoYW1tYW1AeWFtc2FmZXIubWUiLCJzdWIiOiJoYW1tYW1AeWFtc2FmZXIubWUiLCJhdWQiOiJodHRwczpcL1wvaWRlbnRpdHl0b29sa2l0Lmdvb2dsZWFwaXMuY29tXC9nb29nbGUuaWRlbnRpdHkuaWRlbnRpdHl0b29sa2l0LnYxLklkZW50aXR5VG9vbGtpdCIsInVpZCI6IjVjNzVhYWJjYzIwYTMzYmUxM2E0NDY2ZjE1NWQ5YzdjIiwiaWF0IjoxNTEzNDE1Mjk1LCJleHAiOjE1MTM0MTg4OTV9.mjjzRfO10NTc7Ckj9eVcRAcGuH7-Uj-0HFITQYz6mks"
    },
    "message": "User logged in successfully"
}
```
