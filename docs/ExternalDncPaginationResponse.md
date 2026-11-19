# ExternalDncPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[ExternalDnc]**](ExternalDnc.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.external_dnc_pagination_response import ExternalDncPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ExternalDncPaginationResponse from a JSON string
external_dnc_pagination_response_instance = ExternalDncPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ExternalDncPaginationResponse.to_json())

# convert the object into a dict
external_dnc_pagination_response_dict = external_dnc_pagination_response_instance.to_dict()
# create an instance of ExternalDncPaginationResponse from a dict
external_dnc_pagination_response_from_dict = ExternalDncPaginationResponse.from_dict(external_dnc_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


