# onReadyEvent
## Description
The `onReadyEvent` event is called when `JG_API` has finished loading and is ready to be used by code accessing it's API.
## Functions
### getJGAPI()
Returns the instance of JG_API that is currently being used.
## Example Usage
 ```
 @Override
 public void onReadyEvent(ReadyEvent event) {
    JG_API jg_api = event.getJGAPI();
 }
 ```
 ## Last Updated
 2022/06/15