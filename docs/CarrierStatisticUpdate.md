# CarrierStatisticUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**approach** | **str** |  | [optional] 
**phone_number** | **str** |  | 
**contact_name** | **str** |  | [optional] 
**total_subscriber** | **int** |  | [optional] 
**potential_renewal** | **int** |  | [optional] 
**campaign_date_added** | **datetime** |  | 
**campaign_id** | **str** |  | 
**cbucid** | **int** |  | [optional] 
**email** | **str** |  | [optional] 
**street** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**total_tablets** | **int** |  | [optional] 
**total_roam_ready** | **int** |  | [optional] 
**total_link_subs** | **int** |  | [optional] 
**total_conferences** | **int** |  | [optional] 
**total_geotrac** | **int** |  | [optional] 
**total_fleet** | **int** |  | [optional] 
**subscriber_details** | **str** |  | [optional] 
**vertical** | **str** |  | [optional] 
**vertical_detailed** | **str** |  | [optional] 
**avg_data_usage** | **int** |  | [optional] 
**avg_minutes_usage** | **int** |  | [optional] 
**avg_long_distance_usage** | **int** |  | [optional] 
**avg_roaming_usage** | **int** |  | [optional] 
**avg_data_overage** | **int** |  | [optional] 
**avg_minutes_overage** | **int** |  | [optional] 
**avg_ld_overage** | **int** |  | [optional] 
**avg_roam_overage** | **int** |  | [optional] 
**purchase_probability_tablet** | **str** |  | [optional] 
**purchase_probability_roam_ready** | **str** |  | [optional] 
**purchase_probability_fleet_complete** | **str** |  | [optional] 
**purchase_probability_conferences** | **str** |  | [optional] 
**purchase_probability_device_care_warranty** | **str** |  | [optional] 
**last_spoken_date** | **datetime** |  | [optional] 
**last_activity_date** | **datetime** |  | [optional] 
**original_rep** | **str** |  | [optional] 
**sales_rep_id** | **str** |  | [optional] 
**activity_type** | **int** |  | [optional] 
**total_no_of_eligible_subs** | **int** |  | [optional] 
**purchase_probability_busconnect** | **str** |  | [optional] 
**busex_dealer** | **str** |  | [optional] 
**optik_eligibility** | **str** |  | [optional] 
**telus_home_phone_customer** | **str** |  | [optional] 
**telus_internet_customer** | **str** |  | [optional] 
**tactic** | **str** |  | [optional] 
**likely_to_buy_data** | **str** |  | [optional] 
**last_booked_appointment** | **datetime** |  | [optional] 
**wireline** | **str** |  | [optional] 
**product_list** | **str** |  | [optional] 
**number_of_employees** | **int** |  | [optional] 
**cable_footprint** | **str** |  | [optional] 
**service_id** | **str** |  | [optional] 
**avg_rpu** | **int** |  | [optional] 
**bts_discount** | **str** |  | [optional] 
**pap** | **str** |  | [optional] 
**outlet_id** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.carrier_statistic_update import CarrierStatisticUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CarrierStatisticUpdate from a JSON string
carrier_statistic_update_instance = CarrierStatisticUpdate.from_json(json)
# print the JSON string representation of the object
print(CarrierStatisticUpdate.to_json())

# convert the object into a dict
carrier_statistic_update_dict = carrier_statistic_update_instance.to_dict()
# create an instance of CarrierStatisticUpdate from a dict
carrier_statistic_update_from_dict = CarrierStatisticUpdate.from_dict(carrier_statistic_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


