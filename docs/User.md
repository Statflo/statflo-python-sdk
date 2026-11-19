# User


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
**language** | **str** |  | [optional] [default to 'en']
**sales_rep_id** | **str** |  | [optional] 
**external_location_id** | **str** |  | [optional] 
**district_id** | **int** |  | [optional] 
**region_id** | **int** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**theme** | **int** |  | [optional] [default to 2]
**user_active** | **bool** |  | [optional] [default to True]
**inbound_available** | **bool** |  | [optional] [default to False]
**job_title** | **str** |  | [optional] 
**accepted_terms_conditions** | **bool** |  | [optional] 
**appointment_reminder_email** | **bool** |  | [optional] [default to True]
**dealer** | [**Dealer**](Dealer.md) |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**role** | [**Role**](Role.md) |  | 
**user_permissions** | [**List[UserPermission]**](UserPermission.md) |  | 
**user_teams** | [**List[UserTeam]**](UserTeam.md) |  | 
**user_metadata** | [**List[UserMetadata]**](UserMetadata.md) |  | 
**date_added** | **datetime** |  | [optional] 
**campaign_visibility** | **int** |  | [optional] [default to 30]
**permissions** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.user import User

# TODO update the JSON string below
json = "{}"
# create an instance of User from a JSON string
user_instance = User.from_json(json)
# print the JSON string representation of the object
print(User.to_json())

# convert the object into a dict
user_dict = user_instance.to_dict()
# create an instance of User from a dict
user_from_dict = User.from_dict(user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


