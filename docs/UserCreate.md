# UserCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**username** | **str** |  | 
**first_name** | **str** |  | 
**last_name** | **str** |  | 
**company** | **str** |  | [optional] 
**email** | **str** |  | 
**password** | **str** |  | 
**language** | **str** |  | [optional] [default to 'en']
**sales_rep_id** | **str** |  | [optional] 
**external_location_id** | **str** |  | [optional] 
**district_id** | **int** |  | [optional] 
**region_id** | **int** |  | [optional] 
**last_login** | **datetime** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**theme** | **int** |  | [optional] [default to 2]
**token** | **str** |  | [optional] 
**token_paragon** | **str** |  | [optional] 
**user_active** | **bool** |  | [optional] [default to True]
**inbound_available** | **bool** |  | [optional] [default to False]
**job_title** | **str** |  | [optional] 
**accepted_terms_conditions** | **bool** |  | [optional] 
**appointment_reminder_email** | **bool** |  | [optional] [default to True]
**dealer_id** | **int** |  | 
**role_id** | **int** |  | [optional] [default to 2]
**date_added** | **datetime** |  | [optional] 
**campaign_visibility** | **int** |  | [optional] [default to 30]
**permissions** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.user_create import UserCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserCreate from a JSON string
user_create_instance = UserCreate.from_json(json)
# print the JSON string representation of the object
print(UserCreate.to_json())

# convert the object into a dict
user_create_dict = user_create_instance.to_dict()
# create an instance of UserCreate from a dict
user_create_from_dict = UserCreate.from_dict(user_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


