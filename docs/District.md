# District


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**region** | [**Region**](Region.md) |  | 

## Example

```python
from statflo_python_sdk.models.district import District

# TODO update the JSON string below
json = "{}"
# create an instance of District from a JSON string
district_instance = District.from_json(json)
# print the JSON string representation of the object
print(District.to_json())

# convert the object into a dict
district_dict = district_instance.to_dict()
# create an instance of District from a dict
district_from_dict = District.from_dict(district_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


