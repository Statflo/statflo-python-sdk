# CampaignActionPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CampaignAction]**](CampaignAction.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_action_pagination_response import CampaignActionPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignActionPaginationResponse from a JSON string
campaign_action_pagination_response_instance = CampaignActionPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignActionPaginationResponse.to_json())

# convert the object into a dict
campaign_action_pagination_response_dict = campaign_action_pagination_response_instance.to_dict()
# create an instance of CampaignActionPaginationResponse from a dict
campaign_action_pagination_response_from_dict = CampaignActionPaginationResponse.from_dict(campaign_action_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


