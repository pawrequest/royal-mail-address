# AddressFindRequestDef

Address search string

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_text** | **str** | Full address search string | 

## Example

```python
from royal_mail_address_codegen.models.address_find_request_def import AddressFindRequestDef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressFindRequestDef from a JSON string
address_find_request_def_instance = AddressFindRequestDef.from_json(json)
# print the JSON string representation of the object
print(AddressFindRequestDef.to_json())

# convert the object into a dict
address_find_request_def_dict = address_find_request_def_instance.to_dict()
# create an instance of AddressFindRequestDef from a dict
address_find_request_def_from_dict = AddressFindRequestDef.from_dict(address_find_request_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


