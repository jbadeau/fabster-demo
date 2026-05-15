# DefaultApi

All URIs are relative to *http://localhost:3000*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**todosGet**](DefaultApi.md#todosget) | **GET** /todos | List all todos |
| [**todosIdDelete**](DefaultApi.md#todosiddelete) | **DELETE** /todos/{id} | Delete a todo |
| [**todosIdPut**](DefaultApi.md#todosidputoperation) | **PUT** /todos/{id} | Update a todo |
| [**todosPost**](DefaultApi.md#todospostoperation) | **POST** /todos | Create a todo |



## todosGet

> Array&lt;Todo&gt; todosGet()

List all todos

### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '';
import type { TodosGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new DefaultApi();

  try {
    const data = await api.todosGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Array&lt;Todo&gt;**](Todo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Todo list |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## todosIdDelete

> todosIdDelete(id)

Delete a todo

### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '';
import type { TodosIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new DefaultApi();

  const body = {
    // string
    id: id_example,
  } satisfies TodosIdDeleteRequest;

  try {
    const data = await api.todosIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Todo deleted |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## todosIdPut

> Todo todosIdPut(id, todosIdPutRequest)

Update a todo

### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '';
import type { TodosIdPutOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new DefaultApi();

  const body = {
    // string
    id: id_example,
    // TodosIdPutRequest
    todosIdPutRequest: ...,
  } satisfies TodosIdPutOperationRequest;

  try {
    const data = await api.todosIdPut(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |
| **todosIdPutRequest** | [TodosIdPutRequest](TodosIdPutRequest.md) |  | |

### Return type

[**Todo**](Todo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Updated todo |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## todosPost

> Todo todosPost(todosPostRequest)

Create a todo

### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '';
import type { TodosPostOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new DefaultApi();

  const body = {
    // TodosPostRequest
    todosPostRequest: ...,
  } satisfies TodosPostOperationRequest;

  try {
    const data = await api.todosPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **todosPostRequest** | [TodosPostRequest](TodosPostRequest.md) |  | |

### Return type

[**Todo**](Todo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Created todo |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

