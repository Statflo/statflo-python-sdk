# DealerMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_metadata_update import DealerMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerMetadataUpdate from a JSON string
dealer_metadata_update_instance = DealerMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(DealerMetadataUpdate.to_json())

# convert the object into a dict
dealer_metadata_update_dict = dealer_metadata_update_instance.to_dict()
# create an instance of DealerMetadataUpdate from a dict
dealer_metadata_update_from_dict = DealerMetadataUpdate.from_dict(dealer_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


