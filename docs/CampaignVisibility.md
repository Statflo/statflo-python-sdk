# CampaignVisibility


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**visible_to** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_visibility import CampaignVisibility

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignVisibility from a JSON string
campaign_visibility_instance = CampaignVisibility.from_json(json)
# print the JSON string representation of the object
print(CampaignVisibility.to_json())

# convert the object into a dict
campaign_visibility_dict = campaign_visibility_instance.to_dict()
# create an instance of CampaignVisibility from a dict
campaign_visibility_from_dict = CampaignVisibility.from_dict(campaign_visibility_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


