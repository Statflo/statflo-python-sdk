# BulkSubRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**uri** | **str** |  | 
**method** | **str** |  | [optional] [default to 'GET']
**parameters** | **List[object]** |  | 
**headers** | **List[object]** |  | 

## Example

```python
from statflo_python_sdk.models.bulk_sub_request import BulkSubRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BulkSubRequest from a JSON string
bulk_sub_request_instance = BulkSubRequest.from_json(json)
# print the JSON string representation of the object
print(BulkSubRequest.to_json())

# convert the object into a dict
bulk_sub_request_dict = bulk_sub_request_instance.to_dict()
# create an instance of BulkSubRequest from a dict
bulk_sub_request_from_dict = BulkSubRequest.from_dict(bulk_sub_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


