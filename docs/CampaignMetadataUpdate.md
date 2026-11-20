# CampaignMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**campaign_id** | **int** |  | [optional] 
**metadata** | **str** |  | [optional] 
**value** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.campaign_metadata_update import CampaignMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMetadataUpdate from a JSON string
campaign_metadata_update_instance = CampaignMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignMetadataUpdate.to_json())

# convert the object into a dict
campaign_metadata_update_dict = campaign_metadata_update_instance.to_dict()
# create an instance of CampaignMetadataUpdate from a dict
campaign_metadata_update_from_dict = CampaignMetadataUpdate.from_dict(campaign_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


