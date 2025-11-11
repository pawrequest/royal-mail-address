# AddressVerifyReqRespdef

Returns the DPS

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**input** | [**AddressVerifydef**](AddressVerifydef.md) |  | [optional] 
**dps** | **str** |  | [optional] 

## Example

```python
from royal_mail_address_codegen.models.address_verify_req_respdef import AddressVerifyReqRespdef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressVerifyReqRespdef from a JSON string
address_verify_req_respdef_instance = AddressVerifyReqRespdef.from_json(json)
# print the JSON string representation of the object
print(AddressVerifyReqRespdef.to_json())

# convert the object into a dict
address_verify_req_respdef_dict = address_verify_req_respdef_instance.to_dict()
# create an instance of AddressVerifyReqRespdef from a dict
address_verify_req_respdef_from_dict = AddressVerifyReqRespdef.from_dict(address_verify_req_respdef_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


