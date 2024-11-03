# swagger_client.DefaultApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_cancel_job**](DefaultApi.md#delete_cancel_job) | **DELETE** /jobs/{id} | Cancel job
[**delete_clear_jobs**](DefaultApi.md#delete_clear_jobs) | **DELETE** /jobs | (ADMIN) Clear all jobs
[**delete_clear_scaling_rules**](DefaultApi.md#delete_clear_scaling_rules) | **DELETE** /scaling-rules | (ADMIN) Clear all scaling rules
[**delete_clear_users**](DefaultApi.md#delete_clear_users) | **DELETE** /users | (ADMIN) Clear all users
[**delete_delete_scaling_rule**](DefaultApi.md#delete_delete_scaling_rule) | **DELETE** /scaling-rules/{id} | Delete a scaling rule
[**get_get_job**](DefaultApi.md#get_get_job) | **GET** /jobs/{id} | Get a job
[**get_get_scaling_rule**](DefaultApi.md#get_get_scaling_rule) | **GET** /scaling-rules/{id} | Get a scaling rule
[**get_get_work**](DefaultApi.md#get_get_work) | **GET** /work | Get work
[**get_list_jobs**](DefaultApi.md#get_list_jobs) | **GET** /jobs | List jobs
[**get_list_scaling_rules**](DefaultApi.md#get_list_scaling_rules) | **GET** /scaling-rules | List all scaling rules
[**patch_update_scaling_rule**](DefaultApi.md#patch_update_scaling_rule) | **PATCH** /scaling-rules/{id} | Update an existing scaling rule
[**post_batch_create_jobs**](DefaultApi.md#post_batch_create_jobs) | **POST** /jobs/batch | Queue multiple jobs
[**post_create_job**](DefaultApi.md#post_create_job) | **POST** /jobs | Queue a new job
[**post_create_scaling_rule**](DefaultApi.md#post_create_scaling_rule) | **POST** /scaling-rules | Create a new scaling rule
[**post_create_token**](DefaultApi.md#post_create_token) | **POST** /users/{id}/token | (ADMIN) Create a new token
[**post_create_user**](DefaultApi.md#post_create_user) | **POST** /users | (ADMIN) Create a new user
[**post_job_heartbeat**](DefaultApi.md#post_job_heartbeat) | **POST** /jobs/{id}/heartbeat | Job heartbeat
[**post_report_job_completed**](DefaultApi.md#post_report_job_completed) | **POST** /jobs/{id}/completed | Report job completed
[**post_report_job_failure**](DefaultApi.md#post_report_job_failure) | **POST** /jobs/{id}/failed | Report job failure

# **delete_cancel_job**
> InlineResponse204 delete_cancel_job(id)

Cancel job

Cancel a job

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Job ID

try:
    # Cancel job
    api_response = api_instance.delete_cancel_job(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->delete_cancel_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Job ID | 

### Return type

[**InlineResponse204**](InlineResponse204.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_clear_jobs**
> InlineResponse204 delete_clear_jobs()

(ADMIN) Clear all jobs

Clear all jobs

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))

try:
    # (ADMIN) Clear all jobs
    api_response = api_instance.delete_clear_jobs()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->delete_clear_jobs: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse204**](InlineResponse204.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_clear_scaling_rules**
> delete_clear_scaling_rules()

(ADMIN) Clear all scaling rules

Clear all scaling rules

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))

try:
    # (ADMIN) Clear all scaling rules
    api_instance.delete_clear_scaling_rules()
except ApiException as e:
    print("Exception when calling DefaultApi->delete_clear_scaling_rules: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_clear_users**
> delete_clear_users()

(ADMIN) Clear all users

Clear all users

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))

try:
    # (ADMIN) Clear all users
    api_instance.delete_clear_users()
except ApiException as e:
    print("Exception when calling DefaultApi->delete_clear_users: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_delete_scaling_rule**
> delete_delete_scaling_rule(id)

Delete a scaling rule

Delete a scaling rule

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Container Group ID

try:
    # Delete a scaling rule
    api_instance.delete_delete_scaling_rule(id)
except ApiException as e:
    print("Exception when calling DefaultApi->delete_delete_scaling_rule: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Container Group ID | 

### Return type

void (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_get_job**
> InlineResponse202 get_get_job(id)

Get a job

Get a job by ID

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Job ID

try:
    # Get a job
    api_response = api_instance.get_get_job(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_get_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Job ID | 

### Return type

[**InlineResponse202**](InlineResponse202.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_get_scaling_rule**
> InlineResponse201 get_get_scaling_rule(id)

Get a scaling rule

Get a scaling rule

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Container Group ID

try:
    # Get a scaling rule
    api_response = api_instance.get_get_scaling_rule(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_get_scaling_rule: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Container Group ID | 

### Return type

[**InlineResponse201**](InlineResponse201.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_get_work**
> object get_get_work(machine_id, container_group_id)

Get work

Get a job to work on

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
machine_id = NULL # object | Machine ID
container_group_id = NULL # object | Container Group ID

try:
    # Get work
    api_response = api_instance.get_get_work(machine_id, container_group_id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_get_work: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **machine_id** | [**object**](.md)| Machine ID | 
 **container_group_id** | [**object**](.md)| Container Group ID | 

### Return type

**object**

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_list_jobs**
> InlineResponse200 get_list_jobs(status=status, container_group_id=container_group_id, page_size=page_size, page=page, asc=asc)

List jobs

List your jobs

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
status = NULL # object | Job status (optional)
container_group_id = NULL # object | Container Group ID (optional)
page_size = NULL # object | Page size (optional)
page = NULL # object | Page number (optional)
asc = NULL # object | Sort ascending (optional)

try:
    # List jobs
    api_response = api_instance.get_list_jobs(status=status, container_group_id=container_group_id, page_size=page_size, page=page, asc=asc)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_list_jobs: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | [**object**](.md)| Job status | [optional] 
 **container_group_id** | [**object**](.md)| Container Group ID | [optional] 
 **page_size** | [**object**](.md)| Page size | [optional] 
 **page** | [**object**](.md)| Page number | [optional] 
 **asc** | [**object**](.md)| Sort ascending | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_list_scaling_rules**
> InlineResponse2002 get_list_scaling_rules()

List all scaling rules

List all scaling rules

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))

try:
    # List all scaling rules
    api_response = api_instance.get_list_scaling_rules()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->get_list_scaling_rules: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_update_scaling_rule**
> InlineResponse201 patch_update_scaling_rule(id, body=body)

Update an existing scaling rule

Update an existing scaling rule

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Container Group ID
body = swagger_client.ScalingrulesIdBody() # ScalingrulesIdBody |  (optional)

try:
    # Update an existing scaling rule
    api_response = api_instance.patch_update_scaling_rule(id, body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->patch_update_scaling_rule: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Container Group ID | 
 **body** | [**ScalingrulesIdBody**](ScalingrulesIdBody.md)|  | [optional] 

### Return type

[**InlineResponse201**](InlineResponse201.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_batch_create_jobs**
> object post_batch_create_jobs(body=body)

Queue multiple jobs

Queue multiple jobs in one request. Limit 1000 jobs per request.   Queue a new job to be executed by the specified container group. [Get your Container Group ID](https://docs.salad.com/reference/get_container_group)  Note that although we use the term \"AWS S3 bucket\" in the documentation, you can use any S3-compatible storage provider. In particular, we recommend choosing a provider with no egress fees, such as [Cloudflare R2.](https://www.cloudflare.com/developer-platform/r2/)  You must use either the `sync` object or the `input_bucket`, `input_prefix`, `checkpoint_bucket`, `checkpoint_prefix`, `output_bucket`, and `output_prefix` fields. You may not use both.  **Body**  | Key                 | Type     | Description        | Default | |---------------------|----------|--------------------|---------| | `command`           | string   | The command to execute. | **required** | | `arguments`         | array    | List of arguments for the command. | [] | | `environment`       | object   | Key-value pairs defining the environment variables. | {} | | `input_bucket`      | string   | Name of the AWS S3 bucket for input files. | *optional* | | `input_prefix`      | string   | Prefix for input files in the S3 bucket. | *optional* | | `checkpoint_bucket` | string   | Name of the AWS S3 bucket for checkpoint files. | *optional* | | `checkpoint_prefix` | string   | Prefix for checkpoint files in the S3 bucket. | *optional* | | `output_bucket`     | string   | Name of the AWS S3 bucket for output files. | *optional* | | `output_prefix`     | string   | Prefix for output files in the S3 bucket. | *optional* | | `max_failures`      | integer  | Maximum number of allowed failures before the job is marked failed. | 3 | | `heartbeat_interval`| integer | Time interval (in seconds) for sending heartbeat signals. | 30 | | `webhook`           | string   | URL for the webhook to notify upon completion or failure. | *optional* | | `container_group_id`| string  | ID of the container group where the command will be executed. | **required** | | `compression` | boolean | If true, will gzip files it uploads to the bucket, appending the filename with .gz | false | | `sync` | object | Sync configuration for the job. | *optional* |  **body.sync**  | Key      | Type   | Description | Default | |----------|--------|-------------|---------| | `before` | SyncConfig[] | List of sync configurations to run before the job. | *optional* | | `during` | SyncConfig[] | List of sync configurations to run during the job. | *optional* | | `after`  | SyncConfig[] | List of sync configurations to run after the job, but before marking the job complete. | *optional* |  **SyncConfig**  | Key          | Type   | Description | Default | |--------------|--------|-------------|---------| | `bucket`     | string | Name of the AWS S3 bucket. | **required** | | `prefix`     | string | Prefix for files in the S3 bucket. | **required** | | `local_path` | string | Local path to sync files to/from. | **required** | | `direction`  | string | Direction of the sync. Must be \"download\" for `before`, and \"upload\" for `during` and `after` | **required** | | `pattern`    | string | An ECMAScript(javascript) Regular Expression. Filepaths/keys that match will be included in the sync. Default is to include all files. | *optional* | 

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
body = NULL # object |  (optional)

try:
    # Queue multiple jobs
    api_response = api_instance.post_batch_create_jobs(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_batch_create_jobs: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**object**](object.md)|  | [optional] 

### Return type

**object**

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_create_job**
> InlineResponse202 post_create_job(body=body)

Queue a new job

 Queue a new job to be executed by the specified container group. [Get your Container Group ID](https://docs.salad.com/reference/get_container_group)  Note that although we use the term \"AWS S3 bucket\" in the documentation, you can use any S3-compatible storage provider. In particular, we recommend choosing a provider with no egress fees, such as [Cloudflare R2.](https://www.cloudflare.com/developer-platform/r2/)  You must use either the `sync` object or the `input_bucket`, `input_prefix`, `checkpoint_bucket`, `checkpoint_prefix`, `output_bucket`, and `output_prefix` fields. You may not use both.  **Body**  | Key                 | Type     | Description        | Default | |---------------------|----------|--------------------|---------| | `command`           | string   | The command to execute. | **required** | | `arguments`         | array    | List of arguments for the command. | [] | | `environment`       | object   | Key-value pairs defining the environment variables. | {} | | `input_bucket`      | string   | Name of the AWS S3 bucket for input files. | *optional* | | `input_prefix`      | string   | Prefix for input files in the S3 bucket. | *optional* | | `checkpoint_bucket` | string   | Name of the AWS S3 bucket for checkpoint files. | *optional* | | `checkpoint_prefix` | string   | Prefix for checkpoint files in the S3 bucket. | *optional* | | `output_bucket`     | string   | Name of the AWS S3 bucket for output files. | *optional* | | `output_prefix`     | string   | Prefix for output files in the S3 bucket. | *optional* | | `max_failures`      | integer  | Maximum number of allowed failures before the job is marked failed. | 3 | | `heartbeat_interval`| integer | Time interval (in seconds) for sending heartbeat signals. | 30 | | `webhook`           | string   | URL for the webhook to notify upon completion or failure. | *optional* | | `container_group_id`| string  | ID of the container group where the command will be executed. | **required** | | `compression` | boolean | If true, will gzip files it uploads to the bucket, appending the filename with .gz | false | | `sync` | object | Sync configuration for the job. | *optional* |  **body.sync**  | Key      | Type   | Description | Default | |----------|--------|-------------|---------| | `before` | SyncConfig[] | List of sync configurations to run before the job. | *optional* | | `during` | SyncConfig[] | List of sync configurations to run during the job. | *optional* | | `after`  | SyncConfig[] | List of sync configurations to run after the job, but before marking the job complete. | *optional* |  **SyncConfig**  | Key          | Type   | Description | Default | |--------------|--------|-------------|---------| | `bucket`     | string | Name of the AWS S3 bucket. | **required** | | `prefix`     | string | Prefix for files in the S3 bucket. | **required** | | `local_path` | string | Local path to sync files to/from. | **required** | | `direction`  | string | Direction of the sync. Must be \"download\" for `before`, and \"upload\" for `during` and `after` | **required** | | `pattern`    | string | An ECMAScript(javascript) Regular Expression. Filepaths/keys that match will be included in the sync. Default is to include all files. | *optional* | 

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
body = swagger_client.JobsBody() # JobsBody |  (optional)

try:
    # Queue a new job
    api_response = api_instance.post_create_job(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_create_job: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**JobsBody**](JobsBody.md)|  | [optional] 

### Return type

[**InlineResponse202**](InlineResponse202.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_create_scaling_rule**
> InlineResponse201 post_create_scaling_rule(body=body)

Create a new scaling rule

Create a new scaling rule

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
body = swagger_client.ScalingrulesBody() # ScalingrulesBody |  (optional)

try:
    # Create a new scaling rule
    api_response = api_instance.post_create_scaling_rule(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_create_scaling_rule: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**ScalingrulesBody**](ScalingrulesBody.md)|  | [optional] 

### Return type

[**InlineResponse201**](InlineResponse201.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_create_token**
> InlineResponse2012 post_create_token(id, body=body)

(ADMIN) Create a new token

Create a new token

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | User ID
body = swagger_client.IdTokenBody() # IdTokenBody |  (optional)

try:
    # (ADMIN) Create a new token
    api_response = api_instance.post_create_token(id, body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_create_token: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| User ID | 
 **body** | [**IdTokenBody**](IdTokenBody.md)|  | [optional] 

### Return type

[**InlineResponse2012**](InlineResponse2012.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_create_user**
> InlineResponse2011 post_create_user(body=body)

(ADMIN) Create a new user

Create a new user

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
body = swagger_client.UsersBody() # UsersBody |  (optional)

try:
    # (ADMIN) Create a new user
    api_response = api_instance.post_create_user(body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_create_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UsersBody**](UsersBody.md)|  | [optional] 

### Return type

[**InlineResponse2011**](InlineResponse2011.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_job_heartbeat**
> InlineResponse2001 post_job_heartbeat(id, body=body)

Job heartbeat

Update the heartbeat for a job

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Job ID
body = swagger_client.IdHeartbeatBody() # IdHeartbeatBody |  (optional)

try:
    # Job heartbeat
    api_response = api_instance.post_job_heartbeat(id, body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_job_heartbeat: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Job ID | 
 **body** | [**IdHeartbeatBody**](IdHeartbeatBody.md)|  | [optional] 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_report_job_completed**
> InlineResponse204 post_report_job_completed(id, body=body)

Report job completed

Report a job completed

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Job ID
body = swagger_client.IdCompletedBody() # IdCompletedBody |  (optional)

try:
    # Report job completed
    api_response = api_instance.post_report_job_completed(id, body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_report_job_completed: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Job ID | 
 **body** | [**IdCompletedBody**](IdCompletedBody.md)|  | [optional] 

### Return type

[**InlineResponse204**](InlineResponse204.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_report_job_failure**
> InlineResponse204 post_report_job_failure(id, body=body)

Report job failure

Report a job failure

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: apiKey
configuration = swagger_client.Configuration()
configuration.api_key['X-Kelpie-Key'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-Kelpie-Key'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.DefaultApi(swagger_client.ApiClient(configuration))
id = NULL # object | Job ID
body = swagger_client.IdFailedBody() # IdFailedBody |  (optional)

try:
    # Report job failure
    api_response = api_instance.post_report_job_failure(id, body=body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DefaultApi->post_report_job_failure: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**object**](.md)| Job ID | 
 **body** | [**IdFailedBody**](IdFailedBody.md)|  | [optional] 

### Return type

[**InlineResponse204**](InlineResponse204.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

