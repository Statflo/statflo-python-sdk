# Brand


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 

## Example

```python
from statflo_python_sdk.models.brand import Brand

# TODO update the JSON string below
json = "{}"
# create an instance of Brand from a JSON string
brand_instance = Brand.from_json(json)
# print the JSON string representation of the object
print(Brand.to_json())

# convert the object into a dict
brand_dict = brand_instance.to_dict()
# create an instance of Brand from a dict
brand_from_dict = Brand.from_dict(brand_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


