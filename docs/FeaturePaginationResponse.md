# FeaturePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Feature]**](Feature.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.feature_pagination_response import FeaturePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FeaturePaginationResponse from a JSON string
feature_pagination_response_instance = FeaturePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(FeaturePaginationResponse.to_json())

# convert the object into a dict
feature_pagination_response_dict = feature_pagination_response_instance.to_dict()
# create an instance of FeaturePaginationResponse from a dict
feature_pagination_response_from_dict = FeaturePaginationResponse.from_dict(feature_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


