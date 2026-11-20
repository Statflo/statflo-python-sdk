# CampaignMappingPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CampaignMapping]**](CampaignMapping.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_mapping_pagination_response import CampaignMappingPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMappingPaginationResponse from a JSON string
campaign_mapping_pagination_response_instance = CampaignMappingPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignMappingPaginationResponse.to_json())

# convert the object into a dict
campaign_mapping_pagination_response_dict = campaign_mapping_pagination_response_instance.to_dict()
# create an instance of CampaignMappingPaginationResponse from a dict
campaign_mapping_pagination_response_from_dict = CampaignMappingPaginationResponse.from_dict(campaign_mapping_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


