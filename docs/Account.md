# Account


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | [optional] 
**account_id** | **str** |  | [optional] 
**account_type** | **str** |  | [optional] [default to 'I']
**external_user_id** | **str** |  | [optional] 
**external_location_id** | **str** |  | [optional] [default to 'unassigned']
**city** | **str** |  | [optional] 
**dealer** | [**Dealer**](Dealer.md) |  | 
**number_of_campaign_members** | **int** |  | [optional] [default to 0]
**deal_value** | **str** |  | [optional] 
**potential_renewals** | **int** |  | [optional] [default to 0]
**total_residuals** | **str** |  | [optional] 
**total_eligible_revenue** | **str** |  | [optional] 
**last_spoken_date** | **datetime** |  | [optional] 
**last_activity_date** | **datetime** |  | [optional] 
**additions_in_year** | **int** |  | [optional] 
**ineligibles** | **int** |  | [optional] 
**subs_gps** | **int** |  | [optional] 
**subs_hspa** | **int** |  | [optional] 
**subs_cdma** | **int** |  | [optional] 
**subs_mike** | **int** |  | [optional] 
**subs_modems** | **int** |  | [optional] 
**prev_external_user_id** | **str** |  | [optional] 
**carrier_statistics** | **int** |  | [optional] 
**not_client** | **int** |  | [optional] 
**status** | **int** |  | [optional] [default to 0]
**attempt** | **int** |  | [optional] [default to 0]
**call_type** | **int** |  | [optional] 
**call_date** | **datetime** |  | [optional] 
**original_external_user_id** | **str** |  | [optional] 
**date_added** | **datetime** |  | [optional] 
**proposed_account_id** | **int** |  | [optional] 
**website** | **str** |  | [optional] 
**business_hours** | **str** |  | [optional] 
**vertical** | **str** |  | [optional] 
**source_id** | **int** |  | [optional] 
**source** | **str** |  | [optional] [default to 'api']
**customer_external_id** | **str** |  | [optional] 
**coupon_code** | **str** |  | [optional] 
**current_carrier_id** | **int** |  | [optional] 
**preferred_carrier_id** | **int** |  | [optional] 
**old_ban** | **str** |  | [optional] 
**customer_business_unit_customer_id** | **str** |  | [optional] 
**brand_id** | **int** |  | [optional] 
**seat_type** | **str** |  | [optional] 
**rpt_bu** | **str** |  | [optional] 
**record_owned** | **bool** |  | [optional] [default to True]
**account_subtype** | **str** |  | [optional] 
**date_created** | **datetime** |  | [optional] 
**date_updated** | **datetime** |  | [optional] 
**brand** | [**Brand**](Brand.md) |  | 

## Example

```python
from statflo_python_sdk.models.account import Account

# TODO update the JSON string below
json = "{}"
# create an instance of Account from a JSON string
account_instance = Account.from_json(json)
# print the JSON string representation of the object
print(Account.to_json())

# convert the object into a dict
account_dict = account_instance.to_dict()
# create an instance of Account from a dict
account_from_dict = Account.from_dict(account_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


