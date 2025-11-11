# AddressesDef


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addresses** | [**List[AddressSummaryDef]**](AddressSummaryDef.md) |  | [optional] 

## Example

```python
from royal_mail_address_codegen.models.addresses_def import AddressesDef

# TODO update the JSON string below
json = "{}"
# create an instance of AddressesDef from a JSON string
addresses_def_instance = AddressesDef.from_json(json)
# print the JSON string representation of the object
print(AddressesDef.to_json())

# convert the object into a dict
addresses_def_dict = addresses_def_instance.to_dict()
# create an instance of AddressesDef from a dict
addresses_def_from_dict = AddressesDef.from_dict(addresses_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


