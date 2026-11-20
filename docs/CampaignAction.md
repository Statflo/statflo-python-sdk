# CampaignAction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**campaign_name** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
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
from statflo_python_sdk.models.campaign_action import CampaignAction

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignAction from a JSON string
campaign_action_instance = CampaignAction.from_json(json)
# print the JSON string representation of the object
print(CampaignAction.to_json())

# convert the object into a dict
campaign_action_dict = campaign_action_instance.to_dict()
# create an instance of CampaignAction from a dict
campaign_action_from_dict = CampaignAction.from_dict(campaign_action_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


