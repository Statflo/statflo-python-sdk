# CampaignActionUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**campaign_name** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_action_update import CampaignActionUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignActionUpdate from a JSON string
campaign_action_update_instance = CampaignActionUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignActionUpdate.to_json())

# convert the object into a dict
campaign_action_update_dict = campaign_action_update_instance.to_dict()
# create an instance of CampaignActionUpdate from a dict
campaign_action_update_from_dict = CampaignActionUpdate.from_dict(campaign_action_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


