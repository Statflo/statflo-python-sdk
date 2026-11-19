# Location


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**external_dealer_id** | **str** |  | [optional] 
**dealer** | [**Dealer**](Dealer.md) |  | 
**district** | [**District**](District.md) |  | 
**external_location_id** | **str** |  | [optional] 
**salesforce_location_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**address_line1** | **str** |  | [optional] 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**zip_code** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
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
from statflo_python_sdk.models.location import Location

# TODO update the JSON string below
json = "{}"
# create an instance of Location from a JSON string
location_instance = Location.from_json(json)
# print the JSON string representation of the object
print(Location.to_json())

# convert the object into a dict
location_dict = location_instance.to_dict()
# create an instance of Location from a dict
location_from_dict = Location.from_dict(location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


