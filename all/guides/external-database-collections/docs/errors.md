SortOrder: 2
# Errors

Each SPI call returns a response including an HTTP status code. If an error response is required, the response must include an error status code and a message that describes the type of error that occurred.

The error message should be in the following format:  
```JSON
{
  "message": "..."
}
```
Use the following HTTP Status/Error codes:

| HTTP Status Code | Description | 
| :-------------- | :------- |  
| 200 - OK | Success |
| 400 - Bad Request | One or more request parameters is wrong or missing |
| 401 - Unauthorized | The system was not able to authenticate the request |
| 404 - Not Found | Resource not found / does not exist |
| 409 - Conflict | The resource you are attempting to create already exists |


>Note
>
>4XX statuses will appear in the error produced by the Wix Data function call.