# CarrierPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Carrier]**](Carrier.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.carrier_pagination_response import CarrierPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CarrierPaginationResponse from a JSON string
carrier_pagination_response_instance = CarrierPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CarrierPaginationResponse.to_json())

# convert the object into a dict
carrier_pagination_response_dict = carrier_pagination_response_instance.to_dict()
# create an instance of CarrierPaginationResponse from a dict
carrier_pagination_response_from_dict = CarrierPaginationResponse.from_dict(carrier_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


