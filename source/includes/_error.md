# Errors
```
401 Unauthorized
```
```
{
  "error": {
    "code": "GEN-UNAUTHORIZED",
    "message": "You don't have enough privileges to perform this action."
  }
}
```

Biz Airlines uses standard HTTP status codes to communicate errors

|         |   |
|---------|---|
| **200** | OK - Everything went as planned. |
| **400** | Bad Request - Something in your header or request body was malformed. |
| **401** | Unauthorized - Necessary credentials were either missing or invalid. |
| **403** | Forbidden - Your credentials are valid but you don't have access to the requested resource. |
| **404** | Not Found - The requested object doesn't exist. |
| **500+** | Server Errors - Something went wrong on our end. |

In addition to the status code, the HTTP body of the response will also contain a JSON representation of the error.
