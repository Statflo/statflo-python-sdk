# CampaignMemberPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CampaignMember]**](CampaignMember.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_member_pagination_response import CampaignMemberPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignMemberPaginationResponse from a JSON string
campaign_member_pagination_response_instance = CampaignMemberPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CampaignMemberPaginationResponse.to_json())

# convert the object into a dict
campaign_member_pagination_response_dict = campaign_member_pagination_response_instance.to_dict()
# create an instance of CampaignMemberPaginationResponse from a dict
campaign_member_pagination_response_from_dict = CampaignMemberPaginationResponse.from_dict(campaign_member_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


