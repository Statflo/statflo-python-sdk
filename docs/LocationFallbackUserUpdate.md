# LocationFallbackUserUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_fallback_user_update import LocationFallbackUserUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationFallbackUserUpdate from a JSON string
location_fallback_user_update_instance = LocationFallbackUserUpdate.from_json(json)
# print the JSON string representation of the object
print(LocationFallbackUserUpdate.to_json())

# convert the object into a dict
location_fallback_user_update_dict = location_fallback_user_update_instance.to_dict()
# create an instance of LocationFallbackUserUpdate from a dict
location_fallback_user_update_from_dict = LocationFallbackUserUpdate.from_dict(location_fallback_user_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


