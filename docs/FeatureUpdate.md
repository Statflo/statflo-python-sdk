# FeatureUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**category** | **str** |  | [optional] 
**default_package** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.feature_update import FeatureUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of FeatureUpdate from a JSON string
feature_update_instance = FeatureUpdate.from_json(json)
# print the JSON string representation of the object
print(FeatureUpdate.to_json())

# convert the object into a dict
feature_update_dict = feature_update_instance.to_dict()
# create an instance of FeatureUpdate from a dict
feature_update_from_dict = FeatureUpdate.from_dict(feature_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


