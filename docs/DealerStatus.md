# DealerStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | [optional] 
**translation** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_status import DealerStatus

# TODO update the JSON string below
json = "{}"
# create an instance of DealerStatus from a JSON string
dealer_status_instance = DealerStatus.from_json(json)
# print the JSON string representation of the object
print(DealerStatus.to_json())

# convert the object into a dict
dealer_status_dict = dealer_status_instance.to_dict()
# create an instance of DealerStatus from a dict
dealer_status_from_dict = DealerStatus.from_dict(dealer_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


