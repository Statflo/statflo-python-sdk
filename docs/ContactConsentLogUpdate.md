# ContactConsentLogUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact_id** | **int** |  | 
**timestamp** | **datetime** |  | 
**change** | **object** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_consent_log_update import ContactConsentLogUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ContactConsentLogUpdate from a JSON string
contact_consent_log_update_instance = ContactConsentLogUpdate.from_json(json)
# print the JSON string representation of the object
print(ContactConsentLogUpdate.to_json())

# convert the object into a dict
contact_consent_log_update_dict = contact_consent_log_update_instance.to_dict()
# create an instance of ContactConsentLogUpdate from a dict
contact_consent_log_update_from_dict = ContactConsentLogUpdate.from_dict(contact_consent_log_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


