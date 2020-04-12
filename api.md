# API Specification
===================

## 1 Register

Endpoint ```	/register```

### RegisterRequest

```
{
	"email": "<email address>"
}
	
```

### RegisterResponse
```
{
	"status": "<status>",
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
	"status": "<status>",
	"access_token": "<token>"
}
```