# CampaignVisibilityCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**visible_to** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_visibility_create import CampaignVisibilityCreate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignVisibilityCreate from a JSON string
campaign_visibility_create_instance = CampaignVisibilityCreate.from_json(json)
# print the JSON string representation of the object
print(CampaignVisibilityCreate.to_json())

# convert the object into a dict
campaign_visibility_create_dict = campaign_visibility_create_instance.to_dict()
# create an instance of CampaignVisibilityCreate from a dict
campaign_visibility_create_from_dict = CampaignVisibilityCreate.from_dict(campaign_visibility_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


