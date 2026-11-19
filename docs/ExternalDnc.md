# ExternalDnc


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_to** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**message_content** | **str** |  | [optional] 
**source_id** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.external_dnc import ExternalDnc

# TODO update the JSON string below
json = "{}"
# create an instance of ExternalDnc from a JSON string
external_dnc_instance = ExternalDnc.from_json(json)
# print the JSON string representation of the object
print(ExternalDnc.to_json())

# convert the object into a dict
external_dnc_dict = external_dnc_instance.to_dict()
# create an instance of ExternalDnc from a dict
external_dnc_from_dict = ExternalDnc.from_dict(external_dnc_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


