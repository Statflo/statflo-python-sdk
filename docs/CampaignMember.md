# CampaignMember


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**account_id** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**campaign** | [**Campaign**](Campaign.md) |  | 
**campaign_id** | **int** |  | 
**start_date** | **datetime** |  | [optional] 
**end_date** | **datetime** |  | [optional] 
**secondary_dealer_id** | **str** |  | [optional] 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**campaign_nickname** | **str** |  | [optional] 
**source** | **str** |  | [optional] [default to 'api']
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
from statflo_python_sdk.models.campaign_member import CampaignMember

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMember from a JSON string
campaign_member_instance = CampaignMember.from_json(json)
# print the JSON string representation of the object
print(CampaignMember.to_json())

# convert the object into a dict
campaign_member_dict = campaign_member_instance.to_dict()
# create an instance of CampaignMember from a dict
campaign_member_from_dict = CampaignMember.from_dict(campaign_member_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


