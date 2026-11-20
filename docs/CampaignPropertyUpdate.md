# CampaignPropertyUpdate


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
from statflo_python_sdk.models.campaign_property_update import CampaignPropertyUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignPropertyUpdate from a JSON string
campaign_property_update_instance = CampaignPropertyUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignPropertyUpdate.to_json())

# convert the object into a dict
campaign_property_update_dict = campaign_property_update_instance.to_dict()
# create an instance of CampaignPropertyUpdate from a dict
campaign_property_update_from_dict = CampaignPropertyUpdate.from_dict(campaign_property_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


