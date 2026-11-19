# LocationFallbackUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**location** | [**Location**](Location.md) |  | 
**user** | [**User**](User.md) |  | 

## Example

```python
from statflo_python_sdk.models.location_fallback_user import LocationFallbackUser

# TODO update the JSON string below
json = "{}"
# create an instance of LocationFallbackUser from a JSON string
location_fallback_user_instance = LocationFallbackUser.from_json(json)
# print the JSON string representation of the object
print(LocationFallbackUser.to_json())

# convert the object into a dict
location_fallback_user_dict = location_fallback_user_instance.to_dict()
# create an instance of LocationFallbackUser from a dict
location_fallback_user_from_dict = LocationFallbackUser.from_dict(location_fallback_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


