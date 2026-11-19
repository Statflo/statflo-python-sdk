# TimelinePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Timeline]**](Timeline.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.timeline_pagination_response import TimelinePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TimelinePaginationResponse from a JSON string
timeline_pagination_response_instance = TimelinePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(TimelinePaginationResponse.to_json())

# convert the object into a dict
timeline_pagination_response_dict = timeline_pagination_response_instance.to_dict()
# create an instance of TimelinePaginationResponse from a dict
timeline_pagination_response_from_dict = TimelinePaginationResponse.from_dict(timeline_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


