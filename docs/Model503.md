# Model503


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_code** | **str** | HTTP error code.  Please note that this will only be populated in the event of an error condition. | 
**http_message** | **str** | HTTP error code description. Please note that this will only be populated in the event of an error condition. | 
**more_information** | **str** | Information relating to the error condition. | [optional] 
**errors** | [**List[ErrorsDef]**](ErrorsDef.md) |  | [optional] 

## Example

```python
from royal_mail_address_codegen.models.model503 import Model503

# TODO update the JSON string below
json = "{}"
# create an instance of Model503 from a JSON string
model503_instance = Model503.from_json(json)
# print the JSON string representation of the object
print(Model503.to_json())

# convert the object into a dict
model503_dict = model503_instance.to_dict()
# create an instance of Model503 from a dict
model503_from_dict = Model503.from_dict(model503_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


