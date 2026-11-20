# EwcAcceptance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**source_id** | **str** |  | [optional] 
**next_steps** | **str** |  | [optional] 
**next_date** | **datetime** |  | [optional] 
**outcome_reason** | **str** |  | [optional] 
**message_template** | [**MessageTemplate**](MessageTemplate.md) |  | 
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
from statflo_python_sdk.models.ewc_acceptance import EwcAcceptance

# TODO update the JSON string below
json = "{}"
# create an instance of EwcAcceptance from a JSON string
ewc_acceptance_instance = EwcAcceptance.from_json(json)
# print the JSON string representation of the object
print(EwcAcceptance.to_json())

# convert the object into a dict
ewc_acceptance_dict = ewc_acceptance_instance.to_dict()
# create an instance of EwcAcceptance from a dict
ewc_acceptance_from_dict = EwcAcceptance.from_dict(ewc_acceptance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


