# ContentSharingRecommendPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[ContentSharingRecommendPaginationResponse]**](ContentSharingRecommendPaginationResponse.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_recommend_pagination_response import ContentSharingRecommendPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingRecommendPaginationResponse from a JSON string
content_sharing_recommend_pagination_response_instance = ContentSharingRecommendPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ContentSharingRecommendPaginationResponse.to_json())

# convert the object into a dict
content_sharing_recommend_pagination_response_dict = content_sharing_recommend_pagination_response_instance.to_dict()
# create an instance of ContentSharingRecommendPaginationResponse from a dict
content_sharing_recommend_pagination_response_from_dict = ContentSharingRecommendPaginationResponse.from_dict(content_sharing_recommend_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


