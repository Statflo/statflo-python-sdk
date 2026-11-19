# CampaignMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**metadata** | **str** |  | [optional] 
**value** | **object** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.campaign_metadata import CampaignMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMetadata from a JSON string
campaign_metadata_instance = CampaignMetadata.from_json(json)
# print the JSON string representation of the object
print(CampaignMetadata.to_json())

# convert the object into a dict
campaign_metadata_dict = campaign_metadata_instance.to_dict()
# create an instance of CampaignMetadata from a dict
campaign_metadata_from_dict = CampaignMetadata.from_dict(campaign_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


