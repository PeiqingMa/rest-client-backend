## RESTful API

### Send a request
Endpoint: `POST    /v1/request`  
Request body:
```json5
{
    "method": "GET",
    "url": "{{protocol}}://{{host}}/v1/test",
    "environment": "test",
    "headers": [{
        "key": "header1",
        "value": "something"
    }, {
        "key": "header2",
        "value": "something"
    }],
    "requestBody": "" // a string, encoded
}
```
Response body:
```json5
{
    "code": 200,
    "headers": [{
        "key": "header1",
        "value": "something"
    }, {
        "key": "header2",
        "value": "something"
    }],
    "responseBody": "" // a string, encoded
}
```

### Save a request

### Create/update an environment
Endpoint: `POST    /v1/env`  
Request body:
```json5
{
    "name": "test", // name should be unique
    "variable": [{
        "key": "header1",
        "value": "something"
    }, {
        "key": "header2",
        "value": "something"
    }]
}
```
Response body:
```json5
{
    "id": "abc123",
    "name": "test",
    "variable": [{
        "key": "header1",
        "value": "something"
    }, {
        "key": "header2",
        "value": "something"
    }]
}
```

### Create a folder

### Update a folder

### List all environments

### List all requests with folders

### Search requests (full text) 

### Delete an environment

### Delete a request

### Delete a folder
