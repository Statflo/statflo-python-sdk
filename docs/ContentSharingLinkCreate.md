# ContentSharingLinkCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**category_id** | **int** |  | 
**language** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**url** | **str** |  | 
**image** | **str** |  | [optional] 
**status** | **bool** |  | 
**display_order** | **int** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_link_create import ContentSharingLinkCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingLinkCreate from a JSON string
content_sharing_link_create_instance = ContentSharingLinkCreate.from_json(json)
# print the JSON string representation of the object
print(ContentSharingLinkCreate.to_json())

# convert the object into a dict
content_sharing_link_create_dict = content_sharing_link_create_instance.to_dict()
# create an instance of ContentSharingLinkCreate from a dict
content_sharing_link_create_from_dict = ContentSharingLinkCreate.from_dict(content_sharing_link_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


