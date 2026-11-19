# AccountContactMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**contact** | [**Contact**](Contact.md) |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_contact_metadata import AccountContactMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of AccountContactMetadata from a JSON string
account_contact_metadata_instance = AccountContactMetadata.from_json(json)
# print the JSON string representation of the object
print(AccountContactMetadata.to_json())

# convert the object into a dict
account_contact_metadata_dict = account_contact_metadata_instance.to_dict()
# create an instance of AccountContactMetadata from a dict
account_contact_metadata_from_dict = AccountContactMetadata.from_dict(account_contact_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


