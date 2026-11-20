# RcsAgentUseCase


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
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_use_case import RcsAgentUseCase

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentUseCase from a JSON string
rcs_agent_use_case_instance = RcsAgentUseCase.from_json(json)
# print the JSON string representation of the object
print(RcsAgentUseCase.to_json())

# convert the object into a dict
rcs_agent_use_case_dict = rcs_agent_use_case_instance.to_dict()
# create an instance of RcsAgentUseCase from a dict
rcs_agent_use_case_from_dict = RcsAgentUseCase.from_dict(rcs_agent_use_case_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


