# AddressSummaryDef

Summary of the matching address

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_id** | **str** | Unique identifier for address record retrieval | [optional] 
**type** | **str** | Type of the response entity | [optional] 
**address_summary1** | **str** | Address Line 3 | [optional] 
**address_summary2** | **str** | PostTown | [optional] 
**highlight** | **str** | A list of number ranges identifying the matched characters in the Text and Description | [optional] 

## Example

```python
from royal_mail_address_codegen.models.address_summary_def import AddressSummaryDef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressSummaryDef from a JSON string
address_summary_def_instance = AddressSummaryDef.from_json(json)
# print the JSON string representation of the object
print(AddressSummaryDef.to_json())

# convert the object into a dict
address_summary_def_dict = address_summary_def_instance.to_dict()
# create an instance of AddressSummaryDef from a dict
address_summary_def_from_dict = AddressSummaryDef.from_dict(address_summary_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


