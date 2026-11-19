# AccountContactMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**contact_id** | **int** |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_contact_metadata_create import AccountContactMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountContactMetadataCreate from a JSON string
account_contact_metadata_create_instance = AccountContactMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(AccountContactMetadataCreate.to_json())

# convert the object into a dict
account_contact_metadata_create_dict = account_contact_metadata_create_instance.to_dict()
# create an instance of AccountContactMetadataCreate from a dict
account_contact_metadata_create_from_dict = AccountContactMetadataCreate.from_dict(account_contact_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


