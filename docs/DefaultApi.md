# royal_mail_address_codegen.DefaultApi

All URIs are relative to *https://api.royalmail.net/addressfind/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**address_find**](DefaultApi.md#address_find) | **POST** /address | To find address summary with unique address id.
[**address_retrieve**](DefaultApi.md#address_retrieve) | **GET** /address/{addressId} | To retrieve complete details for an address.
[**address_verify**](DefaultApi.md#address_verify) | **POST** /address/dps | To find matching addresses with DPS, AQI and AVC.


# **address_find**
> AddressesDef address_find(x_rmg_date_time, address_find_request, x_rmg_language=x_rmg_language, accept=accept)

To find address summary with unique address id.

To find address summary with unique address id.

### Example

* Api Key Authentication (Client-Id):
* Api Key Authentication (Client-Secret):

```python
import royal_mail_address_codegen
from royal_mail_address_codegen.models.address_find_request_def import AddressFindRequestDef
from royal_mail_address_codegen.models.addresses_def import AddressesDef
from royal_mail_address_codegen.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.royalmail.net/addressfind/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = royal_mail_address_codegen.Configuration(
    host = "https://api.royalmail.net/addressfind/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Client-Id
configuration.api_key['Client-Id'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Id'] = 'Bearer'

# Configure API key authorization: Client-Secret
configuration.api_key['Client-Secret'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Secret'] = 'Bearer'

# Enter a context with an instance of the API client
with royal_mail_address_codegen.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = royal_mail_address_codegen.DefaultApi(api_client)
    x_rmg_date_time = '2013-10-20' # date | This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00
    address_find_request = royal_mail_address_codegen.AddressFindRequestDef() # AddressFindRequestDef | 
    x_rmg_language = 'x_rmg_language_example' # str | Optional default english (optional)
    accept = 'accept_example' # str | Pass though; used for markdown (optional)

    try:
        # To find address summary with unique address id.
        api_response = api_instance.address_find(x_rmg_date_time, address_find_request, x_rmg_language=x_rmg_language, accept=accept)
        print("The response of DefaultApi->address_find:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->address_find: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_rmg_date_time** | **date**| This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00 | 
 **address_find_request** | [**AddressFindRequestDef**](AddressFindRequestDef.md)|  | 
 **x_rmg_language** | **str**| Optional default english | [optional] 
 **accept** | **str**| Pass though; used for markdown | [optional] 

### Return type

[**AddressesDef**](AddressesDef.md)

### Authorization

[Client-Id](../README.md#Client-Id), [Client-Secret](../README.md#Client-Secret)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | detailed information about given collection. |  -  |
**400** | Bad Request. A malformed request has been received. |  -  |
**401** | Unauthorized. |  -  |
**404** | Not Found. |  -  |
**405** | Method Not Allowed. |  -  |
**500** | An unexpected error has occurred. |  -  |
**503** | Service Unavailable.  The API is currently unavailable. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **address_retrieve**
> AddressRecordDef address_retrieve(address_id, x_rmg_date_time, x_rmg_language=x_rmg_language, accept=accept)

To retrieve complete details for an address.

To retrieve complete details for an address.

### Example

* Api Key Authentication (Client-Id):
* Api Key Authentication (Client-Secret):

```python
import royal_mail_address_codegen
from royal_mail_address_codegen.models.address_record_def import AddressRecordDef
from royal_mail_address_codegen.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.royalmail.net/addressfind/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = royal_mail_address_codegen.Configuration(
    host = "https://api.royalmail.net/addressfind/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Client-Id
configuration.api_key['Client-Id'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Id'] = 'Bearer'

# Configure API key authorization: Client-Secret
configuration.api_key['Client-Secret'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Secret'] = 'Bearer'

# Enter a context with an instance of the API client
with royal_mail_address_codegen.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = royal_mail_address_codegen.DefaultApi(api_client)
    address_id = 'address_id_example' # str | Unique identifier for address record retrieval
    x_rmg_date_time = '2013-10-20' # date | This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00
    x_rmg_language = 'x_rmg_language_example' # str | Optional default english (optional)
    accept = 'accept_example' # str | Pass though; used for markdown (optional)

    try:
        # To retrieve complete details for an address.
        api_response = api_instance.address_retrieve(address_id, x_rmg_date_time, x_rmg_language=x_rmg_language, accept=accept)
        print("The response of DefaultApi->address_retrieve:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->address_retrieve: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address_id** | **str**| Unique identifier for address record retrieval | 
 **x_rmg_date_time** | **date**| This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00 | 
 **x_rmg_language** | **str**| Optional default english | [optional] 
 **accept** | **str**| Pass though; used for markdown | [optional] 

### Return type

[**AddressRecordDef**](AddressRecordDef.md)

### Authorization

[Client-Id](../README.md#Client-Id), [Client-Secret](../README.md#Client-Secret)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | detailed information about given collection. |  -  |
**400** | Bad Request. A malformed request has been received. |  -  |
**401** | Unauthorized. |  -  |
**404** | Not Found. |  -  |
**405** | Method Not Allowed. |  -  |
**500** | An unexpected error has occurred. |  -  |
**503** | Service Unavailable.  The API is currently unavailable. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **address_verify**
> List[AddressVerifyReqRespdef] address_verify(x_rmg_date_time, address_find_request, x_rmg_language=x_rmg_language, accept=accept)

To find matching addresses with DPS, AQI and AVC.

To find matching addresses with DPS, AQI and AVC.

### Example

* Api Key Authentication (Client-Id):
* Api Key Authentication (Client-Secret):

```python
import royal_mail_address_codegen
from royal_mail_address_codegen.models.address_verify_req_respdef import AddressVerifyReqRespdef
from royal_mail_address_codegen.models.address_verify_request_def import AddressVerifyRequestDef
from royal_mail_address_codegen.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.royalmail.net/addressfind/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = royal_mail_address_codegen.Configuration(
    host = "https://api.royalmail.net/addressfind/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: Client-Id
configuration.api_key['Client-Id'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Id'] = 'Bearer'

# Configure API key authorization: Client-Secret
configuration.api_key['Client-Secret'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Client-Secret'] = 'Bearer'

# Enter a context with an instance of the API client
with royal_mail_address_codegen.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = royal_mail_address_codegen.DefaultApi(api_client)
    x_rmg_date_time = '2013-10-20' # date | This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00
    address_find_request = royal_mail_address_codegen.AddressVerifyRequestDef() # AddressVerifyRequestDef | 
    x_rmg_language = 'x_rmg_language_example' # str | Optional default english (optional)
    accept = 'accept_example' # str | Pass though; used for markdown (optional)

    try:
        # To find matching addresses with DPS, AQI and AVC.
        api_response = api_instance.address_verify(x_rmg_date_time, address_find_request, x_rmg_language=x_rmg_language, accept=accept)
        print("The response of DefaultApi->address_verify:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->address_verify: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_rmg_date_time** | **date**| This should be populated with the date time in ISO 8601 subset format below when the message was generated. Eg. 2016-10-20T10:04:00+01:00 | 
 **address_find_request** | [**AddressVerifyRequestDef**](AddressVerifyRequestDef.md)|  | 
 **x_rmg_language** | **str**| Optional default english | [optional] 
 **accept** | **str**| Pass though; used for markdown | [optional] 

### Return type

[**List[AddressVerifyReqRespdef]**](AddressVerifyReqRespdef.md)

### Authorization

[Client-Id](../README.md#Client-Id), [Client-Secret](../README.md#Client-Secret)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | detailed information about given collection. |  -  |
**400** | Bad Request. A malformed request has been received. |  -  |
**401** | Unauthorized. |  -  |
**404** | Not Found. |  -  |
**405** | Method Not Allowed. |  -  |
**500** | An unexpected error has occurred. |  -  |
**503** | Service Unavailable.  The API is currently unavailable. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

