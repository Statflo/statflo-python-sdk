# DealerExternalIdPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[DealerExternalId]**](DealerExternalId.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.dealer_external_id_pagination_response import DealerExternalIdPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DealerExternalIdPaginationResponse from a JSON string
dealer_external_id_pagination_response_instance = DealerExternalIdPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(DealerExternalIdPaginationResponse.to_json())

# convert the object into a dict
dealer_external_id_pagination_response_dict = dealer_external_id_pagination_response_instance.to_dict()
# create an instance of DealerExternalIdPaginationResponse from a dict
dealer_external_id_pagination_response_from_dict = DealerExternalIdPaginationResponse.from_dict(dealer_external_id_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


