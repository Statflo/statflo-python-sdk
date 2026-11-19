# DealerMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_metadata import DealerMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of DealerMetadata from a JSON string
dealer_metadata_instance = DealerMetadata.from_json(json)
# print the JSON string representation of the object
print(DealerMetadata.to_json())

# convert the object into a dict
dealer_metadata_dict = dealer_metadata_instance.to_dict()
# create an instance of DealerMetadata from a dict
dealer_metadata_from_dict = DealerMetadata.from_dict(dealer_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


