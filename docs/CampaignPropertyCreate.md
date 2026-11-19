# CampaignPropertyCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**campaign_id** | **int** |  | 
**campaign_priority** | **int** |  | [optional] 
**display_priority** | **int** |  | [optional] 
**carryover_unattempted** | **int** |  | [optional] 
**visibility_crm** | **int** |  | [optional] 
**visibility_report** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_property_create import CampaignPropertyCreate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignPropertyCreate from a JSON string
campaign_property_create_instance = CampaignPropertyCreate.from_json(json)
# print the JSON string representation of the object
print(CampaignPropertyCreate.to_json())

# convert the object into a dict
campaign_property_create_dict = campaign_property_create_instance.to_dict()
# create an instance of CampaignPropertyCreate from a dict
campaign_property_create_from_dict = CampaignPropertyCreate.from_dict(campaign_property_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


