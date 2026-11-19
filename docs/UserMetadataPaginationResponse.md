# UserMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[UserMetadata]**](UserMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_metadata_pagination_response import UserMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserMetadataPaginationResponse from a JSON string
user_metadata_pagination_response_instance = UserMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(UserMetadataPaginationResponse.to_json())

# convert the object into a dict
user_metadata_pagination_response_dict = user_metadata_pagination_response_instance.to_dict()
# create an instance of UserMetadataPaginationResponse from a dict
user_metadata_pagination_response_from_dict = UserMetadataPaginationResponse.from_dict(user_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


