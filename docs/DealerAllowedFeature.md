# DealerAllowedFeature


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**dealer** | [**Dealer**](Dealer.md) |  | 
**feature** | [**Feature**](Feature.md) |  | 

## Example

```python
from statflo_python_sdk.models.dealer_allowed_feature import DealerAllowedFeature

# TODO update the JSON string below
json = "{}"
# create an instance of DealerAllowedFeature from a JSON string
dealer_allowed_feature_instance = DealerAllowedFeature.from_json(json)
# print the JSON string representation of the object
print(DealerAllowedFeature.to_json())

# convert the object into a dict
dealer_allowed_feature_dict = dealer_allowed_feature_instance.to_dict()
# create an instance of DealerAllowedFeature from a dict
dealer_allowed_feature_from_dict = DealerAllowedFeature.from_dict(dealer_allowed_feature_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


