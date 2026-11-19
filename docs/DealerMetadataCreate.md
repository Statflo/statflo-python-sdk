# DealerMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_metadata_create import DealerMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerMetadataCreate from a JSON string
dealer_metadata_create_instance = DealerMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(DealerMetadataCreate.to_json())

# convert the object into a dict
dealer_metadata_create_dict = dealer_metadata_create_instance.to_dict()
# create an instance of DealerMetadataCreate from a dict
dealer_metadata_create_from_dict = DealerMetadataCreate.from_dict(dealer_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


