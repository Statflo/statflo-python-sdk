# AccountMemberUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**account_id** | **str** |  | [optional] 
**phone_number** | **str** |  | 
**account_type** | **str** |  | [optional] 
**language** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**account_member_name** | **str** |  | [optional] 
**service** | **str** |  | [optional] 
**product** | **str** |  | [optional] 
**service_start_date** | **datetime** |  | [optional] 
**service_end_date** | **datetime** |  | [optional] 
**location_id** | **str** |  | [optional] 
**date_created** | **datetime** |  | [optional] 
**trade_in** | **str** |  | [optional] 
**imei** | **str** |  | [optional] 
**esn_dec** | **str** |  | [optional] 
**eduf** | **float** |  | [optional] 
**contact_term** | **int** |  | [optional] 
**contact_months_left** | **int** |  | [optional] 
**units** | **str** |  | [optional] 
**street_number** | **str** |  | [optional] 
**street_name** | **str** |  | [optional] 
**unit_type** | **str** |  | [optional] 
**unit** | **str** |  | [optional] 
**po_box** | **str** |  | [optional] 
**rr** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**home_phone** | **str** |  | [optional] 
**business_phone** | **str** |  | [optional] 
**business_extensions** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**status** | **bool** |  | [optional] 
**avg_data_usage** | **int** |  | [optional] 
**avg_minutes_usage** | **int** |  | [optional] 
**avg_long_distance_usage** | **int** |  | [optional] 
**avg_roaming_usage** | **int** |  | [optional] 
**avg_data_overage** | **int** |  | [optional] 
**avg_mins_overage** | **int** |  | [optional] 
**avg_ld_overage** | **float** |  | [optional] 
**avg_roam_overage** | **float** |  | [optional] 
**campaign_type** | **str** |  | [optional] 
**campaign_id** | **str** |  | [optional] 
**avg_rpu** | **float** |  | [optional] 
**tab** | **float** |  | [optional] 
**tab_charge** | **float** |  | [optional] 
**tab_date** | **datetime** |  | [optional] 
**source** | **str** |  | [optional] 
**source_id** | **int** |  | [optional] 
**customer_external_id** | **str** |  | [optional] 
**old_ban** | **str** |  | [optional] 
**salesforce_line_id** | **str** |  | [optional] 
**byod_customer** | **str** |  | [optional] 
**prepaid** | **str** |  | [optional] 
**subscriber_id** | **str** |  | [optional] 
**port_in_carrier_id** | **int** |  | [optional] 
**port_in_carrier_name** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_member_update import AccountMemberUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountMemberUpdate from a JSON string
account_member_update_instance = AccountMemberUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountMemberUpdate.to_json())

# convert the object into a dict
account_member_update_dict = account_member_update_instance.to_dict()
# create an instance of AccountMemberUpdate from a dict
account_member_update_from_dict = AccountMemberUpdate.from_dict(account_member_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


