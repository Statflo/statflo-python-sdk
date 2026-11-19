# Dealer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**country_code** | **str** |  | 
**calendar_format** | **int** |  | [optional] [default to 0]
**status** | [**DealerStatus**](DealerStatus.md) |  | 
**website** | **str** |  | [optional] 
**address_line1** | **str** |  | [optional] 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**carrier** | [**Carrier**](Carrier.md) |  | 
**permissions** | [**List[Permission]**](Permission.md) |  | 
**dealer_features** | [**List[DealerAllowedFeature]**](DealerAllowedFeature.md) |  | 
**features** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.dealer import Dealer

# TODO update the JSON string below
json = "{}"
# create an instance of Dealer from a JSON string
dealer_instance = Dealer.from_json(json)
# print the JSON string representation of the object
print(Dealer.to_json())

# convert the object into a dict
dealer_dict = dealer_instance.to_dict()
# create an instance of Dealer from a dict
dealer_from_dict = Dealer.from_dict(dealer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


