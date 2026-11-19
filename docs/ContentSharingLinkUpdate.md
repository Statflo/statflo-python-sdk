# ContentSharingLinkUpdate


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
from statflo_python_sdk.models.content_sharing_link_update import ContentSharingLinkUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingLinkUpdate from a JSON string
content_sharing_link_update_instance = ContentSharingLinkUpdate.from_json(json)
# print the JSON string representation of the object
print(ContentSharingLinkUpdate.to_json())

# convert the object into a dict
content_sharing_link_update_dict = content_sharing_link_update_instance.to_dict()
# create an instance of ContentSharingLinkUpdate from a dict
content_sharing_link_update_from_dict = ContentSharingLinkUpdate.from_dict(content_sharing_link_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


