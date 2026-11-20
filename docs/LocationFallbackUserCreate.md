# LocationFallbackUserCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location_id** | **int** |  | 
**user_id** | **int** |  | 

## Example

```python
from statflo_python_sdk.models.location_fallback_user_create import LocationFallbackUserCreate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationFallbackUserCreate from a JSON string
location_fallback_user_create_instance = LocationFallbackUserCreate.from_json(json)
# print the JSON string representation of the object
print(LocationFallbackUserCreate.to_json())

# convert the object into a dict
location_fallback_user_create_dict = location_fallback_user_create_instance.to_dict()
# create an instance of LocationFallbackUserCreate from a dict
location_fallback_user_create_from_dict = LocationFallbackUserCreate.from_dict(location_fallback_user_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


