# Campaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**campaign_nickname** | **str** |  | 
**totango_name** | **str** |  | [optional] 
**type** | **str** |  | [optional] [default to 'add']
**frequency** | **str** |  | [optional] [default to 'monthly']
**lifetime** | **str** |  | [optional] [default to 'monthly']
**method** | **str** |  | [optional] [default to 'provided']
**carrier_allowed** | **bool** |  | [optional] [default to False]
**account_type** | **str** |  | [optional] [default to 'I']
**dnc_scrub** | **bool** |  | [optional] [default to False]
**reporting_period_type** | **str** |  | [optional] [default to 'month']
**reporting_period_before** | **int** |  | [optional] [default to 0]
**reporting_period_after** | **int** |  | [optional] [default to 0]
**transaction_earliest** | **str** |  | [optional] 
**transaction_latest** | **str** |  | [optional] 
**product_types** | **str** |  | [optional] 
**source** | **str** |  | [optional] [default to 'api']
**campaign_metadata** | [**List[CampaignMetadata]**](CampaignMetadata.md) |  | 
**campaign_mappings** | [**List[CampaignMapping]**](CampaignMapping.md) |  | 
**campaign_properties** | [**List[CampaignProperty]**](CampaignProperty.md) |  | 

## Example

```python
from statflo_python_sdk.models.campaign import Campaign

# TODO update the JSON string below
json = "{}"
# create an instance of Campaign from a JSON string
campaign_instance = Campaign.from_json(json)
# print the JSON string representation of the object
print(Campaign.to_json())

# convert the object into a dict
campaign_dict = campaign_instance.to_dict()
# create an instance of Campaign from a dict
campaign_from_dict = Campaign.from_dict(campaign_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


