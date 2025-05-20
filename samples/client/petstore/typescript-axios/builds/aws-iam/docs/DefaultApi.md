# DefaultApi

All URIs are relative to *https://abc123.execute-api.us-east-1.amazonaws.com/prod*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getInventory**](#getinventory) | **GET** /store/inventory | Returns pet inventories by status|
|[**getPetById**](#getpetbyid) | **GET** /pet | Find pet by ID|

# **getInventory**
> { [key: string]: number; } getInventory()


### Example

```typescript
import {
    DefaultApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.getInventory();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**{ [key: string]: number; }**

### Authorization

[sigv4_auth](../README.md#sigv4_auth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getPetById**
> Pet getPetById()


### Example

```typescript
import {
    DefaultApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DefaultApi(configuration);

const { status, data } = await apiInstance.getPetById();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Pet**

### Authorization

[aws_iam](../README.md#aws_iam)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | successful operation |  -  |
|**404** | Pet not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

