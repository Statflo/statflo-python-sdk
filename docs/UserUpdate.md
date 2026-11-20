# UserUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**username** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**company** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**password** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**sales_rep_id** | **str** |  | [optional] 
**external_location_id** | **str** |  | [optional] 
**district_id** | **int** |  | [optional] 
**region_id** | **int** |  | [optional] 
**last_login** | **datetime** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**theme** | **int** |  | [optional] 
**token** | **str** |  | [optional] 
**token_paragon** | **str** |  | [optional] 
**user_active** | **bool** |  | [optional] 
**inbound_available** | **bool** |  | [optional] 
**job_title** | **str** |  | [optional] 
**accepted_terms_conditions** | **bool** |  | [optional] 
**appointment_reminder_email** | **bool** |  | [optional] 
**dealer_id** | **int** |  | 
**role_id** | **int** |  | [optional] 
**date_added** | **datetime** |  | [optional] 
**campaign_visibility** | **int** |  | [optional] 
**permissions** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.user_update import UserUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserUpdate from a JSON string
user_update_instance = UserUpdate.from_json(json)
# print the JSON string representation of the object
print(UserUpdate.to_json())

# convert the object into a dict
user_update_dict = user_update_instance.to_dict()
# create an instance of UserUpdate from a dict
user_update_from_dict = UserUpdate.from_dict(user_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


