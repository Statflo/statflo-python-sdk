# RcsAgent


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
**rep_user** | [**User**](User.md) |  | 
**website** | **List[object]** |  | 
**email** | **List[object]** |  | 
**phone_number** | **List[object]** |  | 
**regulation_id** | **str** |  | [optional] [default to 'RN285c55a933ea017bdc9c0d6e6ad1ce00']
**regulation_version** | **int** |  | [optional] [default to 1]
**us_regulation_id** | **str** |  | [optional] [default to 'RN3038ea6be8e9792456beb40f0a18695d']
**us_regulation_version** | **int** |  | [optional] [default to 1]
**comment** | **str** |  | [optional] 
**friendly_name** | **str** |  | [optional] 
**status_notification_email** | **str** |  | [optional] 
**status_callback_url** | **str** |  | [optional] 
**sid** | **str** |  | [optional] 
**registration_sid** | **str** |  | [optional] 
**google_registration_sid** | **str** |  | [optional] 
**address_sid** | **str** |  | [optional] 
**user** | [**User**](User.md) |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**rcs_agent_use_case** | [**RcsAgentUseCase**](RcsAgentUseCase.md) |  | 
**rcs_agent_business** | [**RcsAgentBusiness**](RcsAgentBusiness.md) |  | 
**rcs_agent_metadata** | [**List[RcsAgentMetadata]**](RcsAgentMetadata.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent import RcsAgent

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgent from a JSON string
rcs_agent_instance = RcsAgent.from_json(json)
# print the JSON string representation of the object
print(RcsAgent.to_json())

# convert the object into a dict
rcs_agent_dict = rcs_agent_instance.to_dict()
# create an instance of RcsAgent from a dict
rcs_agent_from_dict = RcsAgent.from_dict(rcs_agent_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


