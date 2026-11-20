# CampaignMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**campaign_id** | **int** |  | 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.campaign_metadata_create import CampaignMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMetadataCreate from a JSON string
campaign_metadata_create_instance = CampaignMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(CampaignMetadataCreate.to_json())

# convert the object into a dict
campaign_metadata_create_dict = campaign_metadata_create_instance.to_dict()
# create an instance of CampaignMetadataCreate from a dict
campaign_metadata_create_from_dict = CampaignMetadataCreate.from_dict(campaign_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


