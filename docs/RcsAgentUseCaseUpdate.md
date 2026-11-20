# RcsAgentUseCaseUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**organic_website_traffic_monthly** | **int** |  | [optional] 
**has_existing_short_code_traffic** | **bool** |  | [optional] 
**existing_short_code_number** | **str** |  | [optional] 
**existing_short_code_traffic_monthly** | **int** |  | [optional] 
**rbm_traffic_forecast_monthly** | **int** |  | [optional] 
**campaign_overview** | **str** |  | [optional] 
**messaging_flow** | **str** |  | [optional] 
**help_sample_message** | **str** |  | [optional] 
**stop_sample_message** | **str** |  | [optional] 
**message_service_type** | **str** |  | [optional] 
**access_instructions** | **str** |  | [optional] 
**opt_in_description** | **str** |  | [optional] 
**opt_out_description** | **str** |  | [optional] 
**screenshot_urls** | **List[str]** |  | 
**trigger_event_description** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**video_urls** | **List[str]** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_use_case_update import RcsAgentUseCaseUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentUseCaseUpdate from a JSON string
rcs_agent_use_case_update_instance = RcsAgentUseCaseUpdate.from_json(json)
# print the JSON string representation of the object
print(RcsAgentUseCaseUpdate.to_json())

# convert the object into a dict
rcs_agent_use_case_update_dict = rcs_agent_use_case_update_instance.to_dict()
# create an instance of RcsAgentUseCaseUpdate from a dict
rcs_agent_use_case_update_from_dict = RcsAgentUseCaseUpdate.from_dict(rcs_agent_use_case_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


