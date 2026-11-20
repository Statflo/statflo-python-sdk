# ContentSharingRecommendedCreate


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
from statflo_python_sdk.models.content_sharing_recommended_create import ContentSharingRecommendedCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ContentSharingRecommendedCreate from a JSON string
content_sharing_recommended_create_instance = ContentSharingRecommendedCreate.from_json(json)
# print the JSON string representation of the object
print(ContentSharingRecommendedCreate.to_json())

# convert the object into a dict
content_sharing_recommended_create_dict = content_sharing_recommended_create_instance.to_dict()
# create an instance of ContentSharingRecommendedCreate from a dict
content_sharing_recommended_create_from_dict = ContentSharingRecommendedCreate.from_dict(content_sharing_recommended_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


