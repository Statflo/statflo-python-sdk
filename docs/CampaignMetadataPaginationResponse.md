# CampaignMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CampaignMetadata]**](CampaignMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_metadata_pagination_response import CampaignMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMetadataPaginationResponse from a JSON string
campaign_metadata_pagination_response_instance = CampaignMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignMetadataPaginationResponse.to_json())

# convert the object into a dict
campaign_metadata_pagination_response_dict = campaign_metadata_pagination_response_instance.to_dict()
# create an instance of CampaignMetadataPaginationResponse from a dict
campaign_metadata_pagination_response_from_dict = CampaignMetadataPaginationResponse.from_dict(campaign_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


