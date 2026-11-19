# AccountContactMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact_id** | **int** |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_contact_metadata_update import AccountContactMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountContactMetadataUpdate from a JSON string
account_contact_metadata_update_instance = AccountContactMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountContactMetadataUpdate.to_json())

# convert the object into a dict
account_contact_metadata_update_dict = account_contact_metadata_update_instance.to_dict()
# create an instance of AccountContactMetadataUpdate from a dict
account_contact_metadata_update_from_dict = AccountContactMetadataUpdate.from_dict(account_contact_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


