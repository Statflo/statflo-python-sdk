# CampaignPropertyPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CampaignProperty]**](CampaignProperty.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_property_pagination_response import CampaignPropertyPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignPropertyPaginationResponse from a JSON string
campaign_property_pagination_response_instance = CampaignPropertyPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignPropertyPaginationResponse.to_json())

# convert the object into a dict
campaign_property_pagination_response_dict = campaign_property_pagination_response_instance.to_dict()
# create an instance of CampaignPropertyPaginationResponse from a dict
campaign_property_pagination_response_from_dict = CampaignPropertyPaginationResponse.from_dict(campaign_property_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


