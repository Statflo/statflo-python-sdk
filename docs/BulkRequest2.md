# BulkRequest2


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**requests** | [**List[BulkSubRequest]**](BulkSubRequest.md) |  | [optional] [default to []]

## Example

```python
from statflo_python_sdk.models.bulk_request2 import BulkRequest2

# TODO update the JSON string below
json = "{}"
# create an instance of BulkRequest2 from a JSON string
bulk_request2_instance = BulkRequest2.from_json(json)
# print the JSON string representation of the object
print(BulkRequest2.to_json())

# convert the object into a dict
bulk_request2_dict = bulk_request2_instance.to_dict()
# create an instance of BulkRequest2 from a dict
bulk_request2_from_dict = BulkRequest2.from_dict(bulk_request2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


