# LocationCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**external_dealer_id** | **str** |  | [optional] 
**district_id** | **int** |  | 
**external_location_id** | **str** |  | [optional] 
**salesforce_location_id** | **str** |  | [optional] 
**name** | **str** |  | 
**address_line1** | **str** |  | 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | 
**state** | **str** |  | 
**zip_code** | **str** |  | 
**country** | **str** |  | 
**phone** | **str** |  | 
**fax** | **str** |  | [optional] 
**website** | **str** |  | [optional] 
**manager** | **str** |  | [optional] 
**manager_phone** | **str** |  | [optional] 
**manager_email** | **str** |  | [optional] 
**locator** | **str** |  | [optional] 
**address** | **str** |  | [optional] 
**outlet** | **str** |  | [optional] 
**full_address** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.location_create import LocationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationCreate from a JSON string
location_create_instance = LocationCreate.from_json(json)
# print the JSON string representation of the object
print(LocationCreate.to_json())

# convert the object into a dict
location_create_dict = location_create_instance.to_dict()
# create an instance of LocationCreate from a dict
location_create_from_dict = LocationCreate.from_dict(location_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


