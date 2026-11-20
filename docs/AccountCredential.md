# AccountCredential


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
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
from statflo_python_sdk.models.account_credential import AccountCredential

# TODO update the JSON string below
json = "{}"
# create an instance of AccountCredential from a JSON string
account_credential_instance = AccountCredential.from_json(json)
# print the JSON string representation of the object
print(AccountCredential.to_json())

# convert the object into a dict
account_credential_dict = account_credential_instance.to_dict()
# create an instance of AccountCredential from a dict
account_credential_from_dict = AccountCredential.from_dict(account_credential_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


