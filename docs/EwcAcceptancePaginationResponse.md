# EwcAcceptancePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[EwcAcceptance]**](EwcAcceptance.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.ewc_acceptance_pagination_response import EwcAcceptancePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EwcAcceptancePaginationResponse from a JSON string
ewc_acceptance_pagination_response_instance = EwcAcceptancePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(EwcAcceptancePaginationResponse.to_json())

# convert the object into a dict
ewc_acceptance_pagination_response_dict = ewc_acceptance_pagination_response_instance.to_dict()
# create an instance of EwcAcceptancePaginationResponse from a dict
ewc_acceptance_pagination_response_from_dict = EwcAcceptancePaginationResponse.from_dict(ewc_acceptance_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


