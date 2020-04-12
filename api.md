# API Specification


## 1 Register

Endpoint ```/register```

### RegisterRequest

```
{
    "email": "<email address>"
}
    
```

### RegisterResponse
```
{
    "status": {
        "success": false,
        "error": "<error message>"
    },
    "auth_token": "<token>"
}
    
```


## 2 Login

Endpoint ```/login```

### LoginRequest
```
{
    "auth_token": "<token>",
    "password": "<password>"    
}
```

### LoginResponse
```
{
    "status": {
        "success": false,
        "error": "<error message>"
    },
    "access_token": "<token>"
}
```
