# ContentSharingRecommended


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**link** | [**ContentSharingLink**](ContentSharingLink.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_recommended import ContentSharingRecommended

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingRecommended from a JSON string
content_sharing_recommended_instance = ContentSharingRecommended.from_json(json)
# print the JSON string representation of the object
print(ContentSharingRecommended.to_json())

# convert the object into a dict
content_sharing_recommended_dict = content_sharing_recommended_instance.to_dict()
# create an instance of ContentSharingRecommended from a dict
content_sharing_recommended_from_dict = ContentSharingRecommended.from_dict(content_sharing_recommended_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


