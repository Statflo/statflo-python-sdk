# CarrierStatisticPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CarrierStatistic]**](CarrierStatistic.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.carrier_statistic_pagination_response import CarrierStatisticPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CarrierStatisticPaginationResponse from a JSON string
carrier_statistic_pagination_response_instance = CarrierStatisticPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CarrierStatisticPaginationResponse.to_json())

# convert the object into a dict
carrier_statistic_pagination_response_dict = carrier_statistic_pagination_response_instance.to_dict()
# create an instance of CarrierStatisticPaginationResponse from a dict
carrier_statistic_pagination_response_from_dict = CarrierStatisticPaginationResponse.from_dict(carrier_statistic_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


