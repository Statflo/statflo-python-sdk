# DealerExternalIdCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_external_id_create import DealerExternalIdCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerExternalIdCreate from a JSON string
dealer_external_id_create_instance = DealerExternalIdCreate.from_json(json)
# print the JSON string representation of the object
print(DealerExternalIdCreate.to_json())

# convert the object into a dict
dealer_external_id_create_dict = dealer_external_id_create_instance.to_dict()
# create an instance of DealerExternalIdCreate from a dict
dealer_external_id_create_from_dict = DealerExternalIdCreate.from_dict(dealer_external_id_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


