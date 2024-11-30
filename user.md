### Register User (/api/users/register)

This endpoint allows you to register a new user.

#### Request Body

json
```
{
  "name": "Test User",
  "email": "test@mail.com",
  "password": "Test_12345"
}
``` 

#### Response

Upon successful registration, the API returns a JSON object with the following fields:

json
```
{
    "success": true,
    "message": "User registered successfully",
    "data": {
        "id": 4,
        "name": "Test User",
        "email": "test@mail.com",
        "role": "ROLE_USER",
        "status": "ACTIVE"
    }
}
```

### Login (/api/auth/login)

This endpoint allows users to log in by providing their email and password.

#### Request Body

json
```
{
  "email": "test@mail.com",
  "password": "Test_12345"
}
```
    

---

#### Response

Upon successful login, the API returns a JSON object with the following fields:

json
```
{
    "success": true,
    "message": "User registered successfully",
    "data": {
        "id": 4,
        "name": "Test User",
        "email": "test@mail.com",
        "role": "ROLE_USER",
        "status": "ACTIVE"
    }
}
```

### Get Users (/api/admin/users)

This endpoint retrieves a list of users with their details. The response is in JSON format and has a schema as follows:

json
```
{
    "success": true,
    "message": "All users retrieved successfully",
    "data": [
        {
            "id": 3,
            "name": "Normal User",
            "email": "normal@mail.com",
            "role": "ROLE_USER",
            "status": "ACTIVE"
        },
        {
            "id": 4,
            "name": "Test User",
            "email": "test@mail.com",
            "role": "ROLE_USER",
            "status": "ACTIVE"
        }
    ]
}
```
