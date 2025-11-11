# ErrorsDef

Array containing error information.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Code associated with the error condition | [optional] 
**description** | **str** | Description of the error condition | [optional] 
**cause** | **str** | Cause of the error (if known) | [optional] 
**resolution** | **str** | Description of the resolution and action required to correct the error | [optional] 

## Example

```python
from royal_mail_address_codegen.models.errors_def import ErrorsDef

# TODO update the JSON string below
json = "{}"
# create an instance of ErrorsDef from a JSON string
errors_def_instance = ErrorsDef.from_json(json)
# print the JSON string representation of the object
print(ErrorsDef.to_json())

# convert the object into a dict
errors_def_dict = errors_def_instance.to_dict()
# create an instance of ErrorsDef from a dict
errors_def_from_dict = ErrorsDef.from_dict(errors_def_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


