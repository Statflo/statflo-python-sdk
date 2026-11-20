# AccountCredentialUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**account_sid** | **str** |  | [optional] 
**auth_token** | **str** |  | [optional] 
**secondary_business_profile_sid** | **str** |  | [optional] 
**address_sid** | **str** |  | [optional] 
**supporting_document_sid** | **str** |  | [optional] 
**customer_profile_business_information_sid** | **str** |  | [optional] 
**authorized_representative_sid** | **str** |  | [optional] 
**messaging_service_id** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_credential_update import AccountCredentialUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountCredentialUpdate from a JSON string
account_credential_update_instance = AccountCredentialUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountCredentialUpdate.to_json())

# convert the object into a dict
account_credential_update_dict = account_credential_update_instance.to_dict()
# create an instance of AccountCredentialUpdate from a dict
account_credential_update_from_dict = AccountCredentialUpdate.from_dict(account_credential_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


