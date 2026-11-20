# ContentSharingCategory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**display_order** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 
**links** | [**List[ContentSharingLink]**](ContentSharingLink.md) |  | 

## Example

```python
from statflo_python_sdk.models.content_sharing_category import ContentSharingCategory

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingCategory from a JSON string
content_sharing_category_instance = ContentSharingCategory.from_json(json)
# print the JSON string representation of the object
print(ContentSharingCategory.to_json())

# convert the object into a dict
content_sharing_category_dict = content_sharing_category_instance.to_dict()
# create an instance of ContentSharingCategory from a dict
content_sharing_category_from_dict = ContentSharingCategory.from_dict(content_sharing_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


