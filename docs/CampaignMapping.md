# CampaignMapping


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**file_name** | **str** |  | 
**date_added** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_mapping import CampaignMapping

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMapping from a JSON string
campaign_mapping_instance = CampaignMapping.from_json(json)
# print the JSON string representation of the object
print(CampaignMapping.to_json())

# convert the object into a dict
campaign_mapping_dict = campaign_mapping_instance.to_dict()
# create an instance of CampaignMapping from a dict
campaign_mapping_from_dict = CampaignMapping.from_dict(campaign_mapping_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


