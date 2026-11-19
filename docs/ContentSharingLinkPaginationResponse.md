# ContentSharingLinkPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[ContentSharingLinkPaginationResponse]**](ContentSharingLinkPaginationResponse.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_link_pagination_response import ContentSharingLinkPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingLinkPaginationResponse from a JSON string
content_sharing_link_pagination_response_instance = ContentSharingLinkPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ContentSharingLinkPaginationResponse.to_json())

# convert the object into a dict
content_sharing_link_pagination_response_dict = content_sharing_link_pagination_response_instance.to_dict()
# create an instance of ContentSharingLinkPaginationResponse from a dict
content_sharing_link_pagination_response_from_dict = ContentSharingLinkPaginationResponse.from_dict(content_sharing_link_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


