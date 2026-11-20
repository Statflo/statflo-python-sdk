# CampaignMemberUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**account_id** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**campaign_id** | **int** |  | 
**start_date** | **datetime** |  | [optional] 
**end_date** | **datetime** |  | [optional] 
**secondary_dealer_id** | **str** |  | [optional] 
**campaign_nickname** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**date_created** | **datetime** |  | 
**exclude_dnc** | **str** |  | [optional] 
**exclude_dnc_date** | **datetime** |  | [optional] 
**exclude_kill** | **str** |  | [optional] 
**exclude_duplicate** | **str** |  | [optional] 
**exclude_terminated** | **str** |  | [optional] 
**exclude_terminated_date** | **datetime** |  | [optional] 
**exclude_prepaid** | **str** |  | [optional] 
**exclude_no_dealer_match** | **str** |  | [optional] 
**exclude_archived** | **str** |  | [optional] 
**exclude_legacy** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_member_update import CampaignMemberUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMemberUpdate from a JSON string
campaign_member_update_instance = CampaignMemberUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignMemberUpdate.to_json())

# convert the object into a dict
campaign_member_update_dict = campaign_member_update_instance.to_dict()
# create an instance of CampaignMemberUpdate from a dict
campaign_member_update_from_dict = CampaignMemberUpdate.from_dict(campaign_member_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


