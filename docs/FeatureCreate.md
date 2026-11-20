# FeatureCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**category** | **str** |  | [optional] 
**default_package** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.feature_create import FeatureCreate

# TODO update the JSON string below
json = "{}"
# create an instance of FeatureCreate from a JSON string
feature_create_instance = FeatureCreate.from_json(json)
# print the JSON string representation of the object
print(FeatureCreate.to_json())

# convert the object into a dict
feature_create_dict = feature_create_instance.to_dict()
# create an instance of FeatureCreate from a dict
feature_create_from_dict = FeatureCreate.from_dict(feature_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


