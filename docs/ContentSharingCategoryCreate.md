# ContentSharingCategoryCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**display_order** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_category_create import ContentSharingCategoryCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingCategoryCreate from a JSON string
content_sharing_category_create_instance = ContentSharingCategoryCreate.from_json(json)
# print the JSON string representation of the object
print(ContentSharingCategoryCreate.to_json())

# convert the object into a dict
content_sharing_category_create_dict = content_sharing_category_create_instance.to_dict()
# create an instance of ContentSharingCategoryCreate from a dict
content_sharing_category_create_from_dict = ContentSharingCategoryCreate.from_dict(content_sharing_category_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


