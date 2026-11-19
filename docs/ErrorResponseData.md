# ErrorResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | [optional] 
**error** | **object** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.error_response_data import ErrorResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ErrorResponseData from a JSON string
error_response_data_instance = ErrorResponseData.from_json(json)
# print the JSON string representation of the object
print(ErrorResponseData.to_json())

# convert the object into a dict
error_response_data_dict = error_response_data_instance.to_dict()
# create an instance of ErrorResponseData from a dict
error_response_data_from_dict = ErrorResponseData.from_dict(error_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


