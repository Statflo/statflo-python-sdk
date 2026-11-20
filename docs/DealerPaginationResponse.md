# DealerPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Dealer]**](Dealer.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_pagination_response import DealerPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DealerPaginationResponse from a JSON string
dealer_pagination_response_instance = DealerPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(DealerPaginationResponse.to_json())

# convert the object into a dict
dealer_pagination_response_dict = dealer_pagination_response_instance.to_dict()
# create an instance of DealerPaginationResponse from a dict
dealer_pagination_response_from_dict = DealerPaginationResponse.from_dict(dealer_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


