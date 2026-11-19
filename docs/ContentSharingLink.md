# ContentSharingLink


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**category** | [**ContentSharingCategory**](ContentSharingCategory.md) |  | 
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
from statflo_python_sdk.models.content_sharing_link import ContentSharingLink

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingLink from a JSON string
content_sharing_link_instance = ContentSharingLink.from_json(json)
# print the JSON string representation of the object
print(ContentSharingLink.to_json())

# convert the object into a dict
content_sharing_link_dict = content_sharing_link_instance.to_dict()
# create an instance of ContentSharingLink from a dict
content_sharing_link_from_dict = ContentSharingLink.from_dict(content_sharing_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


