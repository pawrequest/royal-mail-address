# AddressRecordDef

Full and detailed address record as available in the address store

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_id** | **str** | Unique identifier for address record retrieval | [optional] 
**domestic_id** | **str** | Domestic ID | [optional] 
**language** | **str** | Language of the result | [optional] 
**language_alternatives** | **str** | Available language alternatives | [optional] 
**department** | **str** | Department | [optional] 
**company** | **str** | Company name | [optional] 
**sub_building** | **str** | Building name | [optional] 
**building_number** | **str** | Building number | [optional] 
**building_name** | **str** | Building name | [optional] 
**secondary_street** | **str** | Secondary Street name | [optional] 
**street** | **str** | Street name | [optional] 
**block** | **str** | block number | [optional] 
**neighbourhood** | **str** | Neighbourhood name | [optional] 
**district** | **str** | District name | [optional] 
**city** | **str** | City name | [optional] 
**line1** | **str** | Address Line 1 | [optional] 
**line2** | **str** | Address Line 2 | [optional] 
**line3** | **str** | Address Line 3 | [optional] 
**line4** | **str** | Address Line 4 | [optional] 
**line5** | **str** | Address Line 5 | [optional] 
**admin_area_name** | **str** | Admin area | [optional] 
**admin_area_code** | **str** | Admin area code | [optional] 
**province** | **str** | Province | [optional] 
**province_name** | **str** | ProvinceName | [optional] 
**province_code** | **str** | Province Code | [optional] 
**postal_code** | **str** | Postal Code | [optional] 
**country_name** | **str** | Country Name | [optional] 
**country_iso2** | **str** | 2 digit Country Iso code | [optional] 
**country_iso3** | **str** | 3 digit Country Iso code | [optional] 
**country_iso_number** | **str** | Country Iso Number | [optional] 
**sorting_number1** | **str** | Sorting Number 1 | [optional] 
**sorting_number2** | **str** | Sorting Number 2 | [optional] 
**barcode** | **str** | Barcode with DPS | [optional] 
**po_box_number** | **str** | PO Box Number | [optional] 
**label** | **str** | Label | [optional] 
**type** | **str** | Type | [optional] 
**data_level** | **str** | Data Level | [optional] 

## Example

```python
from royal_mail_address_codegen.models.address_record_def import AddressRecordDef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressRecordDef from a JSON string
address_record_def_instance = AddressRecordDef.from_json(json)
# print the JSON string representation of the object
print(AddressRecordDef.to_json())

# convert the object into a dict
address_record_def_dict = address_record_def_instance.to_dict()
# create an instance of AddressRecordDef from a dict
address_record_def_from_dict = AddressRecordDef.from_dict(address_record_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


