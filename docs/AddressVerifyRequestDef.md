# AddressVerifyRequestDef


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addresses** | [**List[AddressVerifydef]**](AddressVerifydef.md) |  | [optional] 

## Example

```python
from royal_mail_address_codegen.models.address_verify_request_def import AddressVerifyRequestDef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressVerifyRequestDef from a JSON string
address_verify_request_def_instance = AddressVerifyRequestDef.from_json(json)
# print the JSON string representation of the object
print(AddressVerifyRequestDef.to_json())

# convert the object into a dict
address_verify_request_def_dict = address_verify_request_def_instance.to_dict()
# create an instance of AddressVerifyRequestDef from a dict
address_verify_request_def_from_dict = AddressVerifyRequestDef.from_dict(address_verify_request_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


