# RcsAgentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**application_name** | **str** |  | 
**sender_id** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | 
**logo_url** | **str** |  | 
**banner_url** | **str** |  | 
**privacy_url** | **str** |  | 
**terms_of_service_url** | **str** |  | 
**accent_color** | **str** |  | 
**callback_url** | **str** |  | 
**callback_method** | **str** |  | 
**fallback_url** | **str** |  | [optional] 
**fallback_method** | **str** |  | [optional] 
**status** | **str** |  | 
**rep_user_id** | **int** |  | 
**website** | **List[object]** |  | 
**email** | **List[object]** |  | 
**phone_number** | **List[object]** |  | 
**regulation_id** | **str** |  | [optional] 
**regulation_version** | **int** |  | [optional] 
**us_regulation_id** | **str** |  | [optional] 
**us_regulation_version** | **int** |  | [optional] 
**comment** | **str** |  | [optional] 
**friendly_name** | **str** |  | [optional] 
**status_notification_email** | **str** |  | [optional] 
**status_callback_url** | **str** |  | [optional] 
**sid** | **str** |  | [optional] 
**registration_sid** | **str** |  | [optional] 
**google_registration_sid** | **str** |  | [optional] 
**address_sid** | **str** |  | [optional] 
**rcs_agent_use_case_id** | **int** |  | [optional] 
**rcs_agent_business_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_update import RcsAgentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentUpdate from a JSON string
rcs_agent_update_instance = RcsAgentUpdate.from_json(json)
# print the JSON string representation of the object
print(RcsAgentUpdate.to_json())

# convert the object into a dict
rcs_agent_update_dict = rcs_agent_update_instance.to_dict()
# create an instance of RcsAgentUpdate from a dict
rcs_agent_update_from_dict = RcsAgentUpdate.from_dict(rcs_agent_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


