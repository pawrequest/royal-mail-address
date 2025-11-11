# AddressVerifydef

Summary of the matching address

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address_line1** | **str** |  | 
**address_line2** | **str** |  | [optional] 
**address_line3** | **str** |  | [optional] 
**post_town** | **str** |  | 
**county** | **str** |  | [optional] 
**postcode** | **str** |  | 

## Example

```python
from royal_mail_address_codegen.models.address_verifydef import AddressVerifydef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressVerifydef from a JSON string
address_verifydef_instance = AddressVerifydef.from_json(json)
# print the JSON string representation of the object
print(AddressVerifydef.to_json())

# convert the object into a dict
address_verifydef_dict = address_verifydef_instance.to_dict()
# create an instance of AddressVerifydef from a dict
address_verifydef_from_dict = AddressVerifydef.from_dict(address_verifydef_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


