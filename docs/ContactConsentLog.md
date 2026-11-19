# ContactConsentLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact** | [**Contact**](Contact.md) |  | 
**timestamp** | **datetime** |  | 
**change** | **object** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_consent_log import ContactConsentLog

# TODO update the JSON string below
json = "{}"
# create an instance of ContactConsentLog from a JSON string
contact_consent_log_instance = ContactConsentLog.from_json(json)
# print the JSON string representation of the object
print(ContactConsentLog.to_json())

# convert the object into a dict
contact_consent_log_dict = contact_consent_log_instance.to_dict()
# create an instance of ContactConsentLog from a dict
contact_consent_log_from_dict = ContactConsentLog.from_dict(contact_consent_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


