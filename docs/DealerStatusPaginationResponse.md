# DealerStatusPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[DealerStatus]**](DealerStatus.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_status_pagination_response import DealerStatusPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DealerStatusPaginationResponse from a JSON string
dealer_status_pagination_response_instance = DealerStatusPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(DealerStatusPaginationResponse.to_json())

# convert the object into a dict
dealer_status_pagination_response_dict = dealer_status_pagination_response_instance.to_dict()
# create an instance of DealerStatusPaginationResponse from a dict
dealer_status_pagination_response_from_dict = DealerStatusPaginationResponse.from_dict(dealer_status_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


