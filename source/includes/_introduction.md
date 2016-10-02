# Introduction
## Basics
The Biz Airlines API is designed according to [REST](https://en.wikipedia.org/wiki/Representational_state_transfer) principles.

The API accepts JSON in request bodies and requires that the `content-type: application/json` header be specified for all such requests. The API will always respond with a JSON object. Depending on context, resources may return single objects or arrays of objects, nested within the response object.

## Authentication
```
HTTP Example
```
```
POST /v1/me HTTP/1.1
Host: api.bizairlines.com
Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.eyJpc3MiOiJodHRwOlwvXC9hcGkuYml6YWlybGluZXMuY29tXC8iLCJhdWQiOiJodHRwOlwvXC9hcGkuYml6YWlybGluZXMuY29tXC8iLCJpYXQiOjE0NzA0ODkyNzMsIm5iZiI6MTQ3MDQ4OTI3MywiZXhwIjoxNzg2MDIyMDczLCJpZCI6MX0.jlWjsSKMPt1krq86VtYPDzc5tKcn68yVT2fAhoxCBfVjA_NHc3uOVeAXN1MiVcaUU0wIzOdFP8hDz9zcWcgBkA
Content-Type: application/json
```

Biz Airlines uses [JWT](https://jwt.io/) to generate it's API authentication tokens. Some endpoints requires token and it must be sent inside the HTTP Authorization header and the token should be prepended with `Bearer `.
