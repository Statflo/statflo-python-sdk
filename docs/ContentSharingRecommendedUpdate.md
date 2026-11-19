# ContentSharingRecommendedUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**campaign_id** | **int** |  | [optional] 
**link** | [**ContentSharingLink**](ContentSharingLink.md) |  | 
**content_id** | **int** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.content_sharing_recommended_update import ContentSharingRecommendedUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingRecommendedUpdate from a JSON string
content_sharing_recommended_update_instance = ContentSharingRecommendedUpdate.from_json(json)
# print the JSON string representation of the object
print(ContentSharingRecommendedUpdate.to_json())

# convert the object into a dict
content_sharing_recommended_update_dict = content_sharing_recommended_update_instance.to_dict()
# create an instance of ContentSharingRecommendedUpdate from a dict
content_sharing_recommended_update_from_dict = ContentSharingRecommendedUpdate.from_dict(content_sharing_recommended_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


