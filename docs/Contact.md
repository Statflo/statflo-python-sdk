# Contact


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**account_name** | **str** |  | [optional] 
**account_id** | **str** |  | [optional] 
**contact_name** | **str** |  | [optional] 
**street_number** | **str** |  | [optional] 
**street_name** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**zip_code** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**phone_extension** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**primary_contact** | **bool** |  | [optional] [default to True]
**dealer** | [**Dealer**](Dealer.md) |  | 
**date_added** | **datetime** |  | [optional] 
**date_created** | **datetime** |  | [optional] 
**date_updated** | **datetime** |  | [optional] 
**job_title** | **str** |  | [optional] 
**source** | **str** |  | [optional] [default to 'api']
**source_id** | **int** |  | [optional] 
**customer_id** | **str** |  | [optional] 
**old_ban** | **str** |  | [optional] 
**sms_capable** | **bool** |  | [optional] 
**flag** | **str** |  | [optional] 
**opted_out** | **object** |  | [optional] 
**communication_methods** | **object** |  | [optional] 
**first_name** | **str** |  | [optional] 
**preferred_language** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact import Contact

# TODO update the JSON string below
json = "{}"
# create an instance of Contact from a JSON string
contact_instance = Contact.from_json(json)
# print the JSON string representation of the object
print(Contact.to_json())

# convert the object into a dict
contact_dict = contact_instance.to_dict()
# create an instance of Contact from a dict
contact_from_dict = Contact.from_dict(contact_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


