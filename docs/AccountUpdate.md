# AccountUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**account_id** | **str** |  | 
**account_type** | **str** |  | [optional] 
**external_user_id** | **str** |  | [optional] 
**external_location_id** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**number_of_campaign_members** | **int** |  | [optional] 
**deal_value** | **str** |  | [optional] 
**potential_renewals** | **int** |  | [optional] 
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
**status** | **int** |  | [optional] 
**attempt** | **int** |  | [optional] 
**call_type** | **int** |  | [optional] 
**call_date** | **datetime** |  | [optional] 
**original_external_user_id** | **str** |  | [optional] 
**date_added** | **datetime** |  | [optional] 
**proposed_account_id** | **int** |  | [optional] 
**website** | **str** |  | [optional] 
**business_hours** | **str** |  | [optional] 
**vertical** | **str** |  | [optional] 
**source_id** | **int** |  | [optional] 
**source** | **str** |  | [optional] 
**customer_external_id** | **str** |  | [optional] 
**coupon_code** | **str** |  | [optional] 
**current_carrier_id** | **int** |  | [optional] 
**preferred_carrier_id** | **int** |  | [optional] 
**old_ban** | **str** |  | [optional] 
**customer_business_unit_customer_id** | **str** |  | [optional] 
**brand_id** | **int** |  | [optional] 
**seat_type** | **str** |  | [optional] 
**rpt_bu** | **str** |  | [optional] 
**record_owned** | **bool** |  | [optional] 
**account_subtype** | **str** |  | [optional] 
**date_created** | **datetime** |  | [optional] 
**date_updated** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_update import AccountUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountUpdate from a JSON string
account_update_instance = AccountUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountUpdate.to_json())

# convert the object into a dict
account_update_dict = account_update_instance.to_dict()
# create an instance of AccountUpdate from a dict
account_update_from_dict = AccountUpdate.from_dict(account_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


