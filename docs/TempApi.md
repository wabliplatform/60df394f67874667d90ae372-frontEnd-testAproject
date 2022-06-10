# TempApi.TempApi

All URIs are relative to *http://83.212.100.226:3000/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createtemp**](TempApi.md#createtemp) | **POST** /temp | Creates the data
[**deletetemp**](TempApi.md#deletetemp) | **DELETE** /temp/{tempId} | Delete the element
[**getAlltemp**](TempApi.md#getAlltemp) | **GET** /temp/getAll | Get all the data
[**gettemp**](TempApi.md#gettemp) | **GET** /temp/{tempId} | Get the element
[**updatetemp**](TempApi.md#updatetemp) | **PUT** /temp/{tempId} | Updates the element



## createtemp

> Temp createtemp(temp)

Creates the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.TempApi();
let temp = new TempApi.Temp(); // Temp | data to be created
apiInstance.createtemp(temp, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **temp** | [**Temp**](Temp.md)| data to be created | 

### Return type

[**Temp**](Temp.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletetemp

> deletetemp(tempId)

Delete the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.TempApi();
let tempId = "tempId_example"; // String | the Id parameter
apiInstance.deletetemp(tempId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tempId** | **String**| the Id parameter | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getAlltemp

> [Temp] getAlltemp()

Get all the data

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.TempApi();
apiInstance.getAlltemp((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**[Temp]**](Temp.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## gettemp

> Temp gettemp(tempId)

Get the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.TempApi();
let tempId = "tempId_example"; // String | the Id parameter
apiInstance.gettemp(tempId, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tempId** | **String**| the Id parameter | 

### Return type

[**Temp**](Temp.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatetemp

> Temp updatetemp(tempId, opts)

Updates the element

### Example

```javascript
import TempApi from 'temp_api';

let apiInstance = new TempApi.TempApi();
let tempId = "tempId_example"; // String | the Id parameter
let opts = {
  'temp': new TempApi.Temp() // Temp | data to be updated
};
apiInstance.updatetemp(tempId, opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tempId** | **String**| the Id parameter | 
 **temp** | [**Temp**](Temp.md)| data to be updated | [optional] 

### Return type

[**Temp**](Temp.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

