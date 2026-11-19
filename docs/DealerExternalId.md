# DealerExternalId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_external_id import DealerExternalId

# TODO update the JSON string below
json = "{}"
# create an instance of DealerExternalId from a JSON string
dealer_external_id_instance = DealerExternalId.from_json(json)
# print the JSON string representation of the object
print(DealerExternalId.to_json())

# convert the object into a dict
dealer_external_id_dict = dealer_external_id_instance.to_dict()
# create an instance of DealerExternalId from a dict
dealer_external_id_from_dict = DealerExternalId.from_dict(dealer_external_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


