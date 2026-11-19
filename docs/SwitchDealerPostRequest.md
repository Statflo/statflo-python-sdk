# SwitchDealerPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dealer_id** | **int** |  | [optional] 
**role_id** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.switch_dealer_post_request import SwitchDealerPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SwitchDealerPostRequest from a JSON string
switch_dealer_post_request_instance = SwitchDealerPostRequest.from_json(json)
# print the JSON string representation of the object
print(SwitchDealerPostRequest.to_json())

# convert the object into a dict
switch_dealer_post_request_dict = switch_dealer_post_request_instance.to_dict()
# create an instance of SwitchDealerPostRequest from a dict
switch_dealer_post_request_from_dict = SwitchDealerPostRequest.from_dict(switch_dealer_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


