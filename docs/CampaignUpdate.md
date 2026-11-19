# CampaignUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**campaign_nickname** | **str** |  | 
**totango_name** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**frequency** | **str** |  | [optional] 
**lifetime** | **str** |  | [optional] 
**method** | **str** |  | [optional] 
**carrier_allowed** | **bool** |  | [optional] 
**account_type** | **str** |  | [optional] 
**dnc_scrub** | **bool** |  | [optional] 
**reporting_period_type** | **str** |  | [optional] 
**reporting_period_before** | **int** |  | [optional] 
**reporting_period_after** | **int** |  | [optional] 
**transaction_earliest** | **str** |  | [optional] 
**transaction_latest** | **str** |  | [optional] 
**product_types** | **str** |  | [optional] 
**source** | **str** |  | [optional] 
**visibility_crm** | **int** |  | [optional] 
**visibility_report** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.campaign_update import CampaignUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CampaignUpdate from a JSON string
campaign_update_instance = CampaignUpdate.from_json(json)
# print the JSON string representation of the object
print(CampaignUpdate.to_json())

# convert the object into a dict
campaign_update_dict = campaign_update_instance.to_dict()
# create an instance of CampaignUpdate from a dict
campaign_update_from_dict = CampaignUpdate.from_dict(campaign_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


