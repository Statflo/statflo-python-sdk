# DealerExternalIdUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] 
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_external_id_update import DealerExternalIdUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerExternalIdUpdate from a JSON string
dealer_external_id_update_instance = DealerExternalIdUpdate.from_json(json)
# print the JSON string representation of the object
print(DealerExternalIdUpdate.to_json())

# convert the object into a dict
dealer_external_id_update_dict = dealer_external_id_update_instance.to_dict()
# create an instance of DealerExternalIdUpdate from a dict
dealer_external_id_update_from_dict = DealerExternalIdUpdate.from_dict(dealer_external_id_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


