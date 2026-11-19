# CampaignProperty


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**campaign_priority** | **int** |  | [optional] 
**display_priority** | **int** |  | [optional] 
**carryover_unattempted** | **int** |  | [optional] 
**visibility_crm_status** | [**CampaignVisibility**](CampaignVisibility.md) |  | 
**visibility_report_status** | [**CampaignVisibility**](CampaignVisibility.md) |  | 
**message_template_assignments** | [**List[MessageTemplateAssignment]**](MessageTemplateAssignment.md) |  | 

## Example

```python
from statflo_python_sdk.models.campaign_property import CampaignProperty

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignProperty from a JSON string
campaign_property_instance = CampaignProperty.from_json(json)
# print the JSON string representation of the object
print(CampaignProperty.to_json())

# convert the object into a dict
campaign_property_dict = campaign_property_instance.to_dict()
# create an instance of CampaignProperty from a dict
campaign_property_from_dict = CampaignProperty.from_dict(campaign_property_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


