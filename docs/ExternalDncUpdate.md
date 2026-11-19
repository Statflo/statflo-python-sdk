# ExternalDncUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_to** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**message_content** | **str** |  | [optional] 
**source_id** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.external_dnc_update import ExternalDncUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ExternalDncUpdate from a JSON string
external_dnc_update_instance = ExternalDncUpdate.from_json(json)
# print the JSON string representation of the object
print(ExternalDncUpdate.to_json())

# convert the object into a dict
external_dnc_update_dict = external_dnc_update_instance.to_dict()
# create an instance of ExternalDncUpdate from a dict
external_dnc_update_from_dict = ExternalDncUpdate.from_dict(external_dnc_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


