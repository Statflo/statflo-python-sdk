# CampaignVisibilityUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**visible_to** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_visibility_update import CampaignVisibilityUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignVisibilityUpdate from a JSON string
campaign_visibility_update_instance = CampaignVisibilityUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignVisibilityUpdate.to_json())

# convert the object into a dict
campaign_visibility_update_dict = campaign_visibility_update_instance.to_dict()
# create an instance of CampaignVisibilityUpdate from a dict
campaign_visibility_update_from_dict = CampaignVisibilityUpdate.from_dict(campaign_visibility_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


