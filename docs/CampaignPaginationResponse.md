# CampaignPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Campaign]**](Campaign.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_pagination_response import CampaignPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignPaginationResponse from a JSON string
campaign_pagination_response_instance = CampaignPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignPaginationResponse.to_json())

# convert the object into a dict
campaign_pagination_response_dict = campaign_pagination_response_instance.to_dict()
# create an instance of CampaignPaginationResponse from a dict
campaign_pagination_response_from_dict = CampaignPaginationResponse.from_dict(campaign_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


