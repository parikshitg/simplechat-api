# SimpleChat API Specification

## Structures

### Struct Status
```
{
    "success": bool,
    "error": string,
}
```

### Struct UserProfile
```
{
    "id": string,
    "name": string,
    "email:" string
    "photo": string,
} 
```


# API

## 1. Register

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
    "status": Status,
    "auth_token": "<token>"
}
    
```


## 2. Login

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
    "status": Status,
    "access_token": "<token>"
}
```

## 3. Profile

Endpoint ```/profile```

### ProfileRequest
```
{
    "access_token": "<token">,
    "id": "<profile id>"
}
```

### ProfileResponse
```
{
    "status": Status,
    "profile": UserProfile,
}
```


